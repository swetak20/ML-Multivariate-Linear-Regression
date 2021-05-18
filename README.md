# ML-Multivariate-Linear-Regression
Linear Regression is implemented on a dataset to predict the "Chance of admit" based on various factors as mentioned in the .csv file.

Linear Regression is implemented in two difeerent ways:
  1. Using the library - sklearn
  2. From scratch, by obtaining matrices and using the *least square solution* formula.

Later the results are verified by obtaining the prediction for the same test case.

## 1. Using scikit-learn

Using functions of scikit-learn library, the data is used to train the regression and co-effecients are obtained and hence prediction for test case is obtained.

The following functions are used here:
* LinearRegression()
* fit()
* .coef_
* .intercept_

## 2.  Least Square Solution
    
For linear system Ax = b of m equations in n unknowns that are inconsistent, one looks for vectors 
that come as close as possible to being solutions in the sense that they minimize b − Ax
with respect to the 
**Euclidean inner product.**

If A is an m × n matrix with linearly independent column vectors,
then for every m × 1 matrix b, the linear system Ax = b has a unique least squares
solution. This solution is given by 
$$x = inv(((\mathbf{A}^\intercal)A ))\mathbf{A}^\intercal\ b\   $$       



c + $a_{0}$$x_{0}$ + $a_{0}$$x_{0}$ + $a_{0}$$x_{0}$ +.....+ $a_{0}$$x_{0}$ = b

where :
* c = constant
* $x_{0}$ ,$x_{1}$ ,$x_{2}$,....,$x_{n}$ are the independent variables
* b is the dependent variable

To convert the equation to the form Ax = b:
   1. Matrix A contains all the columns of dependent variable and an additional column of with value 1( to obtain the constant c), here columns are: 'const', 'GRE Score', 'TOEFL Score', 'University Rating', 'SOP', 'LOR', 'CGPA', 'Research'
   2. Matrix b contains the values of dependent variables, here the column is : Chance_of_admit
   3. Once the above matrices are obtained, we plug them in the formula of *least square solution* to get the matrix *x* and hence obtain the co-effecients.
   4. Once *x* is obtained,  *b* is calculated for a test case by matrix multiplication of A and *x*

   
