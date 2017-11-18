#Kapitel 4 : Operationen auf matrix

Die grösse einer Matrix, m×n  bezeichnet, ist der Anzahl von Reihen, bzw. von Spalten der Matrix. Eine Matrix, deren Anzahl der Reihen gleich der Anzahll der Spalten, d.H. m=n gilt, ist, wird die Matrix quadratische Matrix genannt.


Multiplikation

Wie haben im vorherigen Kapitel gesehen, wie sich in Matrixschreibweise die Koeffizienten von den Variablen miteinander getrennt lassen und damit zu einer multiplikation einer Matrix durch einen Vektor führt. Dazu gehört, dass diese multiplikation definiert werden muss.

Seien A eine m×n Matrix and B eine m′×n′ matrix.

AB=C
is possible only if n=m′. The C matrix size is m×n′

.

The multiplication A
by B is done by distributing A rows on each columns of B and by adding the products, namely (ci,j)=∑nk=0ai,kbk,j

.
Example I
⎛⎝⎜4−168−20⎞⎠⎟(0−71−1)=⎛⎝⎜4⋅0+8⋅−7−1⋅0+−2⋅−76⋅0+0⋅−74⋅1+8⋅−1−1⋅1+−2⋅−16⋅1+0⋅−1⎞⎠⎟=⎛⎝⎜−56140−416⎞⎠⎟(1)
Addition

The addition of two matrices is possible only if they both have the same size. The corresponding elements are added. The subtraction is defined in a similar way.
Example II
(91212−38)+(70−10−1−60)=(161−811−98)(2)
Mutiplication by a scalar (number)

All elements of the matrix are multiplied by the scalar.
Example III
−2⎛⎝⎜−11−702−4−1⎞⎠⎟=⎛⎝⎜−2⋅−11−2⋅−7−2⋅0−2⋅2−2⋅−4−2⋅−1⎞⎠⎟=⎛⎝⎜22140−482⎞⎠⎟(3)
Decomposition

A matrix multiplying a column matrix can be decomposed into an addition of multiplications. This is due to the previous rules.
Example IV
⎛⎝⎜234−52−1⎞⎠⎟(λ1λ2)=⎛⎝⎜2λ1+−5λ23λ1+2λ24λ1+−1λ2⎞⎠⎟=λ1⎛⎝⎜234⎞⎠⎟+λ2⎛⎝⎜−52−1⎞⎠⎟(4)
Recapitulation

Multiplication

    AB=C

where A a matrix of size m×n and B a matrix of size m′×n′. The multiplication is possible only if n=m′. Matrix C size is m×n′
.
AB≠AB
Let K=T
, the left multiplication by P gives PK=PT
Let K=T
, the right multiplication by P gives KP=TP

Addition

    A+B=(ai,j+bi,j)

Multiplication by a scalar

    λA=(λai,j)

Distribution

    A(B+C)=AB+AC

Decomposition matrix multiplying a column matrix

    (v1⋮vn⋯⋯⋯w1⋮wn)(λ1⋮λn)=λ1(v1⋮vn)+⋯+λn(w1⋮wn)
