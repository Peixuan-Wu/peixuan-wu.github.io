# Swift and brutal intro to Linear Algebra
## Graphics's Dependencies
### Basic mathmatics 
Linear algebra, calculus, statistics

### Basic physics
Optics, Mechanics

### Misc
Signal processing
Numerical analysis

### And a bit of aesthetics


## Vectors
1.Direction and length  

2.$\vec{AB}$ = B - A （表示从A到B的一个向量)
向量常用  

3.usually written as $\alpha$ or in bold **a**

4.No absolute starting position

5.Magnitude (length) of a vector written as ||$\vec{a}$||

6.unit vector  
$\hat{a}$ = $\vec{a}$/||$\vec{a}$||  
used to represent direction

### Vector Addition
1.Geometrically: Parallelogram law & Trianagle law

2.Algebraically: Simply add coordinates

### Cartesian Coordinates

X and Y can be any(orthogonal unit) vectors
A = 4x + 3y
A = $\begin{pmatrix} x \\ y \end{pmatrix}$
方便计算长度

### Vector Multiplication
#### Dot(scalar) Product

$\vec{a}$ $\cdot$ $\vec{b}$ = ||$\vec{a}$|| ||$\vec{b}$|| $\cdot$ $\cos\theta$

##### Dot product in Cartesian Coordinates
$\vec{a}$ $\cdot$ $\vec{b}$ =  $\begin{pmatrix} Xa \\ Ya \end{pmatrix}$ $\cdot$ $\begin{pmatrix} Xb \\ Yb \end{pmatrix}$ = XaXb + YaYb

##### Dot product for Projection
投影必须是沿着 $\vec{a}$的方向  
因此可以表示为  
$\vec{b_perpendicular}$ = k $\hat{a}$ = ||$\vec{b_perpendicular}$|| = ||$\vec{b}$|| $\cos\theta$

##### Dot product in Graphics
1.Measure how close two directions are  
2.Decompose a vector  
3.Determine forward/backward  > or < 0  

#### Cross product: Properties
**a** $\times$ **b** = - **b** $\times$ **a**  

|**a** $\times$ **b**| = |**a**||**b**| $\sin\theta$  根据右手定则确定方向
Self-Cross product = 0 向量

1. Cross product is orthogonal to two initial vectors  
2. Direction determined by right-hand rule  
3. Useful in constructing coordinate systems 

##### Cross Product in Graphics
1.Determine left/ right 
2.Determine inside/outside p点在不在三角形内部


## Matrices
### Matrix-Matrix Multiplicatin 
(M $\times$ N)( N $\times$ M) = (M $\times$ N) 矩阵乘法 满足条件
结果用坐标去点乘

#### Properties
> Non-commutative
 
(AB and BA are different in general)  
这个地方思索了一番，为什么不满足交换律？ 具有一定的实际意义  


> Accociative and distributive

A(BC) = (AB)C  
A(B+C) = AB+AC  

### Matrix-Vector Multiplication
1.treat vectot as a column matrix (M $\times$ 1)  
$\begin{pmatrix} -1&0 \\ 0&1 \end{pmatrix}$ $\begin{pmatrix} x \\ y \end{pmatrix}$ = $\begin{pmatrix} -x \\ y \end{pmatrix}$

### Transpose of a Matrix
1.Switch rows and colums  
**Property**  
(AB)^T^ = B^T^A^T^

### Identity Matrix and Inverses
I_3_$\times$_3_ = $\begin{pmatrix} 1&0&0 \\ 0&1&0 \\ 0&0&1 \end{pmatrix}$  
这就是单位矩阵  

AA^-1^ = A^-1^A = I  
(AB)^-1^ = B^-1^A^-1^

## Vector multi in Matrix form
### Dot product?
$\vec{a}$$\cdot$$\vec{b}$ = $\vec{a}$^T^$\vec{b}$  
一行乘一列 = 数

### Cross  product?
$\vec{a}$$\cdot$$\vec{b}$ = A^*^b = $\begin{pmatrix} 0&-Za&Ya \\ Za&0&-Xa \\ -Ya&Xa&0 \end{pmatrix}$ $\begin{pmatrix} Xa \\ Yb \\ Zb \end{pmatrix}$ 

