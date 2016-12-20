# Which Ian McKellen are you talking about?

My first image classifier tells which role Ian McKellen is representing on a photo.
I trained the model using Transfer Learning upon Google Inception and train the bottleneck with four categories:

1-Gandalf

![Gandalf](https://github.com/willycornelissen/which_ian_mckellen/blob/master/Gandalf.jpg)

2-Magneto

![Magneto](https://github.com/willycornelissen/which_ian_mckellen/blob/master/Magneto.jpg)

3-Richard III

![Richard III](https://github.com/willycornelissen/which_ian_mckellen/blob/master/Richard%20III.jpg)

4-Himself

![Himself](https://github.com/willycornelissen/which_ian_mckellen/blob/master/Himself.jpg)

## Install

I run the image classifier with Tensorflow Docker Image on Google's Cloud Platform: 

docker run -it -v <hostdir>:<imagedir> gcr.io/tensorflow/tensorflow:latest-devel

## Accuracy


