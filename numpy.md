---
title: Numpy
category: Numpy
layout: 2017/sheet
tags: [Featured]
updated: 2021-06-29
intro: | 
        The NumPy library is the core library for scientific computing in Python. 
        It provides a high-performance multidimensional array object, and tools for working with these arrays.
---


### NumPy Arrays

![](https://img-1253324855.cos.ap-chengdu.myqcloud.com/picgo/numpy.png)

### Creating Arrays

    a = np.array([1,2,3])

    b = np.array([(1.5,2,3), (4,5,6)], dtype = float)

    c = np.array([[(1.5,2,3), (4,5,6)], [(3,2,1), (4,5,6)]], dtype = float)

#### Initial Placeholders

{: .-prime}

| Shortcut                                                          | Description                      |
| ---                                                               | ---                              |
| np.zeros((3,4))                                                   | Create an array of zeros         |
| np.ones((2,3,4),dtype=np.int16)                                   | Create an array of ones          |
| d = np.arange(10,25,5)                                            | Create an array of evenly spaced values (step value)|

{: .-shortcuts}

np.linspace(0,2,9) *#Create an array of evenly spaced values (number of samples)*

e = np.full((2,2),7) *#Create a constant array*

    f = np.eye(2) #Create a 2X2 identity matrix 

    np.random.random((2,2)) #Create an array with random values

    np.empty((3,2)) #Create an empty array
