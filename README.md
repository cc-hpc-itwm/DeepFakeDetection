# [Unmasking DeepFake with simple Features](https://arxiv.org/abs/1905.12534)

This repository provides the official Python implementation of Unmasking DeepFake with simple Features. 
## Dependencies
Tested on Python 3.6.x.
* [NumPy](http://www.numpy.org/) (1.16.2)
* [Opencv](https://opencv.org/opencv-4-0/) (4.0.0)
* [Matplotlib](https://matplotlib.org/) (3.1.1)



## Analysis Faces-HQ
To the best of our knowledge, no public dataset gathers images containing both artificially and real faces, therefore, we have created our own called Faces-HQ.
In order to have a sufficient variety of faces, we have chosen to download and label, images available from [CelebA-HQ dataset](https://arxiv.org/abs/1710.10196),
[Flickr-Faces-HQ dataset](https://arxiv.org/abs/1812.04948), [100K Facesproject](https://generated.photos/) and [www.thispersondoesnotexist.com](www.thispersondoesnotexist.com). In total, we have collected 40K high quality
images being half of them real and the other half fake faces, achieving in this manner a balanced dataset.

Click [here](/Experiments_Faces-HQ) to go the experiments on DeepFakeDetection.

## Analysis DeepFakeDetection (FaceForensics++)
 [FaceForensics++](https://github.com/ondyari/FaceForensics) is a forensics dataset consisting of video sequences that have been modified with
different automated face manipulation methods. Additionally,it is hosting DeepFakeDetection Dataset. In particular, this dataset contains 363 original
sequences from 28 paid actors in 16 different scenes as well as over 3000 manipulated videos using DeepFakes and their corresponding binary masks.
All videos contain a trackable mostly frontal face without occlusions which enables automated tampering methods to generate realistic forgeries.

Click [here](/Experiments_DeepFakeDetection) to go the experiments on DeepFakeDetection.



### Comparision between DCGAN with and wihtout Octave Convolution

![DCGAN with Octave Conv.](imgs/evo.png) 

## References

This repo combines the pytorch implementation of the following paper:

>Karras et al. [Progressive growing of gans for improved quality, stability, and variation](https://arxiv.org/abs/1710.10196).
>Karras et al. [A Style-Based Generator Architecture for Generative Adversarial Networks](https://arxiv.org/abs/1812.04948).


### Citation
If this work is useful for your research, please cite our [paper](https://arxiv.org/abs/1905.12534):
```
@article{durall2019dropgan,
  title={Stabilizing GANs with Octave Convolutions},
  author={Durall, Ricard and Pfreundt, Franz-Josef and Keuper, Janis},
  journal={arXiv preprint arXiv:1905.12534},
  year={2019}
}
```
