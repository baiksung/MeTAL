# MeTAL - Meta-Learning with Task-Adaptive Loss Function for Few-Shot Learning
#### Sungyong Baik, Janghoon Choi, Heewon Kim, Dohee Cho, Jaesik Min, Kyoung Mu Lee

Official Pytorch implementation of [Meta-Learning with Task-Adaptive Loss Function for Few-Shot Learning](https://openaccess.thecvf.com/content/ICCV2021/papers/Baik_Meta-Learning_With_Task-Adaptive_Loss_Function_for_Few-Shot_Learning_ICCV_2021_paper.pdf)

The code is based off the public code of [MAML++](https://github.com/AntreasAntoniou/HowToTrainYourMAMLPytorch), where their reimplementation of MAML is used as the baseline.

[Paper-arXiv](http://arxiv.org/abs/2110.03909)

## Requirements

Ubuntu 18.04
- Anaconda3
- Python==3.7.10
- PyTorch==1.4
- numpy==1.19.2

To install requirements, first download Anaconda3 and then run the following:
```setup
conda create -n metal python=3.7
conda activate metal
bash install.sh
```

## Datasets
For miniIamgenet, the dataset can be downloaded from the [link](https://drive.google.com/file/d/1qQCoGoEJKUCQkk8roncWH7rhPN7aMfBr/view) provided from [MAML++ public code](https://github.com/AntreasAntoniou/HowToTrainYourMAMLPytorch).
make a directory named 'datasets' and place the downloaded miniImagnet under the 'datasets' directory.

## Training

To train a model, run the following command in `experiments_scripts` directory

```bash
bash MeTAL.sh $GPU_ID
```

## Evaluation

After training is finished, evaluation is performed automatically.
To run an evaluation manually, run the same command

```bash
bash MeTAL.sh $GPU_ID
```

## Reference
```
@InProceedings{baik2021meta,
 title={IntegralAction: Pose-driven Feature Integration for Robust Human Action Recognition in Videos},
 author={Sungyong Baik, Janghoon Choi, Heewon Kim, Dohee Cho, Jaesik Min, and Kyoung Mu Lee}
 booktitle = {International Conference on Computer Vision (ICCV)}, 
 year={2021}
}
```
