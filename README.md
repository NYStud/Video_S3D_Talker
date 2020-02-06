# Video_S3D_Talker

## Features of the project will be:

```
- A transformer based video captioning architecture on YouCook2, MSR-VTT and V2C dataset.

- 3D video features extracted from a largely pre-trained S3D models from HowTo100M dataset.

- Performance reproduced from the recent video representation learning work:
Sun, Chen, et al. "Contrastive bidirectional transformer for temporal representation learning

- Comparisons with other video captioning features like ResNet, or NCE finetuned S3D baselines.
```

## Things to do:
- [x] Initialize the ReadMe.                                            - Feb. 4th
- [x] Upload training script on YC2 Dataset.                            - Feb. 5th
- [ ] Release pre-trained captioning models.                            - Feb. 7th
- [ ] Release extracted video segment features of YC2 using S3D models. - Feb. 7th
- [x] Evaluation script and performances.                               - Feb. 10th
- [ ] Baseline models on MSR-VTT and performances.                      - Feb. 24th

## Performances Comparison on YouCook2 Captioning

| Method  | Features | BLEU-4 | METEOR | ROUGE-L | CIDEr |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| Zhou et al. | ResNet | 4.38 | 11.55 | 27.44 | 0.38 |
| S3D | Kinetic Pre-trained S3D | 3.24 | 9.52 | 26.09 | 0.31 |
| VideoBERT | - | 4.33 | 11.94 | 28.80 | 0.55 |
| CBT | Nce-pretrained S3D | 5.12 | 12.97 | 30.44 | 0.64 |
| Ours | HowTo100M pre-tr. S3D | 3.47 | 10.31 | 33.54 | 0.35 |

## Mention these work if you find it helpful.

  Please cite or mention these works if you find this project helpful: 
  
  ***Our GitHub Project:***
  ```
    @misc{Fang2020,
        author       = {Zhiyuan Fang},
        title        = {Video S3D Talker: transformer based video captioning model using S3D features.},
        month        = {Feb},
        year         = {2020},
        publisher    = {GitHub},
        journal      = {GitHub repository},
        version      = {1.0},
        howpublished = {\url{https://https://github.com/jacobswan1/Video_S3D_Talker}},
        }
  ```
  
  ***HowTo100M:***
  ```
    @inproceedings{miech2019howto100m,
        title={Howto100M: Learning a text-video embedding by watching hundred million narrated video clips},
        author={Miech, Antoine and Zhukov, Dimitri and Alayrac, Jean-Baptiste and Tapaswi, Makarand and Laptev, Ivan and Sivic, Josef},
        booktitle={Proceedings of the IEEE International Conference on Computer Vision},
        pages={2630--2640},
        year={2019}
    }
```

## Acknowledgements

Thanks ***Luowei Zhou*** for sharing his raw videos of [YouCook2 dataset](http://youcook2.eecs.umich.edu/), and  ***Antoine Miech, Jean-Baptiste Alayrac*** for their [HowTo100M pre-trained S3D models](https://github.com/antoine77340/S3D_HowTo100M).

