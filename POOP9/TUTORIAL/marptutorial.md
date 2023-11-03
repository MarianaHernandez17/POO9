---
marp: true
author: Adolfo, Eduardo, Mariana
size: 4:3
theme: gaia
---
## Tutorial para el uso de Marp.
Este tutorial tiene como objetivo explicar funciones básicas respecto a la extensión de VSC Marp.

![width: 800px](descarga.png)

---
## Comandos básicos
Los comandos esenciales para crear una presentación en Marp son:
- **marp: true** : Indica que se usará marp.
- **author**: Indicar los autores del documento.
- **size**: Indicar el tamaño de las diapositivas.
- **theme**: Indicar el diseño de las diapositivas.

---
## Título
Podemos agregar un título de diferentes tamaños usando **#** y podemos reducir el tamaño de letra a mayor número de **#** que se pongan:
# Ejemplo 1
## Ejemplo 2
### Ejemplo 3

---
## Tipografía
Se pueden destacar la tipografía de negritas. itálica, así como el tacahado e insertar código.
- **negrita**: Se ponen 2 asteriscos al inicio y al final de la palabra o frase.
- *italica*: Se pone 1 asterisco al inicio y al final de la palabra o frase.
- ~~tachado~~: Se ponen 2 "~" al inicio y al final de la palabra o frase.
- 'codigo': Se pone comillas simples al inicio y al final del código.

---
## Imágenes 
En Marp también se pueden insertar imágenes estableciendo primero su tamaño y luego el nombre del archivo de imagen que debe estar dentro de la carpeta correspondiente: 

![width: 800px](descarga.png)

---
## Tablas
Para la inserción de tablas, primero se pone la celda y nombre de cada columna comenzando con una barra |(Título 1)|(Título 2)|, para después comenzar a agregar las celdas de manera similar pero poniendo antes |---| para separar del título de la columna de las celdas: 
|Titulo 1|Titulo 2|
|---|---|
|Celda 1|Celda 2|
|Celda 3|Celda 4|