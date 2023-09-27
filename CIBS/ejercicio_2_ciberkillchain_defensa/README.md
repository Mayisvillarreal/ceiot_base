# Ejercicio CiberKillChain - Defensa

## Alumno

María Claudia Villarreal Ardila

## Enunciado

Desarrollar la defensa en función del ataque planteado en orden inverso.

Para cada etapa elegir una sola defensa, la más importante, considerar recursos limitados.

## Resolución

7.	Actions on Objectives
•	Envío el pedido de liberación para que el locker abra, inmediatamente mi secuaz, vestido como domiciliario para no levantar sospechas, accede a los alimentos, rápida y cuidadosamente aplica una dosis de la sustancia mortal y escapa. Solicito un nuevo código de apertura del locker, para que este sea marcado como ocupado y la víctima obtenga el código de liberación.

Defensa: 
El equipo de vigilancia privada del edificio cuenta con una persona que revisa los videos de las cámaras de seguridad, prestando especial atención a la zona de lockers, el vigilante se percata de que un domiciliario accede a un compartimiento que había sido abierto minutos antes, esto no corresponde al funcionamiento normal del sistema, por lo cual alerta a los residentes, informado que sus domicilios pudieron ser manipulados.

6.	Command & Control
•	Envío a uno de mis secuaces a un lugar cercano a los lockers para que pueda observar cuando el mensajero deje el domicilio, yo alisto mi dispositivo y minutos después de que me sea notificada la apertura de un locker para dejar un paquete, accedo a la aplicación e ingreso a la herramienta, y mediante esta, a la App que controla la apertura de los lockers.
Una vez los alimentos sean depositados, espero a que mi cómplice se encuentre en posición para enviar el pedido de liberación

Defensa: TBD

5. Installation • (T1577) Compromise Application Executable: Se abre el sitio web desde el cual se descarga la herramienta de administración remota y esta se instala en el dispositivo de la víctima.

Defensa: (T1474.002) Supply Chain Compromise: Compromise Hardware Supply Chain.
https://attack.mitre.org/techniques/T1474/002/
La víctima realiza actualizaciones de seguridad constantemente, una de estas contiene un parche para los mecanismos de verificación de integridad que detecta la modificación de hardware no autorizada y bloquea su instalación.

4. Exploit • El objetivo abre el correo electrónico y da click en el link malicioso

Defensa: La víctima lee el correo electrónico pero antes de dar click en el link revisa el destinatario y nota que no es el mismo que usa normalmente la administración del edificio, por lo que decide eliminar el correo electrónico.

3. Delivery • (T1456) Drive-By Compromise: Envío al correo electrónico del objetivo un mensaje para inscribirse a una rifa que se realizará entre los residentes del edificio, este contiene un link a un sitio web para descargar la herramienta mencionada en el punto anterior

Defensa: TBD

2. Weaponization
• Puedo usar phishing buscando que la víctima revele las credenciales de acceso a la App
• Decido instalar una herramienta de administración remota en el dispositivo de la víctima, que me permita acceder a este en el momento correcto

Defensa: TBD

Reconnaissance 
• Espías detectan que el objetivo usa frecuentemente el sistema de control de apertura de lockers para recibir alimentos a domicilio.
• (T1589) Gather Victim Identity Information: Se recurre a la miembros de la administración del edificio fingiendo ser una empresa de lavandería para acceder al correo electrónico del objetivo y de otros residentes 
• (T1598)Phishing for Information: Se usa principalmente para obtener información de otros residentes del edificio sobre la app del sistema de control de apertura de lockers.

Defensa:
• (M1017)User Training: 
Los miembros de la administración y los residentes del edificio han participado en capacitaciones para identificar intentos de phishing, por lo tanto no revelan el correo electrónico del objetivo.



