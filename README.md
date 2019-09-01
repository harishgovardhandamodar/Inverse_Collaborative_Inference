# Model Inverse Attack against Collaborative Inference

This code implements model inversion attacks against collaborative inference in the following paper:

Zecheng He, Tianwei Zhang and Ruby Lee, "Model Inversion Attacks Against Collaborative Inference", 35th Annual Computer Security Applications Conference (ACSAC'19), San Juan, Dec 2019

#### 1.Pre-requisite:
#### python 2.7
#### numpy
pip install numpy
#### pytorch
pip install torch
#### torchvision version 0.2.1:
pip install torchvision==0.2.1

#### 2.Run the code:
#### (1) Train the target CIFAR model to inverse

python training.py --dataset CIFAR10 --epochs 50

#### (2) Whitebox Regularized Maximum Likelihood Estimation (rMLE)

python inverse_whitebox_CIFAR.py --iters 5000 --learning_rate 1e-2 --layer conv11 --lambda_TV 0.0 --lambda_l2 0.0

#### (3) Blackbox Inverse Network


#### (4) Access-free Attack

#### 3.Reference
