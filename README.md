# Fine-Tuning
Fine tuning of parameters to generate 128x128x3 images using 1000 images and trained on 1500 epochs.
DCGAN model with dropout of 0.5 and one sided labelling in Discriminator output images with the best visual quality among all the combination experimented.

Ipynb is not uploaded as the file size is too big (> 100mb). Access Google Colab notebook for fine-tuning code via https://colab.research.google.com/drive/1r_aX_4mT3YeyUKi7lRP7Hpc61sVNvOJx?usp=sharing

## Table on a list of configuration changes experimented
![configuration changes table](https://github.com/mingxiuuuuu/Fine-Tuning/blob/master/Configuration%20changes%20experimented.PNG)

## Expanded DCGAN faced convergence failure as Discrimnator can easily discriminate real and fake images with the bigger image. Adding dropout of 0.5 prevented convergence failure while SGD optimiser in Discrimnator, one-side labelling in Discriminator and LeakyReLU optimiser function in Generator do not.
![dropout 0.5](https://github.com/mingxiuuuuu/Fine-Tuning/blob/master/dropout%200.5.png)

## Results after respective configuration changes
![respective configuration changes](https://github.com/mingxiuuuuu/Fine-Tuning/blob/master/images%20generated%20after%20respective%20configuration%20changes.png)

![respective configuration changes](https://github.com/mingxiuuuuu/Fine-Tuning/blob/master/images%20generated%20after%20respective%20configuration%20changes_2.png)
