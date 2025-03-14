# Synthetic ID Card Image Generation for Improving Presentation Attack Detection - Complementary material.
Daniel Benalcazar, Juan E. Tapia, Sebastian Gonzalez, and Christoph Busch,

This work explores three methods for synthetically generating ID card images to increase the amount of data while training fraud-detection networks. These methods include computer vision algorithms and Generative Adversarial Networks. Our results indicate that databases can be supplemented with synthetic images without any loss in performance for the print/scan Presentation Attack Instrument Species (PAIS) and a loss in
performance of 1% for the screen capture PAIS.

# Template
A traditional image processing algorithm is developed, capable of generating fake ID card images from a clear template that resembles the original bona fide and presentation attack scenarios ID Cards from different country template can be generate as describe in our paper. The templates are not provided. A subset of images generated has been shared.

<p align="center" width="100%">
    <img width="33%" src="https://user-images.githubusercontent.com/45126159/216764780-74f28fca-45d8-4881-ad63-7a1b483435df.gif">
</p>


Downloading sample images [here](https://www.dropbox.com/s/4lrxxe5ub4952li/templates-IDcard_v2.zip?dl=0).


# Transfer Texture
A traditional image processing algorithm capable of generating ID card images faster than GAN-based methods is proposed. This algorithm transfers the
noise textures from presentation attack species images to bona fide images. These noise texture templates are available.

10,000 isolated textures are availble for craeting your own images, where any texture can be added to any bona fide image to generate the tampering effect artificially. This process consists of cropping the isolated texture with the image size of the bona fide image, and then applying a pixel-whise mathematical addition between the texture and the bona fide image, as illustrated:

![texture_addition](https://user-images.githubusercontent.com/45126159/216760716-72550814-75d5-4982-be6d-79f336bb8099.png)
Process of device-noise texture addition. A random isolated texture is selected from the set of 5,000 available textures per PAI. The texture is cropped
with the shape of the input image at a random location. The output textured ID card is the pixel-wise addition between the input ID card and the cropped
texture. In this figure, an ID card generated by the Templates method is used (no real data), thus it is not blacked out.

Downloading textures [here](https://www.dropbox.com/scl/fo/6ilul6b9lvn97xyx7s383/AN5Ym1VYSY-P-ZVNRFTEfUw?rlkey=3c5bnw9y5zqbivx8urvw04nr9&st=7c5ffonq&dl=0).
The code to apply the textures to any image is available [here](https://github.com/dpbenalcazar/textures).

# Synthetic images
![alt text](./StyleGAN2.png?raw=true)

Downloading all the images generated by StyleGAN [here](https://www.dropbox.com/s/mwhly4oborsu2un/StyleGAN2-synt-IDcardv2.zip?dl=0).

# Citation:
```
@ARTICLE{10065533,
  author={Benalcazar, Daniel and Tapia, Juan E. and Gonzalez, Sebastian and Busch, Christoph},
  journal={IEEE Transactions on Information Forensics and Security}, 
  title={Synthetic ID Card Image Generation for Improving Presentation Attack Detection}, 
  year={2023},
  volume={},
  number={},
  pages={1-1},
  doi={10.1109/TIFS.2023.3255585}}

```

# License
This work and the methods proposed are only for research purposes and the images are be generated by chance. Any implementation or commercial use modification must be analysed separately for each case to the email: juan.tapia-farias@h-da.de.
<p>
**Password requirement access will be given only for Senior researchers, and Profesors using an academic email**
