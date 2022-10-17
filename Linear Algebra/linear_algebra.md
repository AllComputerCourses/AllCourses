# Linear Algebra:

## What is Linear Algebra?
-> Linear Algebra is the branch of Mathematics that deals with linear equations like these:
<img src="http://www.sciweavers.org/tex2img.php?eq=%7B%5Cdisplaystyle%20a_%7B1%7Dx_%7B1%7D%2B%5Ccdots%20%2Ba_%7Bn%7Dx_%7Bn%7D%3Db%7D&bc=Transparent&fc=Black&im=jpg&fs=12&ff=arev&edit=0" align="center" border="0" alt="{\displaystyle a_{1}x_{1}+\cdots +a_{n}x_{n}=b}" width="178" height="18" />
and linear maps like these:
<img src="http://www.sciweavers.org/tex2img.php?eq=%7B%5Cdisplaystyle%20%28x_%7B1%7D%2C%5Cldots%20%2Cx_%7Bn%7D%29%5Cmapsto%20a_%7B1%7Dx_%7B1%7D%2B%5Ccdots%20%2Ba_%7Bn%7Dx_%7Bn%7D%7D&bc=Transparent&fc=Black&im=jpg&fs=12&ff=arev&edit=0" align="center" border="0" alt="{\displaystyle (x_{1},\ldots ,x_{n})\mapsto a_{1}x_{1}+\cdots +a_{n}x_{n}}" width="262" height="18" />


Linear algebra is central to almost all areas of mathematics. For instance, linear algebra is fundamental in modern presentations of geometry, including for defining basic objects such as lines, planes and rotations. Also, functional analysis, a branch of mathematical analysis, may be viewed as the application of linear algebra to spaces of functions.

Linear algebra is also used in most sciences and fields of engineering, because it allows modeling many natural phenomena, and computing efficiently with such models. For nonlinear systems, which cannot be modeled with linear algebra, it is often used for dealing with first-order approximations, using the fact that the differential of a multivariate function at a point is the linear map that best approximates the function near that point.

## Applications:
+ [Datasets or Data Files](https://en.wikipedia.org/wiki/Data_set)
+ [Images](https://www.projectrhea.org/rhea/index.php/Image_(linear_algebra))
+ [Data Preparation](https://www.techtarget.com/searchbusinessanalytics/definition/data-preparation)
+ [Linear Regression](https://www.geeksforgeeks.org/ml-linear-regression)
+ [Regularization](https://towardsdatascience.com/regularization-an-important-concept-in-machine-learning-5891628907ea)
+ [Principal Component Analysis](https://en.wikipedia.org/wiki/Principal_component_analysis)
+ [Latent Semantic Analysis](https://en.wikipedia.org/wiki/Latent_semantic_analysis)
+ [Recommender Systems](https://en.wikipedia.org/wiki/Recommender_system)
+ [Deep Learning](https://www.techtarget.com/searchenterpriseai/definition/deep-learning-deep-neural-network)

In case you need to learn more about these topics, the links are attached to each topic names.

## Vectors:

Vectors can be defined as the ordered list of numbers. Geometrically, we can picture a vector as a directed line segment, whose length is the magnitude of the vector and with an arrow indicating the direction.

### Characteristics:
+ Dimensionality: The number of elements in the vector.
+ Orientation: Whether it is a column vector or a row vector.

### Representation:
In python, we represent a vector using a Numpy array. It goes kind of like this:
```python
import numpy as np
x = np.array([1, 2, 3, 4]) # This is a 4-D row vector
y = np.array([1], [2], [3], [4]) # This is a 4-D column vector
```
We can also represent a vector using a python list:
```python
vector = [1, 2, 3]
```
Orientation of a vector is important or it leads to errors in calculation.

By convention vectors are column oriented but we can transform them to row oriented by performing transpose opearation.

### Vector Arithmetic:
+ Addition: 
    It is just plain old addition. We can add two vectors if and only if they are in same dimensions otherwise it leads to error.
+ Subtraction:
    It follows the same rules as Vector Addition.
+ Multiplication:
  
  1. Dot Product: 
