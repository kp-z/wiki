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

![Arrays](https://img-1253324855.cos.ap-chengdu.myqcloud.com/picgo/numpy.png)

### Creating Arrays

```python
a = np.array([1,2,3])
b = np.array([(1.5,2,3), (4,5,6)], dtype = float)
c = np.array([[(1.5,2,3), (4,5,6)], [(3,2,1), (4,5,6)]], dtype = float)
```

#### Initial Placeholders

```python
np.zeros((3,4)) #Create an array of zeros
np.zeros_like(a) #Create an array of zeros which have the same shape as a
np.ones((2,3,4),dtype=np.int16) # Create an array of ones
d = np.arange(10,25,5) # Create an array of evenly spaced values (step value)
np.linspace(0,2,9) # Create an array of evenly spaced values (number of samples)
e = np.full((2,2),7) # Create a constant array
f = np.eye(2) # Create a 2X2 identity matrix  
np.random.random((2,2)) # Create an array with random values
np.empty((3,2)) # Create an empty array
```

### I/O

#### Saving & Loading On Disk

```py
 np.save('my_array', a)
 np.savez('array.npz', a, b)
 np.load('my_array.npy')
```

#### Saving & Loading Text Files

```py
 np.loadtxt("myfile.txt")
 np.genfromtxt("my_file.csv", delimiter=',')
 np.savetxt("myarray.txt", a, delimiter=" ")
```

### Data Type

```python
np.int64 # Signed 64-bit integer types
np.float32 # Standard double-precision floating point
np.complex # Complex numbers represented by 128 floats
np.bool # Boolean type storing TRUE and FALSE values
np.object # Python object type
np.string_ # Fixed-length string type
np.unicode_ # Fixed-length unicode type
```

### Inspecting Your Array

```python
 a.shape # Array dimensions
 len(a) # Length of array
 b.ndim # Number of array dimensions 
 e.size # Number of array elements
 b.dtype # Data type of array elements
 b.dtype.name # Name of data type
 b.astype(int) # Convert an array to a different type
```

### Asking For Help

```python
np.info(np.ndarray.dtype)
```

### Array Mathematics

```py
>>> g = a - b 
    array([[-0.5, 0. , 0. ],[-3. , -3. , -3. ]]) 
>>> np.subtract(a,b)
>>> b + a
    array([[ 2.5, 4. , 6. ],[ 5. , 7. , 9. ]]) 
>>> np.add(b,a)
>>> a / b
    array([[ 0.66666667, 1., 1. ], [0.25 , 0.4 , 0.5 ]])
>>> a * b
    array([[ 1.5, 4. , 9. ],[ 4. , 10. , 18. ]]) 
>>> np.multiply(a,b)
>>> np.divide(a,b)
>>> np.exp(b)
>>> np.sqrt(b)
>>> np.sin(a)
>>> np.cos(b)
>>> np.log(a) # Element-wise natural logarithm
>>> e.dot(f) # Dot product
    array([[ 7., 7.], [ 7., 7.]])
```

### Comparison

![](https://img-1253324855.cos.ap-chengdu.myqcloud.com/picgo/numpy2.png)

## Refercence
{: .-two-column}

 * [DataCamp NumPy](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Numpy_Python_Cheat_Sheet.pdf)
 * [A Little Bit of Everything](https://blog.finxter.com/wp-content/uploads/2019/10/grafik-2-768x592.png)
{: .-also-see}

