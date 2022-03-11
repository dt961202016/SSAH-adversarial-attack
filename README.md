Introduction
=
This is an official release of the CVPR2022 paper  **"Frequency-driven Imperceptible Adversarial Attack on Semantic Similarity"** (arxiv link). 


__Abstract:__ lity of learning-based classifiers against carefully crafted perturbations. However, most existing attack methods have inherent limitations in cross-dataset generalization as they rely on a classification layer with a closed set of categories. Furthermore, the perturbations generated by these methods may appear in regions easily perceptible to the human visual system (HVS). To circumvent the former problem, we propose a novel algorithm that attacks semantic similarity on feature representations. In this way, we are able to fool classifiers without limiting attacks to a specific dataset. For imperceptibility, we introduce the low-frequency constraint to limit perturbations within high-frequency components, ensuring perceptual similarity between adversarial examples and originals. Extensive experiments on three datasets(CIFAR-10, CIFAR-100, and ImageNet-1K) and three public online platforms indicate that our attack can yield misleading and transferable adversarial examples across architectures and datasets. Additionally, visualization results and quantitative performance (in terms of four different metrics) show that the proposed algorithm generates more imperceptible perturbations than the state-of-the-art methods. Our code will be publicly available.

Requirements
=
* python ==3.6
* torch == 1.7.0
* torchvision >= 0.7
* numpy == 1.19.2
* Pillow == 8.0.1
* pywt

Required Dataset
=
1. The data structure of Cifar10, Cifar100, ImageNet or any other datasets look like below. Please modify the dataloader at `SSAH-Adversarial-master/main.py/` accordingly for your dataset structure.

```
/dataset/
├── Cifar10
│   │   ├── cifar-10-python.tar.gz
├── Cifar-100-python
│   │   ├── cifar-100-python.tar.gz
├── imagenet
│   ├── val
│   │   ├── n02328150

```

Citation
=
Acknowledgements
=

