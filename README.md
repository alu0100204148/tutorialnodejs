# Tutorial Node.js

##Que es node.js

>Node.js es un entorno de programación en la capa del servidor basado en el lenguaje de programación ECMAScript, asíncrono, con I/O de datos en una arquitectura orientada a eventos y basado en el motor V8 de Google. 
Fue creado con el enfoque de ser útil en la creación de programas de red altamente escalables, como por ejemplo, servidores web.



##Instalación en Win7

>Para instalar en windows simplemente habrá que descargar el programa de la pagina web de [node.js], ejecutaremos el instalador y seguiremos los pasos que nos indica el asistente, indicándole la carpeta en la que queremos que se instale.



##Funcionamiento

>Para comprobar su funcionamiento crearemos un fichero de nombre example.js.

>###example.js


```
var http = require('http');
http.createServer(function (req, res) {
	res.writeHead(200, {'Content-Type': 'text/plain'});
	res.end('Hello World\n');
}).listen(1337, '127.0.0.1');
console.log('Server running at http://127.0.0.1:1337/');
 ```


>Para arrancar el node.js, tan solo deberemos buscar el acceso directo en el menú Inicio de windows y ejecutarlo. Aparecerá una ventana, la cual deberá permanecer abierta.

>Posteriormente abriremos una consola de comandos, escribiendo cmd en el campo buscar del menú inicio.

>Nos situaremos en la carpeta en la que se encuentra nuestro fichero de ejemplo example.js, y escribiremos node example.js ejecutándolo. Debería aparecer el siguiente texto.



![Texto alternativo](captura1.png "captura1")




>Para comprobar que está funcionando realmente, deberemos abrir un explorador web y escribir en la barra de direcciones http://127.0.0.0.1:1337, que corresponde al localhost y al puerto que hemos determinado anteriormente en nuestro fichero. Si todo funciona correctamente el servidor deberá respondernos con un "Hello World".




![Texto alternativo](captura2.png "captura2")





[node.js]:http://nodejs.org
