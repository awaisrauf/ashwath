---
layout: post
title: Tensorflow Installation Guide 
date: 2018-04-12 
description: This tutorial will guide you to install tensorflow on windows computer. Installation will be as easy as 1,2,3. Click to see details.
tags: [tensorflow, installation, easy way to install tensorflow]
page_number: 1
categories: basics
author: Awais
---

# Tensorflow Installation Guide
Tensorflow is a famous deep learning library in python developed by Google. In this tutorial, you will learn to install tensorflow on a windows pc, step by step. 

### Step 1: Install Anaconda 
*  Anaconda is a distribution of python which simplifies its package management therefore we choose to install it for python.

* To install anaconda, go to <a href="https://www.anaconda.com/download/#windows" target="_blank">anaconda website</a> and download 64 bit or 32 bit file according to your system specifications. 

* Double  click on the file and click next until you find following screen where you should select both options,

<img src="https://raw.githubusercontent.com/awaisrauf/ashwath/master/_posts/images/1_fig1.PNG" alt="Select both options." style="width: 550px;"/>

If you select both options in this screen, anaconda will be automatically added to your PATH environment.

### Step 2: Create New Anaconda Environment 
* Open command prompt and type following command to create a new environment. 

```console
C:> conda create -n tensorflow 
```
A line will appear asking you whether to proceed? Type y and click enter.
```console
C:> Proceed ([y]/n)?  
```

### Step 3: Activate Conda Environment 
* Activate tensorflow environment by issuing following commands,

```console
C:> activate tensorflow
(tensorflow)C:>  
```

Notice tensorflow before C:>? This shows that tensorflow environment is now on.

### Step 4: Install Tensorflow
Write following command to install tensorflow,

```console
(tensorflow)C:>  conda install -c conda-forge tensorflow 
```

Following screen will appear, type y and enter and tensorflow will be installed.

<img src="https://raw.githubusercontent.com/awaisrauf/ashwath/master/_posts/images/1_fig2.PNG" alt="command prompt when you install tensorflow." style="width: 550px;"/>

### Step 5: Confirm Installation 
Invoke python in the same prompt by writing following command in the same command prompt,

```console
(tensorflow)C:> python 
```

and write following tensorflow code to test tensorflow installation.

```console
>>> import tensorflow as tf
hello = tf.constant('Hello, TensorFlow101!')
sess = tf.Session()
print(sess.run(hello)) 
```

If you get ''Hello, TensorFlow101!' as output, you have successfully installed tensorflow. Congratulations! Share your successful installation in comments below. 

If you came across problems, comment below and we will help you as soon as possible.
