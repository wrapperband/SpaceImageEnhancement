# Space Image Enhancement

### Using Star Enhancement techniques on Planet Images

#### Introduction

Image of Apollo 12 astronaut on the "Moon", combination of 37 images from low resolution video, cropped to a wide angle format.

Note the flat nature of the landscape, the square format of ground features. Multiple track ways, from tracked digger. A thin wheeled cart track is seen quickly disappearing to the horizon.

Further work : enhance size further and process colour information.

#### Original Image - Apollo 12 Moon from Lander Video Camera

![37 Image scaked 800% Enlargement](https://github.com/wrapperband/SpaceImageEnhancement/blob/master/MoonImages/apollo12-1-original.jpg)


#### Enlarged Image : Download needed for full resolution.  - Apollo 12 Moon from Lander Video Camera

![37 Image scaked 800% Enlargement](https://github.com/wrapperband/SpaceImageEnhancement/blob/master/MoonImages/apollo12-2c_stacked.png)


#### Method

Extract video frames between 2 timepoints using Avidemux.

Clean up frames, remove worst or blurred, remove images with foreground movement.

For the image  Apollo12-2c  - The astronaut is blurred because the image is registered to the background.

 - Apollo 12 Moon from Lander Video Camera
 
 
 From Imagemagic   mogrify is used to increase the size of all the images.
 
 ~/Pictures/apollo12-2b$  mogrify -resize 400% *.jpg
 
 Siril is then used to convert to *.FIT  FITS format, register the images and combine the images, in this case by addition.
 

 
### References 
 
#### Siril   
 
    http://free-astro.org/index.php/Siril
 
#### Siril Download :  
 
    git clone https://gitlab.com/free-astro/siril.git  
 
#### Image Magic
 
    https://www.imagemagick.org/script/index.php   
