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

![Proper](https://github.com/willycornelissen/which_ian_mckellen/blob/master/Proper.jpg)

## Install

I run the image classifier with Tensorflow Docker Image on Google's Cloud Platform: 

docker run -it -v <hostdir>:<imagedir> gcr.io/tensorflow/tensorflow:latest-devel

## Accuracy

python classify.py Gandalf.jpg

| Category      | Score         |
| ------------- | ------------- |
| Gandalf       | 94%           |
| Magneto       | 0.04%         |
| Richard III   | 0.01%         |
| Himself       | 0.01%         |

python classify.py Magneto.jpg

| Category      | Score         |
| ------------- | ------------- |
| Gandalf       | 0.03%         |
| Magneto       | 93%           |
| Richard III   | 0.01%         |
| Himself       | 0.03%         |

python classify.py Richard III.jpg

| Category      | Score         |
| ------------- | ------------- |
| Gandalf       | 0.04%         |
| Magneto       | 0.01%         |
| Richard III   | 88%           |
| Himself       | 0.07%         |

python classify.py Proper.jpg

| Category      | Score         |
| ------------- | ------------- |
| Gandalf       | 0.03%         |
| Magneto       | 17%           |
| Richard III   | 0.04%         |
| Himself       | 76%           |
