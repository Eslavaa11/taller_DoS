==========================================================
TALLER DE ATAQUES DoS Y SERVIDOR
Autor: Andres Eslava
==========================================================

Proyecto realizado en Unity para el taller sobre ataques
DoS con muchas peticiones.  
El objetivo fue entender cómo funcionan las peticiones
masivas a un servidor y cómo se puede simular una sobrecarga
de tráfico de manera controlada con fines educativos.

----------------------------------------------------------
1. FUNCIONAMIENTO GENERAL
----------------------------------------------------------
La aplicación envía varias peticiones al mismo tiempo hacia
una dirección de servidor definida en el campo de texto.
El propósito no es dañar, sino mostrar cómo una gran
cantidad de solicitudes pueden afectar la respuesta del
servidor.

El usuario puede escribir la URL del servidor y ejecutar el
envío de peticiones desde Unity.  
En la consola se muestra la respuesta de cada intento y el
comportamiento general del sistema.

----------------------------------------------------------
2. CÓDIGO PRINCIPAL
----------------------------------------------------------
El código fue escrito en C# dentro de Unity usando la clase
UnityWebRequest, que permite hacer peticiones HTTP desde la
aplicación.

Cada petición se ejecuta en una corrutina (IEnumerator),
lo que permite lanzar varias solicitudes seguidas sin
bloquear la aplicación.

El proceso general es:
1. El usuario ingresa la URL del servidor.
2. Se envía una cantidad de solicitudes repetidas.
3. Se observa cómo responde el servidor al exceso de tráfico.

----------------------------------------------------------
3. OBJETIVO
----------------------------------------------------------
El taller busca mostrar el impacto que puede tener un
ataque DoS y cómo prevenirlo en la práctica real.  
Se aprende cómo funcionan las conexiones cliente-servidor
y cómo una mala configuración o falta de control puede
afectar la estabilidad del sistema.

----------------------------------------------------------
4. INTERFAZ
----------------------------------------------------------
La interfaz de Unity tiene un campo para ingresar la URL
del servidor y un botón para iniciar las pruebas.  
También muestra los mensajes de estado o errores en la
consola para que el usuario pueda analizar los resultados.

----------------------------------------------------------
5. CONCLUSIÓN
----------------------------------------------------------
Este taller permitió comprender de manera práctica los
principios básicos de un ataque DoS y la importancia de
proteger los servidores ante solicitudes excesivas.
Todo el código fue hecho a mano, simple y entendible,
enfocado únicamente con fines de aprendizaje.
