# Rails 6 con postgresql

Para correr el proyecto, debemos agregar dos archivos adicionales.
El primero es `.env` y el segundo `.env.postgresql`

Las variables de entorno para agregar en `.env` son:

```
DB_USER=postgres
DB_PASSWORD=123456
DB_HOST=db
```

Y las variables para el archivo `.env.postgresql` son:

```
POSTGRES_PASSWORD=123456
POSTGRES_USER=postgres
```

Luego de agregar estas variables, debemos construir los containers con docker compose, con los siguientes comandos

```
#Para construir los containers
docker-compose build

#Para levantar los containers
docker-compose up

#Para dejar los containers corriendo en segundo plano
docker-compose up -d
```
