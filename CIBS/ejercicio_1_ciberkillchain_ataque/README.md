# Ejercicio CiberKillChain - Ataque

Hacer una copia de este documento para utilizar com plantilla para el ejercicio quitando las instrucciones y el ejemplo.

## Alumno

María Claudia Villarreal Ardila

## Enunciado

Armar una cyberkillchain usando técnicas de la matriz de Att&ck para un escenario relacionado al trabajo práctico de la carrera.



## Datos trabajo práctico

El proyecto consiste en la implementación de un sistema de control de apertura de lockers, este debe permitir que el mensajero deje el paquete en su destino, sin que el destinatario tenga que estar presente.
La operación prevista es: el mensajero llega a destino y llama al destinatario, si el destinatario no se encuentra en su domicilio, abre su aplicación móvil, solicita un código de apertura y se lo informa al mensajero, quien marca ese código en el teclado y el locker se abre, permitiéndole así depositar el paquete.
Internamente, la App envía un pedido de ocupación al broker, el broker envía el código de apertura a la app y también al locker (suscriber). El código, por supuesto, es aleatorio.
Para retirar el paquete, la App envía un pedido de liberación, el broker, nuevamente, envía el código a la App y al locker y lo marca como libre.


## Resolución

Objetivo:
Obtener el Código de apertura para retirar un paquete que se ha depositado en un locker antes de que el destinatario lo retire.

1.	Reconnaissance
•	Identifico el espacio físico en el que se encuentran los lockers y evalúo el nivel de dificultad para acceder a este 
•	Reúno información sobre la App
•	Mediante ofrecimiento de servicios, realización de encuestas o comprando la información, realizo un listado con números de teléfono y/o correos electrónicos de residentes con acceso al sistema de apertura de lockers 

2.	Weaponization
•	Puedo usar phishing buscando que los destinatarios revelen las credenciales de acceso a la App
•	Decido instalar una herramienta de administración remota en el dispositivo de la víctima, que me permita acceder a este en el momento correcto

3.	Delivery
•	Envío a todos los correos electrónicos que logré obtener, un mensaje para inscribirse a una rifa que se realizará entre los residentes, este contiene un link para descargar la herramienta mencionada en el punto anterior

4.	Exploit
•	Algunos residentes leen el correo electrónico y realizan los pasos esperados para la instalación de la herramienta de administración remota del dispositivo

5.	Installation
•	Envío a uno de mis secuaces a un lugar cercano a los lockers para que pueda observar cuando el mensajero deje los paquetes, yo alisto mi dispositivo y minutos después de que me sea notificada la apertura de un locker para dejar un paquete, accedo a la aplicación e ingreso a la herramienta y mediante esta a la App que controla la apertura de los lockers e identifico cuáles están ocupados.

6.	Command & Control
•	Una vez sepa cuál o cuales lockers están ocupados, envió el pedido de liberación, de estos
7.	Actions on Objectives
•	Cuando tengo los códigos para liberar los lockers se los comunico a mi secuaz, quien rápidamente accede al lugar, retira el o los paquetes y escapa.

 

