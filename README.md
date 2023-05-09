# Final assigment for my AI Trainning

## Hey there! This is my first Deep Learning cloud prediction ☁

I used a Unet architecture that have been trained to detect clouds in Sentinel-2 images with 13 bands. 
Check the encoder and weights details below:

``` python
model = smp.Unet(
    encoder_name="mobilenet_v2",
    encoder_weights="imagenet",
    in_channels=13,
    classes=4
)
```

Then, I trained that model using [CLOUDSEN12 dataset](https://cloudsen12.github.io/) so that Unet will be trained with four (4) clases:

- Thin cloud 
- Thick cloud 
- Shadow
- Clear

So the final result was this 🥳:


Here i could apply and finally understand many deep learning concepts like ""
