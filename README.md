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

---

3. Suma de matrices

Para la suma, creé una hoja nueva y utilicé la fórmula:

=HojaA!A1 + HojaB!A1


Luego arrastré hacia abajo y hacia la derecha hasta cubrir el rango A1:AE30.

El resultado fue una imagen mezclada donde cada celda mostraba el valor de la suma de los dos dibujos.

---

4. Resta de matrices

La resta se hizo igual que la suma, pero usando:

=HojaA!A1 - HojaB!A1


Luego arrastré para completar toda la matriz.
Dependiendo de los valores, algunas celdas podían quedar en 0 o en valores pequeños, afectando la intensidad de color en el pixel-art resultante.




