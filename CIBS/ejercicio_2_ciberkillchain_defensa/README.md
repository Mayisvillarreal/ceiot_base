# Ejercicio CiberKillChain - Defensa

## Alumno

María Claudia Villarreal Ardila

## Enunciado

Desarrollar la defensa en función del ataque planteado en orden inverso.

Para cada etapa elegir una sola defensa, la más importante, considerar recursos limitados.

## Resolución

7.	Actions on Objectives

Mi secuaz debe informarme si un domiciliario se acerca al locker de la víctima, realiza la llamada para solicitar su apertura y deposita los alimentos.

Una vez los alimentos sean depositados en el locker, uso el troyano de acceso remoto para acceder al sistema del móvil de la víctima y desde allí ingresar a la app y solicitar la liberación del pedido.

Cuando obtengo el código de liberación se lo informo a mi cómplice y este inmediatamente accede a los alimentos, rápida y cuidadosamente aplica una dosis de la sustancia mortal, cierra el locker y me informa.

Una vez mi secuaz informa que ha hecho su trabajo, envío un nuevo pedido de liberación, le doy el código y salgo del sistema de la víctima para que este retome el control.

Mi cómplice usa el nuevo código para abrir y cerrar el locker y se retira rápidamente del lugar.


Defensa: 

• (DS0042)Interfaz de usuario: La víctima detecta un funcionamiento anormal en su teléfono y decide investigar
Técnica: https://attack.mitre.org/datasources/DS0042/

•El equipo de vigilancia privada del edificio cuenta con una persona que revisa los videos de las cámaras de seguridad, prestando especial atención a la zona de lockers, el vigilante se percata de que un domiciliario accede a un compartimiento que había sido abierto minutos antes, esto no corresponde al funcionamiento normal del sistema, por lo cual alerta a los residentes, informado que sus domicilios pudieron ser manipulados.

6.	Command & Control

•	Uno de mis secuaces se ubica en un lugar cercano a los lockers con un teléfono celular desde el cual se comunica conmigo.
•	Alisto mi dispositivo para acceder al sistema del teléfono de la víctima mediante el Troyano de acceso remoto


Defensa: TBD

5. Installation

 • (T1577) Compromise Application Executable: Se abre el sitio web desde el cual se descarga la herramienta de administración remota y esta se instala en el dispositivo de la víctima.

Defensa: (T1474.002) Supply Chain Compromise: Compromise Hardware Supply Chain.
https://attack.mitre.org/techniques/T1474/002/
La víctima realiza actualizaciones de seguridad constantemente, una de estas contiene un parche para los mecanismos de verificación de integridad que detecta la modificación de hardware no autorizada y bloquea su instalación.

4. Exploit

• El objetivo abre el correo electrónico y da click en el link malicioso

Defensa: La víctima lee el correo electrónico pero antes de dar click en el link revisa el destinatario y nota que no es el mismo que usa normalmente la administración del edificio, por lo que decide eliminar el correo electrónico.

3. Delivery

• (T1456) Drive-By Compromise: Envío al correo electrónico del objetivo un mensaje para inscribirse a una rifa que se realizará entre los residentes del edificio, este contiene un link a un sitio web para descargar la herramienta mencionada en el punto anterior

Defensa: 

•La víctima abre el correo electrónico desde su computador y el malware está diseñado para actuar sobre Android 
•La víctima no abre el correo electrónico por ser de un remitente desconocido.

2. Weaponization
 
• Puedo usar phishing buscando que la víctima revele las credenciales de acceso a la App

• Decido instalar una herramienta de administración remota en el dispositivo de la víctima, que me permita acceder a este en el momento correcto

Defensa: TBD

1. Reconnaissance 
• Espías detectan que el objetivo usa frecuentemente el sistema de control de apertura de lockers para recibir alimentos a domicilio.
• (T1589) Gather Victim Identity Information: Se recurre a la miembros de la administración del edificio fingiendo ser una empresa de lavandería para acceder al correo electrónico del objetivo y de otros residentes 
• (T1598)Phishing for Information: Se usa principalmente para obtener información de otros residentes del edificio sobre la app del sistema de control de apertura de lockers.

Defensa:
• (M1017)User Training: 
Los miembros de la administración y los residentes del edificio han participado en capacitaciones para identificar intentos de phishing, por lo tanto no revelan el correo electrónico del objetivo.



