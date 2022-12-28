# Neural Causation Coefficient

An unofficial PyTorch implementation of Neural Causation Coefficient (NCC) in the paper, ["Discovering Causal Signals in Images"](https://arxiv.org/abs/1605.08179).

## Requirements

```shell
torch=1.9.0
torchvision=1.10.0
scikit-learn
scipy
tqdm
numpy
pandas
matplotlib
seaborn
skimage
pycocotools
```

## Usage

0. Download datasets: 1) [Tubingen](https://webdav.tuebingen.mpg.de/cause-effect/) dataset, 2) [PASCAL VOC2012](http://host.robots.ox.ac.uk/pascal/VOC/voc2012/) dataset, and 3) [MSCOCO](https://cocodataset.org/#home) dataset.

1. ```NCC_Training.ipynb```: Train NCC Classifier on synthetic dataset and Test it on Tubingen dataset
    - Our reproduced model ```results/NCC_classifier_best.pt``` showed 78.74% accuracy on Tubingen dataset, which was 79% in the original paper.

2. ```ObjectClassifier_Training.ipynb```: Train object classifier on PASCAL VOC2012 dataset

3. ```NCC_Testing.ipynb```: Test NCC Classifier on MSCOCO dataset

## References
David Lopez-Pas et al., *Discovering Causal Signals in Images*, ICML 2017