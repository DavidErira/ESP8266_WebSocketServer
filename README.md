# ESP8266-WebSockets

Este programa corre sobre un ESP8266 mas no sobre un ESP32, se utilizó un sensor mpu6050 para experimentar con un sensor, pero puede funcionar de la misma forma con cualquier otro dato.

Tener en cuenta que no tiene programado un servidor HTTP para servir un codigo de front-end, se puede conectar al ESP mediante la dirección IP que le asiga la red wifi, esta programado en modo STA.


## Comenzando 🚀

Se programa el manejador de eventos del socket en esta función
![visualización](https://raw.githubusercontent.com/DavidErira/ESP8266_WebSocketServer/master/ME.png)
Se le puede programar que hacer en cada evento, cuando se conecta, desconecta o recibe un mensaje

Se programó en caso de recibir un mensaje "ON" un codigo y en caso de recibir un mensaje "OF" otro codigo
![visualización](https://raw.githubusercontent.com/DavidErira/ESP8266_WebSocketServer/master/ONOF.png)
Lo que le permite saber cuando enviar o cancelar el envío de datos,

Para envíar datos se utiliza esta porción de codigo, en donde se establece cada cuento se enviaría un dato, en este caso establecido en 100ms 
![visualización](https://raw.githubusercontent.com/DavidErira/ESP8266_WebSocketServer/master/envio.png)

### Funcionamiento 📋
Se debe establecer la red wifi a la que se requiere conectar
Usar la IP asignada para establecer la conexión
Enviar "ON" al ESP para que empiece hacer envío de sus datos
Enviar "OFF" al ESP para que cancele el envío de sus datos

Se puede modificar la frecuencia con la cual se quiere enviar datos, actualmente establecida en 100ms


## Autor
 ✒️
* **David Erira** - *Desarrollo* - [DEEM](https://github.com/DavidErira)


* Comenta a otros sobre este proyecto 📢



---
⌨️ con ❤️ por [DEEM](https://github.com/DavidErira) 😊
