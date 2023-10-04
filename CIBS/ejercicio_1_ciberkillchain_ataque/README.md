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
Soy líder de una organización criminal dedicada al asesinato a sueldo, hemos sido contratados para liquidar un individuo, se trata de una persona que posee información confidencial y ha estado extorsionando a nuestro cliente, obligándolo a pagar fuertes sumas de dinero a cambio de su silencio.
Las labores de espionaje realizadas advirtieron que el objetivo pasa la mayor parte del día en su domicilio, no tiene un horario claro de salidas, y cuando lo hace se moviliza en un auto blindado, además siempre está armado, lo cual lo convierte en un objetivo difícil. Sin embargo, también se detectó que el hombre pide la mayoría de sus comidas a domicilio, y frecuentemente, a pesar de estar en casa, prefiere usar el sistema de apertura de lockers instalado en el edificio en el que vive, que recibir la comida directamente al mensajero.
Se decide aprovechar el uso de este sistema, obteniendo el código de apertura para manipular los alimentos del objetivo, aplicando en varias oportunidades dosis pequeñas de un veneno indetectable, causando una muerte lenta y silenciosa, que probablemente no sea investigada.

1.	Reconnaissance
   
•	Espías detectan que el objetivo usa frecuentemente el sistema de control de apertura de lockers para recibir alimentos a domicilio.

•	(T1589.002) Gather Victim Identity Information: Se recurre a la miembros de la administración del edificio fingiendo ser una empresa de lavandería para acceder al correo electrónico del objetivo y de otros residentes
Técnica: https://attack.mitre.org/techniques/T1589/002/

•	(T1598.001)Phishing for Information: Se usa principalmente para obtener información de otros residentes del edificio sobre la app del sistema de control de apertura de lockers.
Técnica: https://attack.mitre.org/techniques/T1598/001/


2.	Weaponization
   
•	Puedo usar phishing buscando que la víctima revele las credenciales de acceso a la App

•	Decido instalar un Troyano de acceso remoto en el dispositivo de la víctima, que me permita acceder a este en el momento correcto

3.	Delivery
   
•	(T1456) Drive-By Compromise: Envío al correo electrónico del objetivo un mensaje para inscribirse a una rifa que se realizará entre los residentes del edificio, este contiene un link a un sitio web para descargar la herramienta mencionada en el punto anterior

4.	Exploit
   
•	El objetivo abre el correo electrónico y da click en el link malicioso 

5.	Installation
   
•	(T1577) Compromise Application Executable: Se abre el sitio web desde el cual se descarga la herramienta de administración remota y esta se instala en el dispositivo de la víctima.
Técnica: https://attack.mitre.org/techniques/T1577/

6.	Command & Control
    
•	Uno de mis secuaces se ubica en un lugar cercano a los lockers con un teléfono celular desde el cual se comunica conmigo.
•	Alisto mi dispositivo para acceder al sistema del móvil de la víctima mediante el Troyano de acceso remoto


7.	Actions on Objectives
    
•Mi secuaz debe informarme si un domiciliario se acerca al locker de la víctima, realiza la llamada para solicitar su apertura y deposita los alimentos.

•Una vez los alimentos sean depositados en el locker, uso el troyano de acceso remoto para acceder al sistema del móvil de la víctima y desde allí ingresar a la app y solicitar la liberación del pedido.

•Cuando obtengo el código de liberación se lo informo a mi cómplice y este inmediatamente accede a los alimentos, rápida y cuidadosamente aplica una dosis de la sustancia mortal, cierra el locker y me informa.

•Una vez mi secuaz informa que ha hecho su trabajo, envío un nuevo pedido de liberación, le doy el código y salgo del sistema de la víctima para que este retome el control.

•Mi cómplice usa el nuevo código para abrir y cerrar el locker y se retira rápidamente del lugar




 

