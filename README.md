# Early Stage Flame Dataset ESFD

Early Stage Flame Dataset (ESFD) is a newly published dataset consisting of fire and non-fire images that have occurred in both forest and urban environments collected via the Internet. Images are captured in real-life situations by firefighters or journalists in the area of the Balkan Peninsula. The total number of images is 500, of which 300 images (60%) were used for training, 50 (10%) for validation, and 150 (30%) for testing. The details about the subsets in the dataset are provided below. 

| Subset       | Flame images | Non-flame images | Total in subset |
| :----------- | :----------: | ---------------: | --------------: |
| Train        |  97 (32.34%) |     203 (67.66%) |       300 (60%) |
| Validation   |  16 (32.00%) |      34 (68.00%) |        50 (10%) |
| Test         |  61 (41.06%) |      89 (58.94%) |       150 (30%) |
| Total        | 174 (34.80%) |     326 (65.20%) |             500 |

In Fig. 1. and Fig. 2. some examples of images with and without fire are provided, respectively. The data labeling process is conducted with Segments.ai. The ground truth images are normalized to values 0 and 1, where pixels representing flame are labeled as 1, while pixels representing non-flame objects are labeled as 0. The total number of pixels in the dataset, as represented with ground truth images, is 131, 072, 000.
![Examples of images in the dataset](/imgs/ESFD.png "Examples of different categories of images.").


The distribution of pixels in the dataset is presented in the Table below. Table shows that the number of flame pixels is significantly lower than the number of non-flame pixels, with a ratio of approximately 1:111. Most images in our dataset have minimal indicators of flame presence, making this dataset unique in the literature. It is evident that this dataset is imbalanced, posing a greater challenge for detection. Unlike existing datasets, such as Corsican Fire DataBase (CFDB), which only contain fire images and have a higher percentage of fire pixels (around 23%) and non-fire pixels (77%),our dataset includes images without flame pixels, which is crucial for accurately detecting early signs of fire presence and avoiding false alarms. This is particularly important in early fire detection to alert firefighters in a timely manner.

|              | Flame pixels | Non-flame pixels | Total pixels |
| :----------- | :----------: | ---------------: | -----------: |
| Dataset      |    1,161,704 |      129,910,296 |  131,072,000 |
| Percentage   |       0.886% |          99.114% |         100% |

## How to download the dataset?

The link to the dataset is provided with Google Drive link: will be provided shortly

## How to cite our work?

More details about the dataset is provided in two papers shown below. 

When utilizing our dataset, we kindly request that you acknowledge our contribution by citing our work.

```bibtex
@inproceedings{vsabanovic2023early,
  title={Early Stage Flame Segmentation with DeepLabv3+ and Weighted Cross-Entropy},
  author={{\v{S}}abanovi{\'c}, Adnan and Ahmetspahi{\'c}, Negra and Kapo, Medina and Buza, Emir and Akagic, Amila},
  booktitle={2023 XXIX International Conference on Information, Communication and Automation Technologies (ICAT)},
  pages={1--6},
  year={2023},
  organization={IEEE}
}```

```bibtex
@inproceedings{kapo2023early,
  title={Early stage flame segmentation with deep learning and intel's openvino toolkit},
  author={Kapo, Medina and {\v{S}}abanovi{\'c}, Adnan and Akagic, Amila and Buza, Emir},
  booktitle={2023 XXIX International Conference on Information, Communication and Automation Technologies (ICAT)},
  pages={1--6},
  year={2023},
  organization={IEEE}
}```

## Results of DeepLabv3+ with Weighted Cross-Entropy

![Examples of results](/imgs/ESFD_results.png "Examples of results Early Stage Flame Segmentation with DeepLabv3+
and Weighted Cross-Entropy.").
