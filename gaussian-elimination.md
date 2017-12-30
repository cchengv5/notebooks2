The purpose of this article is to describe how the solutions to a linear system are actually found. The fundamental idea is to add multiples of one equation to the others in &lt;font color=''\#4590a3"&gt;**`order to eliminate a variable and to continue this process until only one variable is left`**. &lt;/font&gt;Once this final variable is determined, its value is substituted back into the other equations in order to evaluate the remaining unknowns. This method, characterized by step‐by‐step elimination of the variables, is called**Gaussian elimination**.

**Example 1**: Solve this system:

![](https://www.cliffsnotes.com/assets/20061.gif)

  


Multiplying the first equation by −3 and adding the result to the second equation eliminates the variable_x_:

![](https://www.cliffsnotes.com/assets/20062.gif)

  


This final equation, −5_y_= −5, immediately implies_y_= 1. Back‐substitution of_y_= 1 into the original first equation,_x + y_= 3, yields_x_= 2. \(Back‐substitution of_y_= 1 into the original second equation, 3_x_− 2_y_= 4, would also yeild_x_= 2.\) The solution of this system is therefore \(_x, y_\) = \(2, 1\), as noted in Example 1.

Gaussian elimination is usually carried out using matrices. This method reduces the effort in finding the solutions by eliminating the need to explicitly write the variables at each step. The previous example will be redone using matrices.

**Example 2**: Solve this system:

![](https://www.cliffsnotes.com/assets/20063.gif)

  


The first step is to write the coefficients of the unknowns in a matrix:

![](https://www.cliffsnotes.com/assets/20064.gif)

This is called the**coefficient matrix**of the system. Next, the coefficient matrix is augmented by writing the constants that appear on the right‐hand sides of the equations as an additional column: 

![](https://www.cliffsnotes.com/assets/20065.gif)

  


This is called the**augmented matrix**, and each row corresponds to an equation in the given system. The first row,**r**1= \(1, 1, 3\), corresponds to the first equation, 1_x_+ 1_y_= 3, and the second row,**r**2= \(3, −2, 4\), corresponds to the second equation, 3_x_− 2_y_= 4. You may choose to include a vertical line—as shown above—to separate the coefficients of the unknowns from the extra column representing the constants.

Now, the counterpart of eliminating a variable from an equation in the system is changing one of the entries in the coefficient matrix to zero. Likewise, the counterpart of adding a multiple of one equation to another is adding a multiple of one row to another row. Adding −3 times the first row of the augmented matrix to the second row yields

![](https://www.cliffsnotes.com/assets/20066.gif)

  


The new second row translates into −5_y_= −5, which means_y_= 1. Back‐substitution into the first row \(that is, into the equation that represents the first row\) yields_x_= 2 and, therefore, the solution to the system: \(_x, y_\) = \(2, 1\).

Gaussian elimination can be summarized as follows. Given a linear system expressed in matrix form,_A_**x = b**, first write down the corresponding augmented matrix:

![](https://www.cliffsnotes.com/assets/20067.gif)

  


Then, perform a sequence of**elementary row operations**, which are any of the following:

Type 1. Interchange any two rows.

Type 2. Multiply a row by a nonzero constant.

Type 3. Add a multiple of one row to another row.

The goal of these operations is to transform—or**reduce**—the original augmented matrix into one of the form![](https://www.cliffsnotes.com/assets/20068.gif)where_A_′ is upper triangular \(_aij_′ = 0 for_i &gt; j_\), any zero rows appear at the bottom of the matrix, and the first nonzero entry in any row is to the right of the first nonzero entry in any higher row; such a matrix is said to be in**echelon**form. The solutions of the system represented by the simpler augmented matrix, \[_A_′ \|**b**′\], can be found by inspectoin of the bottom rows and back‐substitution into the higher rows. Since elementary row operations do not change the solutions of the system, the vectors**x**which satisfy the simpler system_A_′**x**=**b**′ are precisely those that satisfy the original system,_A_**x**=**b**.

**Example 3**: Solve the following system using Gaussian elimination:

![](https://www.cliffsnotes.com/assets/20069.gif)

  


The augmented matrix which represents this system is

![](https://www.cliffsnotes.com/assets/20070.gif)

  


_The first goal is to produce zeros below the first entry in the first column_, which translates into eliminating the first variable,_x_, from the second and third equations. The row operations which accomplish this are as follows:

![](https://www.cliffsnotes.com/assets/20071.gif)

  


The second goal is to produce a zero below the second entry in the second column, which translates into eliminating the second variable,_y_, from the third equation. One way to accomplish this would be to add −1/5 times the second row to the third row. However, to avoid fractions, there is another option: first interchange rows two and three. Interchanging two rows merely interchanges the equations, which clearly will not alter the solution of the system:

![](https://www.cliffsnotes.com/assets/20072.gif)

  


Now, add −5 times the second row to the third row:

![](https://www.cliffsnotes.com/assets/20073.gif)

  


Since the coefficient matrix has been transformed into echelon form, the “forward” part of Gaussian elimination is complete. What remains now is to use the third row to evaluate the third unknown, then to back‐substitute into the second row to evaluate the second unknown, and, finally, to back‐substitute into the first row to evaluate the first unknwon.

The third row of the final matrix translates into 10_z_= 10, which gives_z_= 1. Back‐substitution of this value into the second row, which represents the equation_y_− 3_z_= −1, yields_y_= 2. Back‐substitution of both these values into the first row, which represents the equation_x_− 2_y + z_= 0, gives_x_= 3. The solution of this system is therefore \(_x, y, z_\) = \(3, 2, 1\).

**Example 4**: Solve the following system using Gaussian elimination:

![](https://www.cliffsnotes.com/assets/20074.gif)

  


For this system, the augmented matrix \(vertical line omitted\) is

![](https://www.cliffsnotes.com/assets/20075.gif)

  


First, multiply row 1 by 1/2:

![](https://www.cliffsnotes.com/assets/20076.gif)

  


Now, adding −1 times the first row to the second row yields zeros below the first entry in the first column:

![](https://www.cliffsnotes.com/assets/20077.gif)

  


Interchanging the second and third rows then gives the desired upper‐triangular coefficient matrix: 

![](https://www.cliffsnotes.com/assets/20078.gif)

  


The third row now says_z_= 4. Back‐substituting this value into the second row gives_y_= 1, and back‐substitution of both these values into the first row yields_x_= −2. The solution of this system is therefore \(_x, y, z_\) = \(−2, 1, 4\).

