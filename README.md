# Fundamentos de Álgebra - U3.T1 Matrices
**Fecha:** 11 de noviembre de 2025  
**Profesor:** Jorge J. Pedrozo Romero  
**Alumno:** Alexander Fabrizio Rodríguez Pérez  
**Carrera:** TSU en Desarrollo de Software y Negocios Digitales  

## Objetivo de la Documentación
El propósito de esta documentación es registrar las soluciones y el proceso de los ejercicios de la sección "Ejercicios para obtener asistencia" del tema **Matrices**, utilizando formato Markdown.  
El objetivo es reforzar la comprensión del manejo de matrices y sus operaciones básicas, así como practicar la documentación técnica y la organización de información en un repositorio.

## Ejercicios Realizados

### Ejercicio 1: Clasificar matrices

**Enunciado del problema:**  
Identifica el tipo de cada matriz.

$$ A =
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

$$
B =
\begin{pmatrix}
3 & 0 & 0 \\
0 & -2 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}
$$

$$
C =
\begin{pmatrix}
2 & 1 & 4 \\
1 & 3 & 5 \\
4 & 5 & 6 \\
\end{pmatrix}
$$

$$
D =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 4 & 5 \\
0 & 0 & 6
\end{pmatrix}
$$

**Solución o respuesta:**
Matriz A: Cuadrada, diagonal e identidad.
Matriz B: Cuadrada y diagonal.
Matriz C: Cuadrada y simétrica (C = Cᵗ).
Matriz D: Cuadrada y triangular superior.

**Procedimiento:**
Verificar la dimensión de cada matriz (todas son cuadradas).

Analizar los elementos fuera de la diagonal para determinar si son ceros.

Comparar C con su transpuesta para confirmar si es simétrica.

Comprobar que en D los elementos bajo la diagonal son ceros.

Determinar que A es identidad, ya que la diagonal son unos y el resto ceros.

**Resultado final:**
Matriz	Tipo de matriz
A	Cuadrada, diagonal, identidad
B	Cuadrada, diagonal
C	Cuadrada, simétrica
D	Cuadrada, triangular superior

### Ejercicio 2: Operaciones básicas con matrices

**Enunciado del problema:**  
Dadas las matrices A y B, calcula:  
a) A + B  
b) 2A - B  
c) A × B  
d) B × A  
e) Aᵗ  

$$
A =
\begin{pmatrix}
2 & -1 \\
3 & 4
\end{pmatrix}
$$

$$
B =
\begin{pmatrix}
5 & 2 \\
-1 & 3
\end{pmatrix}
$$


**a) A + B**

$$
A =
\begin{pmatrix}
(2+5) & (-1+2) \\
(3-1) & (4+3)
\end{pmatrix}
$$

Resultado:

$$
A =
\begin{pmatrix}
7 & 1 \\
2 & 7
\end{pmatrix}
$$       

**b) 2A - B**

$$
2A =
\begin{pmatrix}
4 & -2 \\
6 & 8
\end{pmatrix}
$$

$$
2A - B =
\begin{pmatrix}
(4-5) & (-2-2) \\
(6-(-1)) & (8-3)
\end{pmatrix}
$$

**Resultado:**

$$
\begin{pmatrix}
-1 & -4 \\
7 & 5
\end{pmatrix}
$$

---

**c) A × B**

$$
A \times B =
\begin{pmatrix}
(2 \times 5) + (-1 \times -1) & (2 \times 2) + (-1 \times 3) \\
(3 \times 5) + (4 \times -1) & (3 \times 2) + (4 \times 3)
\end{pmatrix}
$$

**Resultado:**

$$
\begin{pmatrix}
11 & 1 \\
11 & 18
\end{pmatrix}
$$

---

**d) B × A**

$$
B \times A =
\begin{pmatrix}
(5 \times 2) + (2 \times 3) & (5 \times -1) + (2 \times 4) \\
(-1 \times 2) + (3 \times 3) & (-1 \times -1) + (3 \times 4)
\end{pmatrix}
$$

**Resultado:**

$$
\begin{pmatrix}
16 & 3 \\
7 & 13
\end{pmatrix}
$$

---

**e) Aᵗ (transpuesta de A)**

$$
A^T =
\begin{pmatrix}
2 & 3 \\
-1 & 4
\end{pmatrix}
$$

---

**Resultado final:**

$$
A + B =
\begin{pmatrix}
7 & 1 \\
2 & 7
\end{pmatrix}
$$

$$
2A - B =
\begin{pmatrix}
-1 & -4 \\
7 & 5
\end{pmatrix}
$$

$$
A \times B =
\begin{pmatrix}
11 & 1 \\
11 & 18
\end{pmatrix}
$$

$$
B \times A =
\begin{pmatrix}
16 & 3 \\
7 & 13
\end{pmatrix}
$$

$$
A^T =
\begin{pmatrix}
2 & 3 \\
-1 & 4
\end{pmatrix}
$$



### Ejercicio 3: Verificación de la propiedad asociativa

**Enunciado del problema:**  
Dadas las matrices A, B y C, verifica que (AB)C = A(BC).

$$
A =
\begin{pmatrix}
1 & 2 \\
3 & 4
\end{pmatrix}
$$

$$
B =
\begin{pmatrix}
2 & 0 \\
1 & 3
\end{pmatrix}
$$

$$
C =
\begin{pmatrix}
1 & 1 \\
0 & 2
\end{pmatrix}
$$

**Paso 1: Calcular $AB$**

$$
AB = \begin{pmatrix}
2 & -1 \\
3 & 4
\end{pmatrix} \begin{pmatrix}
5 & 2 \\
-1 & 3
\end{pmatrix} = 
\begin{pmatrix}
(2 \times 5) + (-1 \times -1) & (2 \times 2) + (-1 \times 3) \\
(3 \times 5) + (4 \times -1) & (3 \times 2) + (4 \times 3)
\end{pmatrix}
$$

$$
AB = \begin{pmatrix}
10 + 1 & 4 - 3 \\
15 - 4 & 6 + 12
\end{pmatrix} = 
\begin{pmatrix}
11 & 1 \\
11 & 18
\end{pmatrix}
$$

**Paso 2: Calcular $(AB)C$**

$$
(AB)C = \begin{pmatrix}
11 & 1 \\
11 & 18
\end{pmatrix} \begin{pmatrix}
1 & 1 \\
0 & 2
\end{pmatrix} = 
\begin{pmatrix}
(11 \times 1) + (1 \times 0) & (11 \times 1) + (1 \times 2) \\
(11 \times 1) + (18 \times 0) & (11 \times 1) + (18 \times 2)
\end{pmatrix}
$$

$$
(AB)C = \begin{pmatrix}
11 + 0 & 11 + 2 \\
11 + 0 & 11 + 36
\end{pmatrix} = 
\begin{pmatrix}
11 & 13 \\
11 & 47
\end{pmatrix}
$$

**Paso 3: Calcular $BC$**

$$
BC = \begin{pmatrix}
5 & 2 \\
-1 & 3
\end{pmatrix} \begin{pmatrix}
1 & 1 \\
0 & 2
\end{pmatrix} = 
\begin{pmatrix}
(5 \times 1) + (2 \times 0) & (5 \times 1) + (2 \times 2) \\
(-1 \times 1) + (3 \times 0) & (-1 \times 1) + (3 \times 2)
\end{pmatrix}
$$

$$
BC = \begin{pmatrix}
5 + 0 & 5 + 4 \\
-1 + 0 & -1 + 6
\end{pmatrix} = 
\begin{pmatrix}
5 & 9 \\
-1 & 5
\end{pmatrix}
$$

**Paso 4: Calcular $A(BC)$**

$$
A(BC) = \begin{pmatrix}
2 & -1 \\
3 & 4
\end{pmatrix} \begin{pmatrix}
5 & 9 \\
-1 & 5
\end{pmatrix} = 
\begin{pmatrix}
(2 \times 5) + (-1 \times -1) & (2 \times 9) + (-1 \times 5) \\
(3 \times 5) + (4 \times -1) & (3 \times 9) + (4 \times 5)
\end{pmatrix}
$$

$$
A(BC) = \begin{pmatrix}
10 + 1 & 18 - 5 \\
15 - 4 & 27 + 20
\end{pmatrix} = 
\begin{pmatrix}
11 & 13 \\
11 & 47
\end{pmatrix}
$$

**Conclusión:**

$$
(AB)C = \begin{pmatrix}
11 & 13 \\
11 & 47
\end{pmatrix} = A(BC)
$$

**Conclusión:**

$$
(A \times B) \times C = A \times (B \times C)
$$

Por lo tanto, se cumple la **propiedad asociativa** de la multiplicación de matrices.


## Conclusión general
Los tres ejercicios permitieron aplicar los conceptos fundamentales de las matrices:

Clasificación de tipos de matrices (identidad, diagonal, simétrica, triangular).

Operaciones básicas: suma, resta, multiplicación escalar, multiplicación de matrices y transpuesta.

Verificación de propiedades algebraicas, como la asociatividad.

El desarrollo de estos ejercicios permitió reforzar la comprensión del álgebra matricial
y la práctica de documentación técnica en formato Markdown.
