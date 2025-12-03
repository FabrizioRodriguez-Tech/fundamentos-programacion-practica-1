# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Cristopher Maximiliano Euan Pool
## Actividad \4 - Matrices doc

---

# 🟦 Ejercicio 1

## Sistema

$$
\begin{cases}
x + y + z = 6\\
2x - y + z = 3\\
x + 2y - z = 2
\end{cases}
$$

## Matriz aumentada (Gauss)

$$
\begin{pmatrix}
1 & 1 & 1 & 6\\
2 & -1 & 1 & 3\\
1 & 2 & -1 & 2
\end{pmatrix}
\rightarrow
\begin{pmatrix}
1 & 1 & 1 & 6\\
0 & -3 & -1 & -9\\
0 & 1 & -2 & -4
\end{pmatrix}
\rightarrow
\begin{pmatrix}
1 & 1 & 1 & 6\\
0 & -3 & -1 & -9\\
0 & 0 & -7 & -21
\end{pmatrix}
$$

## Resultado
$$
x=1,\quad y=2,\quad z=3
$$

---

# 🟩 Gauss–Jordan

$$
\begin{pmatrix}
1 & 1 & 1 & 6\\
0 & -3 & -1 & -9\\
0 & 0 & -7 & -21
\end{pmatrix}
\rightarrow
\begin{pmatrix}
1 & 0 & 0 & 1\\
0 & 1 & 0 & 2\\
0 & 0 & 1 & 3
\end{pmatrix}
$$

## Resultado

$$
x=1,\quad y=2,\quad z=3
$$

---

# 🟪 Matriz Inversa (AX = B)

### Matrices

$$
A=
\begin{pmatrix}
1 & 1 & 1\\
2 & -1 & 1\\
1 & 2 & -1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
6\\3\\2
\end{pmatrix}
$$

### Resultado
$$
X = A^{-1}B =
\begin{pmatrix}
1\\2\\3
\end{pmatrix}
$$

---

# 🟫 Cofactores / Adjunta

$$
\det(A)=7
$$

$$
A^{-1} = \frac{1}{7}\,\text{adj}(A)
$$

### Resultado
$$
\begin{pmatrix}
1\\2\\3
\end{pmatrix}
$$

---

# 🟧 Regla de Cramer

$$
\det(A)=7,\qquad  
\det(D_x)=7,\qquad  
\det(D_y)=14,\qquad  
\det(D_z)=21
$$

### Resultado

$$
x=1,\quad y=2,\quad z=3
$$

---

# 🟦 Ejercicio 2

## a)
$$
\begin{cases}
x+y=3\\
2x+2y=6
\end{cases}
$$

**Conclusión:**  
Tiene infinitas soluciones.

---

## b)
$$
\begin{cases}
x+y=3\\
2x+2y=7
\end{cases}
$$

**Conclusión:**  
No tiene solución.

---

## c)
$$
\begin{cases}
x+y=3\\
x-y=1
\end{cases}
$$

**Conclusión:**  
Solución única:

$$
(x,y)=(2,1)
$$

---

# 🟩 Ejercicio 3

## Sistema

$$
\begin{cases}
x+y+z+w=10\\
2x+y-z+w=5\\
x-y+z-w=1\\
x+y-z+2w=8
\end{cases}
$$

## Matriz reducida (Gauss–Jordan)

$$
\begin{pmatrix}
1 & 0 & 0 & 0 & 0\\
0 & 1 & 0 & 0 & -\frac{5}{2}\\
0 & 0 & 1 & 0 & \frac{7}{2}\\
0 & 0 & 0 & 1 & 5
\end{pmatrix}
$$

## Resultado

$$
x=0,\quad
y=-\frac{5}{2},\quad
z=\frac{7}{2},\quad
w=5
$$

---

# 🟪 Ejercicio 4

## Sistema

$$
\begin{cases}
2P + S + 3U = 100\\
3P + S + 2U = 120\\
P + 2S + U = 80
\end{cases}
$$

## Matriz reducida

$$
\begin{pmatrix}
1 & 0 & 0 & 27.5\\
0 & 1 & 0 & 22.5\\
0 & 0 & 1 & 7.5
\end{pmatrix}
$$

## Resultado

$$
P=27.5,\quad
S=22.5,\quad
U=7.5
$$

---

# ✅ Conclusión
Se documentaron los sistemas y resultados utilizando matrices en formato LaTeX para una presentación clara, ordenada y profesional.
