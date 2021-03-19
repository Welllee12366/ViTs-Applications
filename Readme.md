# Vision Transformer(s) and Its application
A reimplementation of the SOTA vision transformers(ViTs).\
Most of the codes from this repository are **borrowed** from other authors, but we cite them and adaptive the codes for our usage.
# To-do
* Reimplement [Vision Transformer(ViT)](https://github.com/jeonsworld/ViT-pytorch) --Doing
* Reimplement SETR for Semantic Segmentation---Next Step
# Environment
#### OS: 
> Ubuntu Desktop 16.04 or higher
### Hardwares:  
> * Tesla V100 with 16G/32G * n
> * Nvidia RTX 3090 with 24G * n
#### CUDA Envs:
> - For Tesla:  CUDA version is 10.2 or higher
> - For RTX30 Series: CUDA version is 11.0 or higher
#### Python Version:
> higher than 3.6 but less than 3.8
# Requirements
> * tqdm
> * ml_collections
> * [torch](https://pytorch.org)
> * [torchvision](https://pytorch.org)
> * [apex](https://github.com/NVIDIA/apex)

# Vision Transoformer(ViT)
This paper show that Transformers applied directly to image patches and pre-trained on large datasets work really well on image recognition task.
![alt Vision Transformer](figures/vit.gif)
Vision Transformer achieve State-of-the-Art in image recognition task with standard Transformer encoder and fixed-size patches. In order to perform classification, author use the standard approach of adding an extra learnable "classification token" to the sequence.
![alt ViT_Experimental](figures/vit_exp.png)
## Pretrained Models
### [Available Models(Click here)](https://console.cloud.google.com/storage/vit_models/)
* Imagenet21k pre-train models
    > ViT-B_16, ViT-B_32, ViT-L_16, ViT-L_32, ViT-H_14
* Imagenet21k & Imagenet2012 fine-tuned models
    > ViT-B_16-224, ViT-B_16, ViT-B_32, ViT-L_16-224, ViT-L_16, ViT-L_32
* Hybrid Model(ResNet-50 & Transformer)
    > R50-ViT-B_16
# Citations
    @article{dosovitskiy2020,
    title={An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale},
    author={Dosovitskiy, Alexey and Beyer, Lucas and Kolesnikov, Alexander and Weissenborn, Dirk and Zhai, Xiaohua and Unterthiner, Thomas and  Dehghani, Mostafa and Minderer, Matthias and Heigold, Georg and Gelly, Sylvain and Uszkoreit, Jakob and Houlsby, Neil},
    journal={arXiv preprint arXiv:2010.11929},
    year={2020}
    }
# Disclaimer
This repository is only use for research. If it violates your rights and interests, please **submit an issue** to contact us. We will respond as soon as possible. At the same time, we also invite you to help us improve it!