# Split Dataset for Model Training

This repository contains the processed datasets used for training and evaluating the machine learning models in KSGAN.

## Dataset Overview

The dataset is divided into training, validation, and test sets. The training set contains different versions generated using different data augmentation methods, while the validation and test sets are kept unchanged across experiments.

| Set   | Version       | Augmentation  | Excellent |      Good |   Dropout | Total Samples | Dataset                                                            |
| ----- | ------------- | ------------- | --------: | --------: | --------: | ------------: | ------------------------------------------------------------------ |
| Train | VMedian       | –             |     1,783 |     4,839 | 1,852,997 |     1,859,619 | [Kaggle](https://www.kaggle.com/datasets/anhtran10/lo-dataset)     |
| Train | VSMOTE        | SMOTE         | 1,852,997 | 1,852,997 | 1,852,997 |     5,558,991 | [Kaggle](https://www.kaggle.com/datasets/uyentran10/lo-smote-test) |
| Train | VGAN          | GAN           | 1,852,997 | 1,852,997 | 1,852,997 |     5,558,991 | [Kaggle](https://www.kaggle.com/datasets/anhtran10/lo-gan-test)    |
| Train | VK-MeansSMOTE | K-Means SMOTE | 1,852,995 | 1,852,995 | 1,852,997 |     5,558,987 | [Kaggle](https://www.kaggle.com/datasets/anhtran10/lo-dataset)     |
| Train | VSMOTifiedGAN | SMOTified GAN | 1,852,997 | 1,852,997 | 1,852,997 |     5,558,991 | [Kaggle](https://www.kaggle.com/datasets/anhtran10/lo-dataset)     |
| Train | VKSGAN        | KSGAN         | 1,852,995 | 1,852,995 | 1,852,997 |     5,558,987 | [Kaggle](https://www.kaggle.com/datasets/hngliththu/cdsmote-gan)   |
| Val   | All           | –             |       223 |       605 |   231,625 |       232,453 | [Kaggle](https://www.kaggle.com/datasets/anhtran10/lo-dataset)     |
| Test  | All           | –             |       223 |       605 |   231,624 |       232,452 | [Kaggle](https://www.kaggle.com/datasets/anhtran10/lo-dataset)     |

## Dataset Details

### Training Sets

- **VMedian**: Training set after median imputation without data augmentation.
- **VSMOTE**: Training set augmented using SMOTE.
- **VGAN**: Training set augmented using GAN.
- **VK-MeansSMOTE**: Training set augmented using K-Means SMOTE.
- **VSMOTifiedGAN**: Training set augmented using SMOTified GAN.
- **VKSGAN**: Training set augmented using the proposed KSGAN method.

### Validation and Test Sets

The validation and test sets are shared across all training configurations and are not augmented.

- **Val**: Validation set containing 232,453 samples.
- **Test**: Test set containing 232,452 samples.

## Dataset Access

The datasets can be accessed through the following Kaggle resources:

- **VMedian**: The `Median/Median` directory in the [Kaggle dataset](https://www.kaggle.com/datasets/anhtran10/lo-dataset).
- **VSMOTE**: [Kaggle dataset](https://www.kaggle.com/datasets/uyentran10/lo-smote-test).
- **VGAN**: [Kaggle dataset](https://www.kaggle.com/datasets/anhtran10/lo-gan-test).
- **VK-MeansSMOTE**: The `Median/Median` directory in the [Kaggle dataset](https://www.kaggle.com/datasets/anhtran10/lo-dataset).
- **VSMOTifiedGAN**: The `Median/Median` directory in the [Kaggle dataset](https://www.kaggle.com/datasets/anhtran10/lo-dataset).
- **VKSGAN**: [Kaggle dataset](https://www.kaggle.com/datasets/hngliththu/cdsmote-gan).
- **Validation and Test sets**: The `Median/Median` directory in the [Kaggle dataset](https://www.kaggle.com/datasets/anhtran10/lo-dataset).
