# ImformeLaboratorio

AUTORES:


**1.OBJETIVOS** 

Objetivo General

Desarrollar el método de Thevenin en el circuito propuesto utilizando los métodos previamente observados.


Objetivos Específicos

Calcular el voltaje de Thevenin en el circuito propuesto utilizando el teorema de Thevenin y el teorema de superposición.

Mostrar el voltaje y resistencia total obtenidos mediante el método de Thevenin

**2.MARCO TEÓRICO**

 ![](https://github.com/Anabeltoapanta/LABORATORIO-5/blob/main/marco%20teorico%20labo%205.png)


**3. EXPLICACIÓN DEL PROCEDIMIENTO**

Según lo planteado anteriormente el método de Thévenin es un circuito equivalente de cualquier circuito sea mixto o simplemente en serie o paralelo a un circuito resistivo de dos terminales en donde consta de una fuente de voltaje que la llamaremos VTH y una resistencia equivalente llamada RTH.

Para nuestra practica vamos a necesitar las siguientes herramientas
•	Protoboard 
•	5 resistencias
•	1 potenciómetro de precisión de 1 Kohm
•	2 Fuentes de Voltaje
•	Cables de conexión  
•	Multímetro

PROCEDIMIENTO
Para nuestra practica debemos conocer dicho teorema previamente, el cual nos dice que todo circuito por mas complejo que sea este, puede ser simplificado a un circuito equivalente con respecto a dos terminales de salida.

Esto quiere decir que no este circuito equivalente tendrá una resistencia equivalente y un voltaje equivalente con respecto a dos terminales de salida.

Como primer parámetro necesitamos realizar un diagrama esquemático como lo vemos a continuación.

![image](https://user-images.githubusercontent.com/85134094/127005331-f2f3c25f-69da-4451-9f1b-2aa301bdcfa3.png)

En donde nos pide calcular la corriente y el voltaje que circulan por la R5

Para ello los pasos que seguiremos son los siguientes:

1)	Procederemos a simular el circuito en Tinkercad de la siguiente manera 

![image](https://user-images.githubusercontent.com/85134094/127005417-9c510236-dc13-4a68-ab4d-694a990d3a5d.png)

2)	Procedemos a medir la corriente que pasa por la R5, conectando en serie el multímetro a dicha resistencia:

![image](https://user-images.githubusercontent.com/85134094/127005462-d29bedca-33a5-4f46-8c17-6c84fd84c6ed.png)

3)	Procedemos medir el Voltaje que pasa por la R5, conectando el multímetro paralelamente a dicha resistencia:

![image](https://user-images.githubusercontent.com/85134094/127005478-abd9fac4-13e5-46cc-9851-3b7219d4a98f.png)

4)	A continuación, quitamos la resistencia R5 y medimos su voltaje en el circuito abierto, a este voltaje medido se lo llama voltaje de Thévenin V TH:

![image](https://user-images.githubusercontent.com/85134094/127005495-c04db0c5-f0d2-4245-a1db-22ca2de693d1.png)

5)	A continuación, transformamos las fuentes de voltaje en cortos circuitos configurándolos con su valor de voltaje a cero y procedemos a medir la resistencia total sin la resistencia R5, a esta resistencia total la llamamos resistencia de Thévenin RTH.

![image](https://user-images.githubusercontent.com/85134094/127005533-e6a254ea-47c6-48b8-8fb1-136e8b977ef5.png)

6)	A continuación, implementamos el circuito equivalente de Thévenin, conectando la R5 a los terminales abiertos de la siguiente manera:

![image](https://user-images.githubusercontent.com/85134094/127005554-29350114-b8fe-44a0-af91-6d0c52607c9e.png)

7)	A continuación, medimos la intensidad en la R5 conectando el multímetro en serie a dicha resistencia:

![image](https://user-images.githubusercontent.com/85134094/127005578-65890fe9-faef-49dc-a0ac-c384a236db8c.png)

8)	Y por último, medimos el voltaje en la R5 conectando el multímetro paralelamente a dicha resistencia:

![image](https://user-images.githubusercontent.com/85134094/127005604-1dea5f04-5f46-4cf5-b462-adbd04d8a24c.png)

**4. RESPUESTAS A INTERROGANTES**

A continuación, procederemos a realizar los cálculos para demostrar que los datos medidos anteriormente en la practica sean los correctos. 
Para ello nos ayudaremos del diagrama del circuito

![image](https://user-images.githubusercontent.com/85134094/127005670-2b1478d8-e438-44f7-9ab4-07a95c53fe67.png)

En donde el primer paso es calcular la Intensidad y el voltaje que circula por la R5, para esto utilizamos el método de mallas como se muestra a continuación: 

![image](https://user-images.githubusercontent.com/85134094/127005685-4d03e749-f485-4248-9941-fd90063fc912.png)

Para lo siguiente tenemos que retirar la R5 del circuito y calcular los valores del voltaje para los terminales a y b:

![image](https://user-images.githubusercontent.com/85134094/127005730-06126016-4bbb-4783-a016-70595769505f.png)

Para ello nos ayudaremos del método de superposición como se muestra a continuación:

Primero tomaremos como un cortocircuito la fuente de voltaje 2, cabe destacar que por la R4 no circula ninguna corriente por lo que no se la tomara en cuenta para nuestros cálculos.

![image](https://user-images.githubusercontent.com/85134094/127005760-bb6a2dc1-9820-496c-8d96-28217a47ff3a.png)

Como segundo parámetro tomaremos la fuente de voltaje 1 como un cortocircuito, no sin antes mencionar que se aplica el mismo concepto para la R4 en donde no circula corriente por lo que no se lo tomara en cuenta para nuestros cálculos.

![image](https://user-images.githubusercontent.com/85134094/127005793-ee70353d-8beb-4b9f-8f7a-87cd31c573b5.png)

En donde el voltaje de Thévenin resulta de la suma de los voltajes antes calculados en los terminales a y b:

![image](https://user-images.githubusercontent.com/85134094/127005819-7ad60227-d361-442b-bb4a-f3410162b1ed.png)

Como tercer parámetro tomamos nuevamente las fuentes de energía como si fueran cortos circuitos es decir resistencias de valor cero y calculamos la resistencia total y esta resistencia será la resistencia de Thévenin.

![image](https://user-images.githubusercontent.com/85134094/127005840-a1909634-43fd-4981-b2e8-aaaa459e7442.png)

Por último, implementamos el circuito equivalente de Thévenin, en donde tenemos la fuente de voltaje con el valor calculado anteriormente llamado voltaje de Thévenin y la resistencia de Thévenin. A este circuito le añadimos la Resistencia 5 que habíamos retirado anteriormente:

![image](https://user-images.githubusercontent.com/85134094/127005867-5895ff4e-1759-4413-ab30-91698127e233.png)

Y procedemos a calcular la Intensidad y el voltaje en la R5 

![image](https://user-images.githubusercontent.com/85134094/127005905-9d4680f9-c445-4b2f-819c-bf16cd9bec63.png)

Todos estos datos los anotamos en una tabla a continuación y comparamos resultados los cuales nos coinciden los valores calculados con los valores medidos.

![image](https://user-images.githubusercontent.com/85134094/127005996-3905d826-49f4-4db2-bf2f-a905931aed44.png)

**5. VIDEO**

link del video 

https://youtu.be/UDBoQgGre60

**6. CONCLUSONES**
 
 •	Cualquier circuito mixto o simplemente en serie o paralelo puede ser simplificado con respecto a dos terminales de salida con la ayuda del teorema de Thévenin
 
 •	Este metodo nos sirve para calcular circuitos demasiado complejos llevandonos a un circuito simplificado
 
•	Los valores de voltaje y resistencia de thévenin depende de los valores del circuito original, qesto quiere decir que todos los valores son calculados a parotir de los valores iniciales

•	Esta práctica nos permitió visualizar tanto  experimental y matemáticamente como se emplea el Teorema de Thevenin, el cual consiste en que el valor de las resistencias puede ser reemplazada o sustituida por otra fuente de tensión.
 

**7. BIBLIOGRAFÍA**

Robbins, A. H. (2008). Análisis de Circuitos Teoria y Practica. Santa Fe-Mexico: Cengage Learning.


