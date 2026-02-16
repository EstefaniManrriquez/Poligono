# Poligono
Proyecto de polígono en Blender

1. Introducción
En este proyecto se desarrolló un script en Python utilizando el entorno de programación de Blender con el objetivo de generar automáticamente un polígono regular en dos dimensiones.
La finalidad fue aplicar fundamentos matemáticos y programación para automatizar la creación de geometría dentro de un software de modelado 3D.

2. Objetivo
Desarrollar un script que permita construir un polígono regular 2D a partir de dos parámetros:
* Número de lados.
* Radio del polígono.

El sistema debe generar los vértices y conectarlos mediante aristas de forma automática.

3. Metodología

Para el desarrollo del proyecto se siguieron los siguientes pasos:

1. Se utilizó el módulo `bpy`, que permite interactuar con Blender mediante Python.
2. Se creó una nueva malla y un objeto dentro de la escena.
3. Se definió una función llamada `crear_poligono_2d`.
4. Se calculó cada vértice aplicando las fórmulas matemáticas descritas.
5. Se almacenaron los vértices en una lista.
6. Se definieron las aristas conectando cada vértice con el siguiente.
7. Se cargaron los datos a la malla mediante el método `from_pydata`.
8. Se ejecutó el script en el editor de Blender.

4. Desarrollo del Código

El programa recibe como parámetros:

* `nombre`: nombre del objeto.
* `lados`: número de lados del polígono.
* `radio`: tamaño del polígono.

El ciclo `for` permite generar cada vértice calculando su posición en el plano XY.
El valor de Z se mantiene en cero para conservar la figura en dos dimensiones.

Posteriormente se crean las conexiones entre vértices mediante otro ciclo, utilizando el operador módulo (%) para cerrar correctamente la figura.

Finalmente, el objeto es vinculado a la colección activa y se actualiza la malla para visualizar el resultado.

5. Resultados

Al ejecutar el script se obtuvo un polígono regular de seis lados (hexágono) con radio 5, centrado en el origen del plano XY.

El sistema permite modificar fácilmente el número de lados y el radio, generando diferentes polígonos regulares sin necesidad de modelado manual.

6. Conclusiones

El uso de scripting en Blender permite automatizar la generación de geometría mediante fundamentos matemáticos y programación.

Se comprobó que:

* Es posible construir figuras geométricas aplicando funciones trigonométricas.
* La automatización reduce tiempo y errores en el modelado.
* Python es una herramienta poderosa para extender las capacidades de Blender.

