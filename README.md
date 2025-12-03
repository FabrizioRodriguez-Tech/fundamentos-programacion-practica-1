2.1 Modificar el archivo README.md
Abre el archivo README.md existente y modifica:

# Documentación de Ejercicios - 
 ## Información General - **Materia:** Fundamentos de Álgebra - **Tema:** Matrices, transpuestas y operaciones matriciales. - **Fecha:** 25/11/2025 - **Estudiante:** Alexander Fabrizio Rodriguez Pérez - **Grupo:** 1°A
 ## Objetivo de la Documentación El objetivo de este documento es presentar y explicar las actividades realizadas con matrices utilizando representaciones visuales tipo pixel-art en Google Sheets.
Incluye la creación de matrices 30×30, sus transpuestas y operaciones como suma, resta, multiplicación escalar y composición matricial.--- 
 ## Ejercicios Realizados Desarrollo del Proyecto
1. Preparación de las hojas y formato cuadriculado

Comencé ajustando cada hoja de Google Sheets para que tuviera un formato tipo píxel. Para esto:

Configuré 30 filas y 30 columnas.

Ajusté manualmente el tamaño de cada celda para que quedaran cuadradas.

Luego seleccioné toda la hoja y usé Formato → Reglas de formato condicional para asignar colores según los valores del 0 al 9 (los números que utilicé para representar cada color del dibujo).
Cada dibujo se creó colocando los números uno por uno dentro de las 900 celdas (30×30).

Cuando terminé este proceso, ya tenía 5 matrices originales, cada una representando una imagen diferente.
<img width="767" height="585" alt="image" src="https://github.com/user-attachments/assets/7b18711a-9c89-4395-9ae4-583cee663f28" />
<img width="475" height="480" alt="image" src="https://github.com/user-attachments/assets/c207e266-d714-4376-9dab-179751c04795" />
<img width="697" height="573" alt="image" src="https://github.com/user-attachments/assets/bcd80354-40e7-4515-958a-551eb4deaac2" />
<img width="818" height="596" alt="image" src="https://github.com/user-attachments/assets/0a702d86-bbd8-4602-b0de-4faf568bc3c4" />
<img width="654" height="570" alt="image" src="https://github.com/user-attachments/assets/2ff31066-4163-4118-97be-da284ceaf57f" />




---
2. Creación de las matrices transpuestas

Para obtener la transpuesta de cada imagen, utilicé el método de copiar y pegar especial:

Seleccioné todo el rango de la imagen original (A1:AE30).

Presioné Ctrl+C para copiar.

Fui a una nueva hoja.

Seleccioné la celda A1.

Usé Editar → Pegado especial → Transponer.

Esto generó una matriz de 30×30 donde las filas pasaron a ser columnas y viceversa.
El formato condicional se mantuvo, por lo que la imagen transpuesta conservó sus colores originales pero con la estructura invertida.

Así obtuve las 5 matrices transpuestas.

<img width="622" height="567" alt="image" src="https://github.com/user-attachments/assets/be0d65cb-64cf-4c2f-9ec2-ea21f3be1c8d" />
<img width="585" height="592" alt="image" src="https://github.com/user-attachments/assets/5839d8b5-f7c7-402e-8524-50bee611c666" />
<img width="648" height="479" alt="image" src="https://github.com/user-attachments/assets/d7402262-e496-40ac-996e-31ca4d602894" />
<img width="626" height="662" alt="image" src="https://github.com/user-attachments/assets/6c76d6f4-aeb1-4214-a434-b7d6aebc8698" />
<img width="661" height="652" alt="image" src="https://github.com/user-attachments/assets/fd624149-e53a-4a4a-b5a6-7f99448277b1" />


---

3. Suma de matrices

Para la suma, creé una hoja nueva y utilicé la fórmula:

=HojaA!A1 + HojaB!A1


Luego arrastré hacia abajo y hacia la derecha hasta cubrir el rango A1:AE30.

El resultado fue una imagen mezclada donde cada celda mostraba el valor de la suma de los dos dibujos.
<img width="650" height="606" alt="image" src="https://github.com/user-attachments/assets/18bb2552-6454-46bd-b4af-b8cf0d480f33" />


---

4. Resta de matrices

La resta se hizo igual que la suma, pero usando:

=HojaA!A1 - HojaB!A1


Luego arrastré para completar toda la matriz.
Dependiendo de los valores, algunas celdas podían quedar en 0 o en valores pequeños, afectando la intensidad de color en el pixel-art resultante.
<img width="632" height="637" alt="image" src="https://github.com/user-attachments/assets/a9eae5bc-91c7-477c-8be1-a1260b4b566f" />


---

5. Multiplicación escalar

Para multiplicar una matriz por un escalar, escribí el número escalar en una celda (por ejemplo F1) y luego utilicé esta fórmula:

=HojaA!A1 * $F$1


Después rellené toda la matriz arrastrando hacia abajo y a la derecha.
Esto hizo que la imagen original se “intensificara” o cambiara según el valor del escalar.
<img width="649" height="621" alt="image" src="https://github.com/user-attachments/assets/1df4c901-53b1-43e2-88c5-6cf8a1ca7e8a" />

---

6. Composición de matrices

La composición se elaboró colocando la imagen B "encima" de la imagen A, de manera que:

Si B tenía un número → ese número aparecía en la imagen final.

Si la celda de B estaba vacía → se mostraba el valor de A.

Esto funcionó como una superposición similar a una capa transparente.
La fórmula utilizada fue:

=IF(HojaB!A1="", HojaA!A1, HojaB!A1)


Después arrastré la fórmula hasta completar todo el rango A1:AE30.
<img width="647" height="602" alt="image" src="https://github.com/user-attachments/assets/4ef2e395-c039-4d2d-bd93-e56889007011" />



