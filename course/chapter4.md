#Kapitel 4 : Operationen auf matrix

Die grösse einer Matrix, m×n bezeichnet, ist der Anzahl von Reihen, bzw. von Spalten der Matrix. Eine Matrix, deren Anzahl der Reihen gleich dem Anzahl der Spalten, d.H. m=n gilt, ist, dann wird die Matrix quadratische Matrix genannt.


##Matrizenmultiplikation

Wie haben im vorherigen Kapitel gesehen, wie sich in Matrixschreibweise die Koeffizienten von den Variablen miteinander getrennt lassen und damit zu einer multiplikation einer Matrix durch einen Vektor führt. Jetzt muss also diese multiplikation definiert werden.

Seien A eine m×n Matrix und B eine m′×n′matrix.

AB=C ist möglich nur wenn n=m′ gilt. die Matrix C, also das Produkt, ist eine m×n′ Matrix.


The multiplication A by B is done by distributing A rows on each columns of B and by adding the products, namely (ci,j)=∑nk=0ai,kbk,j

.
###Example I
⎛⎝⎜4−168−20⎞⎠⎟(0−71−1)=⎛⎝⎜4⋅0+8⋅−7−1⋅0+−2⋅−76⋅0+0⋅−74⋅1+8⋅−1−1⋅1+−2⋅−16⋅1+0⋅−1⎞⎠⎟=⎛⎝⎜−56140−416⎞⎠⎟(1)

##Addition

Die Addition zweier Matrizen ist nur möglich, wenn diejenige gleiche gross sind. Die entsprechenden Elementen sind addiert. Das gleich gilt für die Subtraktion.

###Example II
(91212−38)+(70−10−1−60)=(161−811−98)(2)

#Skalarmultiplikation (multiplikation mit einem Zahl)

Alle Elemente werden durch den Skalar multipliziert.

###Example III
−2⎛⎝⎜−11−702−4−1⎞⎠⎟=⎛⎝⎜−2⋅−11−2⋅−7−2⋅0−2⋅2−2⋅−4−2⋅−1⎞⎠⎟=⎛⎝⎜22140−482⎞⎠⎟(3)

##Zerlegung Matrix mal Spaltenmatrix

A matrix multiplying a column matrix can be decomposed into an addition of multiplications. This is due to the previous rules.

###Example IV
⎛⎝⎜234−52−1⎞⎠⎟(λ1λ2)=⎛⎝⎜2λ1+−5λ23λ1+2λ24λ1+−1λ2⎞⎠⎟=λ1⎛⎝⎜234⎞⎠⎟+λ2⎛⎝⎜−52−1⎞⎠⎟(4)

##Zusammenfassung

Matrizenmultiplikation
    AB=C

where A a matrix of size m×n and B a matrix of size m′×n′. The multiplication is possible only if n=m′. Matrix C size is m×n′
.
AB≠AB
Let K=T
, the left multiplication by P gives PK=PT
Let K=T
, the right multiplication by P gives KP=TP

Matrizenaddition

    A+B=(ai,j+bi,j)

Skalarmultiplikation

    λA=(λai,j)

Distributivität

    A(B+C)=AB+AC

Zerlegung Matrix mal Spaltenmatrix

    (v1⋮vn⋯⋯⋯w1⋮wn)(λ1⋮λn)=λ1(v1⋮vn)+⋯+λn(w1⋮wn)
