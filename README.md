# Final assigment for my AI Trainning

## Hey there! This is my first Deep Learning cloud prediction ☁

I used a Unet architecture that is commonly used for image segmentation tasks. The model was trained on a dataset of Sentinel-2 images for the specific task of cloud detection. 
Check the encoder and weights details here 👇🏾

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

So the final result looks like this 🥳:
<h1 align="center">
  <br>
  <a href="https://github.com/valeriallactayo/my_dl"><img src="https://github.com/valeriallactayo/my_dl/blob/master/final_result.png" alt="Markdownify" width="700"></a>
</h1>

Not bad, right? Here I could apply and finally understand many Deep Learning concepts like epoch, padding, batch, forward, learning rate and many more.

You can check my python script <a href="https://github.com/valeriallactayo/my_dl/blob/master/dlmodel.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab" title="Open and Execute in Google Colaboratory"></a>
</h1>

Also you can find in this repository the Sentinel2 image (512x512) and the trained model (model.pt) so you can replicate and improve your DL Skills 🙌🏽. 

    
