# SECCION 3: INTRODUCCION A MONGODB SHELL

# 18. Descripcion del modulo

# 19. Accediendo a mongosh Help

Con mongosh --help obtendremos una descripcion general de los parametros y opciones que podemos usar con mongosh. Mongosh es la MongoDBShell moderna, que es una herramienta para interactuar con base de datos MongoDB desde la linea de comandos.

Opciones basicas

    mongosh --host: Especifica el nombre del servidor de MongoDB
    mongosh --port: Define el puerto en el que escucha el servidor MongoDB
    mongosh --username: Usuario para la autenticacion
    mongosh --password: contraseña correspondiente
    mongosh --version: muestra la versión actual de mongosh

Para interactuar con la BD primero ejecutar mongosh:

mongosh: Se conecta al servidor MongoDB que este configurado de manera predeterminada

Una vez iniciada mongosh podemos usar:

    help: muestra una ayuda general
    db.help(): Muestra una ayuda relacionada con las operaciones en una base de datos
    show dbs: Lista todas las base de datos disponibles en el servidor MongoDB
    db.getName(); Se utiliza para obtener el nombre de la base de datos actual en la que está conectado mongosh

# 20. Configurando Mongod y Mongosh

db.shutdownServer(): Apagar el servidor. Se debe ejecutar el comando desde la base de datos admin.
use nombre_de_base_de_datos: Crea o usa una bd especifica.

Entonces luego de apagar el servidor, previamente cambiandonos a bd admin, vamos a correr el servidor en otro puerto con el siguiente comando:

    "C:\Program Files\MongoDB\Server\7.0\bin\mongod.exe" --dbpath="c:\data\db" --port 27018

Luego le tenemos que indicar que mongosh debe conectarse tambien a ese puerto:

    mongosh --port 27018: Con esto ya nos permitira conectarnos.

Si otra vez apagamos el servidor y queremos correrle en ese mismo puerto poner:

    "C:\Program Files\MongoDB\Server\7.0\bin\mongod.exe" --dbpath="c:\data\db"

Y luego ponemos mongosh

# 21. Shell vs Drivers en MongoDB

Los drivers son bibliotecas oficiales que permiten a las aplicaciones (escritas en diferentes lenguajes de programación) conectarse y comunicarse con una base de datos MongoDB.

MongoDB proporciona drivers oficiales para los lenguajes más utilizados, como:

        Node.js (mongodb driver)
        Python (PyMongo)
        Java (MongoDB Java Driver)
        C#/.NET (MongoDB .NET Driver)
        Go (MongoDB Go Driver)
        PHP (MongoDB PHP Library)