---
title: Numpy
category: Numpy
layout: 2017/sheet
tags: [Featured]
updated: 2021-06-29
intro: | 
        The NumPy library is the core library for scientific computing in Python. It provides a high-performance multidimensional array object, and tools for working with these arrays.
---


### NumPy Arrays

    ![](https://img-1253324855.cos.ap-chengdu.myqcloud.com/picgo/numpy.png)

### Creating Arrays

    >>> a = np.array([1,2,3])
    >>> b = np.array([(1.5,2,3), (4,5,6)], dtype = float)
    >>> c = np.array([[(1.5,2,3), (4,5,6)], [(3,2,1), (4,5,6)]], dtype = float)

#### Initial Placeholders

    >>> np.zeros((3,4)) # Create an array of zeros
    >>> np.ones((2,3,4),dtype=np.int16) >>> d = np.arange(10,25,5) # Create an array of ones
    >>> np.linspace(0,2,9) # Create an array of evenly spaced values (step value)
    >>> e = np.full((2,2),7) # Create an array of evenly spaced values (number of samples) Create a constant array
    >>> f = np.eye(2) # Create a 2X2 identity matrix 
    >>> np.random.random((2,2)) # Create an array with random values
    >>> np.empty((3,2)) # Create an empty array

### Reading

```py
    file = open("hello.txt", "r") # open in read mode 'r'
    file.close() 

    print(file.read())  # read the file 
    print fh.readline() # Reading line by line
```

### Writing (overwrite)

```py
    file = open("hello.txt", "w") # open in write mode 'w'
    write("Hello World")

    text_lines = ["First line", "Second line", "Last line"] 
    file.writelines(text_lines)

    file.close()
```

### Writing (append)

```py
    file = open("Hello.txt", "a") # open in append mode
    write("Hello World again")  
    file.close()
```

### Context manager

```py
    with open("welcome.txt", "r") as file:
        # 'file' refers directly to the "welcome.txt"
    data = file.read()
```

It closes the file automatically, no need for `file.close()`.
