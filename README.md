# [Unmasking DeepFake with simple Features](https://arxiv.org/abs/1905.12534)

This repository provides the official Python implementation of Unmasking DeepFake with simple Features. 
## Dependencies
Tested on Python 3.6.x.
* [NumPy](http://www.numpy.org/) (1.16.2)



## CelebA dataset
The full [CelebA-HQ](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) is available [here](https://drive.google.com/open?id=1p6WtrxprsjsiedQJkKVoiqvdrP1m9BuF). To resize the RGB images to 128 by 128 pixels, set the path and run `resize_celeba.py`.


### Example hyper-parameters definition (wgan.sh)
```
python train.py --type wgan \
           --nb-epochs 50 \
           --learning-rate 0.00005 \
           --optimizer rmsprop \
           --critic 5 \
           --cuda
```

### Comparision between DCGAN with and wihtout Octave Convolution

![DCGAN with Octave Conv.](imgs/evo.png) 

## References

This repo combines the pytorch implementation of the following paper:

>Goodfellow et al. [Generative Adversarial Nets](https://arxiv.org/abs/1406.2661).

>Radford et al. [Unsupervised Representation Learning with Deep Convolutional Generative Adversarial Networks](https://arxiv.org/abs/1511.06434).

>Mao et al. [Multi-class Generative Adversarial Networks with the L2 Loss Function](https://arxiv.org/abs/1511.06434).

>Arjovsky et al. [Wasserstein Generative Adversarial Networks](https://arxiv.org/abs/1701.07875).

>Chen et al. [Drop an Octave: Reducing Spatial Redundancy in Convolutional Neural Networks with Octave Convolution](https://arxiv.org/abs/1904.05049).


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
