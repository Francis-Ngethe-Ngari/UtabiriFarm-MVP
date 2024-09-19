tfds.core.DatasetInfo(
    name='plant_village',
    full_name='plant_village/1.0.2',
    description="""
    The PlantVillage dataset consists of 54303 healthy and unhealthy leaf images
    divided into 38 categories by species and disease.
    
    NOTE: The original dataset is not available from the original source
    (plantvillage.org), therefore we get the unaugmented dataset from a paper that
    used that dataset and republished it. Moreover, we dropped images with
    Background_without_leaves label, because these were not present in the original
    dataset.
    
    Original paper URL: https://arxiv.org/abs/1511.08060 Dataset URL:
    https://data.mendeley.com/datasets/tywbtsjrjv/1
    """,
    homepage='https://arxiv.org/abs/1511.08060',
    data_dir='/home/francis/tensorflow_datasets/plant_village/1.0.2',
    file_format=tfrecord,
    download_size=827.82 MiB,
    dataset_size=815.37 MiB,
    features=FeaturesDict({
        'image': Image(shape=(None, None, 3), dtype=uint8),
        'image/filename': Text(shape=(), dtype=string),
        'label': ClassLabel(shape=(), dtype=int64, num_classes=38),
    }),
    supervised_keys=('image', 'label'),
    disable_shuffling=False,
    splits={
        'train': <SplitInfo num_examples=54303, num_shards=8>,
    },
    citation="""@article{DBLP:journals/corr/HughesS15,
      author    = {David P. Hughes and
                   Marcel Salath{\'{e}}},
      title     = {An open access repository of images on plant health to enable the
                   development of mobile disease diagnostics through machine
                   learning and crowdsourcing},
      journal   = {CoRR},
      volume    = {abs/1511.08060},
      year      = {2015},
      url       = {http://arxiv.org/abs/1511.08060},
      archivePrefix = {arXiv},
      eprint    = {1511.08060},
      timestamp = {Mon, 13 Aug 2018 16:48:21 +0200},
      biburl    = {https://dblp.org/rec/bib/journals/corr/HughesS15},
      bibsource = {dblp computer science bibliography, https://dblp.org}
    }""",
)
