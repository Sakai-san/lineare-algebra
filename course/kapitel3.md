#Kapital 3 : Matrix und Eliminationsverfahren

## Matrix

Eine Matrix ist eine Tablelle mit m Zeilen and n Spalten.

It contains the coefficients of a linear system. These are the so-called elements of the matrix.

Example I shows how a linear system is turned into a matricial equation in the form Ax⃗ =y⃗

.
Example I

⎧⎩⎨⎪⎪−x−3y+zx+y−3z3x+4y+2z===10−12−5⟺⎛⎝⎜−113−3141−32⎞⎠⎟A⎛⎝⎜xyz⎞⎠⎟x⃗ =⎛⎝⎜10−12−5⎞⎠⎟y⃗


Index notation is used to specify a matrix element ai,j
, with i the row and j the column. For example, the element a3,2 equals to 4 in the A

matrix of example I.
Matrix elimination

The matrix elimination, also called Gaussian elimination, is a method to solve a linear system. This is in fact the addition method applied on matrices.

The starting point for a matrix elimination is the augmented matrix, as example II shows. The variable elimination is performed by adding two rows together. One of the two rows is then replaced by the result of the addition.
Example II

⎛⎝⎜⎜−113−3141−3210−12−5⎞⎠⎟⎟⟺R1+R2→R2⎛⎝⎜⎜−103−3−241−2210−2−5⎞⎠⎟⎟⟺3R1+R3→R3⎛⎝⎜⎜−100−3−2−51−2510−225⎞⎠⎟⎟

⟺−12R2→R2⎛⎝⎜⎜−100−31−511510125⎞⎠⎟⎟⟺5R2+R3→R3⎛⎝⎜⎜−100−310111010130⎞⎠⎟⎟


Once we get the matrix in echelon form we can solve back the system by going from the bottom up, as follows :

10z=30⟺
z=3

Let’s replace z

in the second row :

y+1⋅3z=1⟺
y=−2

Let’s replace y
and z

in the first row :

−1x+−3⋅−2y+1⋅3z=10⟺−x+9=10⟺
x=−1

The solution is :
single point intersection

Figure 3.1 : single point of intersection (credits montereyinstitute)

x⃗ =⎛⎝⎜−1−23⎞⎠⎟(1)

Example III

⎧⎩⎨⎪⎪4x+y+3z2x+y+z−x−y===120⟺⎛⎝⎜⎜42−111−1310120⎞⎠⎟⎟⟺R1↔R3⎛⎝⎜⎜−124−111013021⎞⎠⎟⎟

⟺2R1+R2→R2⎛⎝⎜⎜−104−1−11013021⎞⎠⎟⎟⟺4R1+R3→R3⎛⎝⎜⎜−100−1−1−3013021⎞⎠⎟⎟⟺−3R2+R3→R3⎛⎝⎜⎜−100−1−1001002−5⎞⎠⎟⎟

From the last row of the echelon matrix we have :

0x+0y+0z=5

That equation is unsolvable, the system then has no solution :
x⃗ ={}(2)


Example IV

{2x+−2yx+−y==21⟺(21−2−121)⟺R1↔R2(12−1−212)⟺−2R1+R2→R2(10−1010)


From the last row of the echelon matrix we have :

0x+0y=0⟺0=0

That equation does not provide any information about the variables.

Let’s move on to the upper row from which we get :

1x+−1y=1⟺x=1+y
. Let y=β

.

In that case we have one equation for two variables. Then the system has infinitely many solutions and the general solution is :
x⃗ =(1+ββ),β∈R(3)


Recapitulation

Transforming linear system into a matricial equation separates the coefficients from the variables. This make things more readable.

Solving a matricial equation is done by performing operations on the augmented matrix rows, such as interchanging rows and multiplying a row by a factor (different than 0

). These operations combined with adding two rows together repeatedly, eventually lead to a matrix in echelon form (like a staircase).

From the echelon matrix, we solve rows by substituing back the values found from the bottom up. Rows of all zeroes do not provide any information about the variables and can thus be ignored.