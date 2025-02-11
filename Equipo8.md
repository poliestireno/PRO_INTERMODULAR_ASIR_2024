# TFG

## Proyecto intermodular 

Queremos hacer una web que se encuentre alojada en un servidor, en esta web encontraremos toda la información de nuestro club como una 
web cualquiera, pero lo interesante viene cuando puedes iniciar sesión con cuenta de administrador y puedas gráficamente dar de alta, de 
baja a jugadores, cambiar datos, moverlos de equipos, asignar a entrenadores equipos, horarios, etc. Todo esto se tiene que actualizar en 
nuestra base de datos. 

Queremos que a través de una misma web pueda ser informativa para los clientes y funcional para los trabajadores. El objetivo es que a 
través de una misma web puedas gestionar el club. 

ESCUELA DEPORTIVA DE LA SALLE 

Vamos a hacer una web tradicional sobre contenido de la escuela deportiva de la salle, resultados de equipos de otras temporadas, 
información de inscripciones, etc. En la misma web habrá una pestaña para iniciar sesión, habrá diferentes tipos de usuarios con diferentes 
privilegios: 

●  PADRES/JUGADORES: dependiendo de la edad tendrán acceso los padres o los jugadores, a partir de 16 años, tendrán acceso los 

jugadores de las diferentes secciones, podrán ver únicamente información sobre su equipo, próximos partidos, convocatorias, 
información del delegado del equipo para poder escribirle para cualquier problema,etc. 

●  ENTRENADORES: podrán crear, modificar y borrar convocatorias. 
●  JEFES DE SECCIÓN: habrá jefes de sección de cada deporte y por categorías, habrá un jefe de sección por cada 3 categorías: 

○  JEFE DE SECCIÓN DE PREBENJAMÍN, BENJAMÍN Y ALEVÍN 
○  JEFE DE SECCIÓN DE INFANTIL, CADETE Y JUVENIL 
○  JEFE DE SECCIÓN DE SENIOR. 

Podrá hacer lo mismo que el entrenador y además podrá dar de alta, de baja o modificar información de los entrenadores. 

●  DIRECTOR DEPORTIVO: podrá hacer lo mismo que el jefe de sección y además podrá dar de alta, de baja o modificar información de 

los jefes de sección, además podrá dar de alta, de baja o modificar información sobre jugadores, será el encargado de crear y 
gestionar las cuentas de los jugadores/ padres. 

●  PRESIDENTE: podrá hacer lo mismo que el director deportivo, este podrá modificar TODOS los datos de la base de datos. 
●  ADMINISTRADOR: podrá modificar tanto la base de datos al completo como los permisos de los diferentes tipos de usuario, además 

podrá modificar la web. 

 


De esta manera, sin tener que saber modificar bases de datos ya que todo el mundo no tiene conocimientos sobre mariadb o el gestor de base 
de datos que utilicemos. 

Queremos que TODO se pueda hacer a través de la web, de tal manera podremos gestionar de la manera más eficiente posible una escuela 
deportiva con más de 500 alumnos y más de 20 equipos. 

![image](https://github.com/user-attachments/assets/f6b2186b-18c0-435d-a19f-de6c8cabb25a)


Este sería un ejemplo de vistas de la web, lo vemos primero desde la vista de un usuario sin registrar, luego la página para iniciar sesión, 
luego la vista de la cuenta de padres/ jugadores y luego desde la cuenta de administrador. Estos son ejemplos que luego se van a adaptara las 
necesidades que veamos una vez lo vayamos creando. 

Se ha elegido MariaDB como gestor de base de datos porque es fácil de usar, confiable y funciona bien para proyectos web. Permite gestionar 
los datos de forma sencilla usando herramientas como phpMyAdmin, sin necesidad de ser experto en SQL. Además, es una opción eficiente y 
adecuada para manejar la información del club deportivo y sus usuarios. 



Para gestionar el servidor y alojar la aplicación web, se utilizará un servidor como Apache o NGINX, que permita servir los archivos y manejar 
las solicitudes de los usuarios. Durante el desarrollo, se configurará un entorno local con herramientas como XAMPP o Docker, lo que facilitará 
las pruebas y ajustes. Para el despliegue final, se considerará un servicio de hosting como Heroku, AWS o DigitalOcean, asegurando que la 
web esté accesible de forma fiable y con buen rendimiento.
