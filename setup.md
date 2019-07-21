# Setup

## Mac

```bash
$ git clone https://github.com/cysmith/neural-style-tf.git && cd neural-style-tf
$ curl http://www.vlfeat.org/matconvnet/models/imagenet-vgg-verydeep-19.mat -o imagenet-vgg-verydeep-19.mat
$ python3 -m venv venv
$ source venv/bin/activate
$ pip install -r requirements.txt
```

# AWS

I was able to run this on the [Deep Learning AMI (Ubuntu)](https://aws.amazon.com/marketplace/pp/B077GCH38C) from Amazon.

```bash
$ ssh ubuntu@<ec2-address>.compute-1.amazonaws.com
$ git clone https://github.com/domtriola/neural-style-tf.git && cd neural-style-tf
$ curl http://www.vlfeat.org/matconvnet/models/imagenet-vgg-verydeep-19.mat -o imagenet-vgg-verydeep-19.mat
$ python -m venv venv # Python version 3.6.5
$ source venv/bin/activate
$ pip install -r requirements-gpu.txt
```
