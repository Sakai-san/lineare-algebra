#Kapitel 3 : Matrix und Eliminationsverfahren

## Matrix

Eine Matrix ist eine Tablelle mit m Zeilen and n Spalten.

Die Matrix enhählt die Koeffizienten eines linearen Systems. Die sind die sogenannten Elementen der Matrix.

Beispiel I zeigt wie ein lineares System sich in einer matrizielen Gleichung in der Form Ax⃗ =y⃗ darstellen lässt.

### Beispiel I

⎧⎩⎨⎪⎪−x−3y+zx+y−3z3x+4y+2z===10−12−5⟺⎛⎝⎜−113−3141−32⎞⎠⎟A⎛⎝⎜xyz⎞⎠⎟x⃗ =⎛⎝⎜10−12−5⎞⎠⎟y⃗


Die Elemente der Matrix werden durch zwei Indizes bezeichnet, also aij, wobei i für die Zeile bzw. j für die Spalte stehen. Als Beispiel, das Element a3,2 der Matrix A des Beispieles I gleich 4 ist.


#Eliminationsverfahren

Das Eliminationsverfahren, auch under dem Namen Gauss-Verfahren bekannt, ist eine Method, um lineare Systeme aufzulösen. Eigentlich handelt sich diese Method, um das Additionsverfahren auf eine Matrix angewandet.

Dazu beginnt man mit der sogenannten erweiterten Matrix wie im Beispiel II erläutert. Die Elimination einer Variable besteht in der Addition zweier Zeilen. Die daraus ergebende Gleichung wird eine der zwei genannten Zeilen ersetzen.

### Beispiel II

⎛⎝⎜⎜−113−3141−3210−12−5⎞⎠⎟⎟⟺R1+R2→R2⎛⎝⎜⎜−103−3−241−2210−2−5⎞⎠⎟⎟⟺3R1+R3→R3⎛⎝⎜⎜−100−3−2−51−2510−225⎞⎠⎟⎟

⟺−12R2→R2⎛⎝⎜⎜−100−31−511510125⎞⎠⎟⎟⟺5R2+R3→R3⎛⎝⎜⎜−100−310111010130⎞⎠⎟⎟

Nachdem die erweiterte Matrix die sogenannte Zeilenstufenform angenommen hat, läss sich das linear System von unten her auflösen, wie folgendes :

10z=30 ⟺ z=3

Aus Einsetzen von z in der zweiten Zeile folgt :

y+1⋅3z=1⟺ y=−2

Durch Einsetzen von y und z in der ersten Zeile lautet hier :

−1x+−3⋅−2y+1⋅3z=10⟺−x+9=10⟺x=−1

Die Lösung lautet hier :

x⃗ =⎛⎝⎜−1−23⎞⎠⎟(1)


Figur 3.1 : eindeutiger Schnittpunkt (credits montereyinstitute)

# Beispiel III

⎧⎩⎨⎪⎪4x+y+3z2x+y+z−x−y===120⟺⎛⎝⎜⎜42−111−1310120⎞⎠⎟⎟⟺R1↔R3⎛⎝⎜⎜−124−111013021⎞⎠⎟⎟

⟺2R1+R2→R2⎛⎝⎜⎜−104−1−11013021⎞⎠⎟⎟⟺4R1+R3→R3⎛⎝⎜⎜−100−1−1−3013021⎞⎠⎟⎟⟺−3R2+R3→R3⎛⎝⎜⎜−100−1−1001002−5⎞⎠⎟⎟

Aus der letzten Zeile folgt :

0x+0y+0z=5

Die obige Gleichung ist unlösbar, also hat das System keine Lösung :
x⃗ ={}(2)


# Beispiel IV

{2x+−2yx+−y==21⟺(21−2−121)⟺R1↔R2(12−1−212)⟺−2R1+R2→R2(10−1010)

Aus der letzten Zeile folgt :

0x+0y=0⟺0=0

Die obige Gleichung ergibt keine Information über die Variable.

Dann gehen wir eine Zeile oben weiter und daraus fogt :

1x+−1y=1⟺x=1+y. Let y=β.

Es bleibt hier eine relevante Gleichung doch besitzt das System zwei Variablen.

Das heisst, dass das System unendliche viele Lösungen hat und die allgemeine Lösung lautet :

x⃗ =(1+ββ),β∈R(3)


#Zusammenfassung

Mit der Darstellung eines linearen Systemes in einer matrizielen Gleichung lässen sie sich die Koeffiziente von den Variablen trennen. Dies macht es mehr leserlich.

Aus der erweiterten Matrix werden Operationen auf Zeilen ausgeführt, zwar Zeileaustauchen, Zeilemultiplizieren mit einem nicht-Null Faktor und Zeileersetzen durch die Summe zweier Zeilen miteinander, bis die genannte Matrix eine Zeilenstufenform angenommen hat, d.H wie eine Treppe aussieht.  

Aus der Zeilenstufenform der Matrix, muss man von unten her die Zeile lösen und rückwärts je Werte einsetzen. Nullzeilen ergeben keine Information über die Variable und können daher ignoriert werden.
