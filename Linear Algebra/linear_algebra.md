# Linear Algebra:

## What is Linear Algebra?
-> Linear Algebra is the branch of Mathematics that deals with linear equations like these:
<img src="https://bit.ly/3ezG7QS" align="center" border="0" alt="a_{1}x_{1}+\cdots +a_{n}x_{n}=b" width="178" height="18" />
and linear maps like these:
<img src="https://bit.ly/3TmQMgc" align="center" border="0" alt="x_{1},\ldots ,x_{n})\mapsto a_{1}x_{1}+\cdots +a_{n}x_{n}" width="256" height="18" />

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
From the above code:

<img src="http://www.sciweavers.org/tex2img.php?eq=x%20%3D%20%20%5Cbegin%7Bbmatrix%7D1%20%26%202%20%26%203%20%26%204%20%5Cend%7Bbmatrix%7D%20&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0" align="center" border="0" alt="x =  \begin{bmatrix}1 & 2 & 3 & 4 \end{bmatrix} " width="136" height="24" />

<img src="https://bit.ly/3TqiiJN" align="center" border="0" alt="y =  \begin{bmatrix}1 \\ 2 \\ 3 \\ 4 \end{bmatrix} " width="71" height="79" />


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
 
        <img src="https://bit.ly/3EN9CsP" align="center" border="0" alt=" \overrightarrow{a} .  \overrightarrow{b}  =  \Sigma  (a_{i} * b_{i} * \Cos( \theta ))" width="228" height="29" />
        
        It is a scalar quantity and has commutative and distributive properties.
        
        Calculating dot product using numpy:
        ```python
        import numpy as np
        a = np.array([20, 30, 40])
        b = np.array([24, 35, 44])
        print(np.dot(a, b))
        ```
        
  2. Cross Product:        
        
        
        It is a vector quantity and can be calculated only if the vector is 3-D or 2-D.
        
        Calculating cross product using numpy:
        
        ```python
        import numpy as np
        a = np.array([20, 30, 40])
        b = np.array([24, 35, 44])
        print(np.dot(a, b))
        ```
        
### Scalar and Vector Projection:
   1. Magnitude of a Vector:
   
        -- It is the distance from tail to the head of the vector.
        
        -- It is indicated using || x ||
        
        -- Formula:
        
   2. Vector Projection:
   
        -- A vector projection of a vector a onto another vector b is the orthogonal projection of a onto b.
        
        -- Formula:
        
   3. Changing the basis of the vector:
   
       Properties:
       
         -- The new basis vectors should be linearly independent of each other.
           
         -- They should span the whole vector space.
            
         -- They aren't necessarily unique.
            
         -- Formula:
            
   4. Spanning Sets:
                 
         The set <insert> is a spanning set for v if and only if every vector in v can be written as a linear combination of <insert>
