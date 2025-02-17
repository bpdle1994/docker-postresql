# Docker-PostgreSQL

## Verificacion de la instalacion de postgre y la descarga de imagen

Se ejecuta los comandos para verificar la instalacion y version junto a la descarga de imagen de postgre

**Comando para verificar la instalacion**

~~~sql
docker --version
~~~

![Imagen de ejemplo](Captura1.png)

**Comando para descargar la imagen**

~~~sql
docker pull postgre
~~~

![Imagen de ejemplo](Captura2.png)

## Crear y ejecutar un contenedor con PostgreSQL

Ejecutar los comandos para crear y ejecutar el contenedor

**Comando para verificar la instalacion**

~~~sql
docker run --name mi_postgres -e POSTGRES_USER=admin -e POSTGRES_PASSWORD=admin123 -e POSTGRES_DB=mi_base -p 5432:5432 -d postgres
~~~

![Imagen de ejemplo](Captura3.png)

## Conectarse a PostgreSQL dentro del contenedor y crear la tabla "Estudiante"

Conexion a postgreSQL dentro del contenedor

**Comando para verificar la instalacion**

~~~sql
docker exec -it mi_postgres psql -U admin -d mi_base
~~~

![Imagen de ejemplo](Captura4.png)

Creacion de la tabla

![Imagen de ejemplo](Captura5.png)

Verificar que la tabla fue creada correctamente

![Imagen de ejemplo](Captura6.png)

## Insertar y consultar datos

Insercion de estudiante     

![Imagen de ejemplo](Captura7.png)

![Imagen de ejemplo](Captura8.png)

Consulta de datos

![Imagen de ejemplo](Captura9.png)

## Salir y detener el contenedor

Para salir de PostgreSQL:

![Imagen de ejemplo](Captura10.png)

Para detener el contenedor:

![Imagen de ejemplo](Captura11.png)

Para iniciarlo nuevamente:

![Imagen de ejemplo](Captura12.png)
