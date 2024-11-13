# SECCION 2: INSTALACION DE MONGODB

# 9. Desscripcion del modulo

# 10. Instrucciones antes de la instalacion


# 11. Instalando MOngoDB en Windows - Como servicio
# 12. Instalando MOngoDB en Windows - Sin servicio

Cuando instalas MongoDB como un servicio:

    Se ejecuta automáticamente en segundo plano: MongoDB se iniciará automáticamente cada vez que inicies tu sistema operativo (Windows, macOS o Linux), sin necesidad de que ejecutes ningún comando adicional.

    Mayor conveniencia para entornos de producción: Es ideal para servidores y entornos donde necesitas que MongoDB esté siempre disponible y se ejecute automáticamente después de reiniciar el sistema.

    Fácil administración: Puedes controlar el servicio usando comandos del sistema, como systemctl (en Linux) o net start/stop (en Windows).

    Logs y gestión centralizada: MongoDB genera y almacena registros automáticamente en rutas predefinidas, facilitando la supervisión y el análisis de problemas.

Cuando instalas MongoDB sin servicio:

    Ejecución manual: Debes iniciar MongoDB manualmente cada vez que quieras usarlo, ejecutando el comando mongod en tu terminal.

    Mayor control: Es útil para entornos de desarrollo o pruebas, donde no necesitas que MongoDB esté siempre activo.

    No se inicia automáticamente: MongoDB no se ejecutará automáticamente al arrancar el sistema; deberás iniciarlo manualmente cada vez que lo necesites.

    Menos uso de recursos: No consume memoria o CPU cuando no está en uso, ya que solo se ejecuta cuando lo lanzas tú mismo.

Comandos para Conectar al Shell de MongoDB

```bash
mongosh
```

Ver la Base de Datos Actual

```bash
db
```

Listar todas las bases de datos

```bash
show dbs
```

Crear/Usar una Base de Datos: Si la base de datos no existe, se crea automáticamente al insertar un documento.

```bash
use miBaseDeDatos
```

# 13. Instalando MOngoDB en Linux - Linea de comando
# 14. Instalando MOngoDB en Linux - Usando Tarball .tgz

# 15. Instalando MOngoDB en Mac - Linea de comando
# 16. Instalando MongoDB en Mac - Usando Tarball .tgz

# 17. Guia para desinstalar MongoDB

Hola estimado estudiante, para que tengan de conocimiento que en algunos casos necesitamos desinstalar nuestro gestor de base de datos NoSQL MongoDB, para ello MongoDB nos proporciona una guía con una serie de pasos para poder realizar una desinstalación exitosa y es por ello que te comparto el siguiente link donde podrás acceder de manera rápida.

Link: https://www.mongodb.com/basics/uninstall-mongodb