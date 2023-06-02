# Laboratorio No° 5

### Integrantes:
- Santiago Andres Gomez Pena <sagomezpe@unal.edu.co>
- Julian Felipe Medina Veira <jmedinave@unal.edu.co>
- Santiago Dleon Sanchez Romero <ssanchezro@unal.edu.co>


![phantom x](https://github.com/jmedinave/Lab-4--Robotica/assets/49196705/429be8d6-74e6-4678-9220-b16d22270292)                   
![image](https://github.com/jmedinave/Lab-4--Robotica/assets/49196705/db5b3025-32a1-4bb7-918f-5f6461aff75a)


### Introducción:
Este repositorio expone el procedimiento para cumplir la guia de laboratorio #5 el cual busca que se cumplan los siguientes puntos:

<ul>
    <li>El robot deber&aacute; tomar un marcador borrable y dibujar figuras en la superficie plana de trabajo.</li>
    <li>El robot debe ser controlado por un &uacute;nico programa (script) y este programa debe ser controlado por el usuario.</li>
    <li>Tomando como base el trabajo realizado en el laboratorio de cinem&aacute;tica directa, y utilizando el modelo de cinem&aacute;tica inversa desarrollado, cree un script que ejecute las rutinas descritas.&nbsp;</li>
    <li>Cree una base porta herramienta para el marcador de forma que cuando el brazo tome y suelte el marcador la orientaci&oacute;n respecto a la herramienta sea v&aacute;lida para escribir sobre la superficie plana, esta base debe estar sujeta a la tabla de trabajo mediante un acople temporal, no da&ntilde;e la superficie de la tabla.</li>
</ul>
<p>El programa debe contar con las siguientes <strong>rutinas</strong>:</p>
<ul>
    <li><strong>Cargar herramienta:</strong> el brazo se desplaza a la base porta herramienta, sujeta el marcador y se ubica en una posici&oacute;n de espera.</li>
    <li><strong>Espacio de trabajo</strong>: el brazo dibuja dos arcos que representan los l&iacute;mites de espacio de trabajo diestro plano sobre la superficie y regresa a una posici&oacute;n de espera.</li>
    <li><strong>Dibujo de Iniciales</strong>: El brazo dibuja al menos dos letras, iniciales de los nombres de los estudiantes, sobre la superficie y retorna a una posici&oacute;n de espera.</li>
    <li><strong>Dibujo de figura libre</strong>: Se dibuja sobre la superficie una figura libre que utilice segmentos rectos y curvos.</li>
    <li><strong>Descarga de la herramienta</strong>: el brazo se desplaza a la base porta herramienta, suelta el marcador y se ubica en una posici&oacute;n de Home.</li>
</ul>
<p>Adicionalmente, el programa debe contar con una interfaz Humano m&aacute;quina HMI.</p>

### Base porta Herramienta y marcador utlizado:

Para el soporte de la herramienta en la base del area de trabajo, se implemento un soporte con la tapa del marcador utilizado a la mesa tal como muestra la siguiente imagen:

![Imagen de WhatsApp 2023-05-26 a las 18 14 06 (1)](https://github.com/jmedinave/Lab-5/assets/49196705/50ec9ed8-a176-48a8-aeea-991137d35059)


### Descripción de la solución planteada:

### Rutinas implementadas:


### Interfaz HMI:

### Análisis de precisión

### Conclusiones

* La presición y exactitud del robot Phantom X es baja debido a que los movimientos son muy bruscos, incluso bajando el delta entre cada punto intermedio de una trayectoria no podemos obtener una trayectoria muy exacta o precisa, esto además se propaga debido a que varios robots del laboratorio tienen algo de libertad de rotación incluso estando energizados debido a que no están bien ajustados a los soportes.

* Una buena comprensión de la cinemática inversa nos permité hacer nuestra propia implementación del control del movimiento del robot, lo cual fue fundamental para implementar la solución de nuestra alicación.

* Ros, junto a modelos de cinemática inversa y directa, permite controlar los movimientos de un robot por medio de python y/o Matlab con suficiente precisión como para recorrer trayectorias complejas.

* La precisión con la que el robot se comporte a comparación del comportamiento simulado ideal depende de factores físicos del robot, como la rigidez de sus eslabones, las fuerzas externas asociadas al proceso y la interfaz que lo controla (esto ultimo respecto al envió de valores de articulación discontinuo desde Matlab). Esta precisión determina la calidad con la que lleva a cabo su función, pues como se evidencio, la desviación entre trayectorias ideales y reales puede ser significativa.






