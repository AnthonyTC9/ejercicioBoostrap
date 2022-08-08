# ejercicioBoostrap
Ejercicio usando boostrap y Sass para la construcción de un sitio estático


se empezo generando los package.json

con npm init -y

se continuo con el video

https://www.youtube.com/watch?v=1kNwZbRiVcQ

que utilizo
npm install bootstrap

se creo una carpeta sass y se creo un documento llamado custom.sass aqui dentro se coloco
@import "../node_modules/bootstrap/scss/bootstrap";
para llamar la biblioteca de boostrap

arriba de dicho documento se incorporaron cambios en css que se ocupaban para el sitio para que los cambios surtan efecto
se instalo sass live el cual abajo a la izquierda se da clic para que observe los cambios de sass y nos cree un css dentro de la misma carpeta
lo ligamos a nuestro index.html con un link y seguiimos editando.

por ultimo se uitlizo
npm i -g purgecss

el cual es un programa que nos ayuda a reducir la cantidad de codigo en nuestro css, para esto
abrimos package.css y editamos la linea del script
"build": "purgecss --css sass/custom.css --content index.html -o css/reducido.css"

se le da un nombre acompañado de la direccion de nuestro css, le decimos que lo compara con lo que necesita nuestro html y despues
le decimos que nos cree uno nuevo en la carpeta css con lo que solo necesita nuestro sitio web.

damos un
npm run build

y listo tenemos purgado nuestro css de codigo que no ocupamos.
