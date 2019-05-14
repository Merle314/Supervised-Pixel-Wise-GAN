# SPGAN-PyTorch
[Project](https://github.com/Merle314/Supervised-Pixel-Wise-GAN) | [Arxiv](https://github.com/Merle314/Supervised-Pixel-Wise-GAN) | 
[PyTorch](https://github.com/Merle314/Supervised-Pixel-Wise-GAN)

<!-- <img src="images/result.png" width="900px"/> -->
<img src="images/result.png"/>

PyTorch implementation of Supervised Pixel-Wise GAN for Face Super Resolution.

## Prerequisites
* Python 3.5
* PyTorch 0.4

## Datasets
 * VGGFace2
 * CelebA
 * LFW
 * Helen

## Run

Use the default hyparameters except changing the parameter "upscale" according to the expected upscaling factor(2, 3, 4 for 4, 8, 16 upcaling factors, respectively).

>python main.py --ngpu=1 --test --start_epoch=0  --test_iter=1000  --batchSize=64 --test_batchSize=32 --nrow=4  --upscale=3 --input_height=128 --output_height=128 --crop_height=128 --lr=2e-4  --nEpochs=500 --cuda

## Result

Comparison our SPGAN-ID model with state-of-the-art methods on 8x super-resolution 16x16 input face images, and the zoom in details of important face parts to prove the effectiveness of our SPGAN-ID model.

<img src="images/compare.png"/>

## Citation

If you use our codes, please cite the following paper:

## Acknowledgments
Code borrows heavily from [WaveeltSRNet](https://github.com/hhb072/WaveletSRNet).