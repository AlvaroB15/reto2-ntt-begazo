# reto2-ntt-begazo

Los repos del reto 2 son

Backend:

```https://github.com/AlvaroB15/ms-users-reto2```
```https://github.com/AlvaroB15/ms-login-reto2```

Frontend:

```https://github.com/AlvaroB15/angular18-reto2```

Endpoints publicos 

Frontend
```https://admirable-beijinho-3e3a3b.netlify.app/login```

Microservicios

Endpoint de registrar y listar usuarios```https://ms-users-reto2-production.up.railway.app/api```

Endpoint de login
```https://ms-login-reto2-production.up.railway.app/api```

Tener instalado la v18 de node (o usar un nvm, fnm, u otro manejador de versiones de node)
Tener instalado docker y docker-compose (o usar el docker compose up -d, el cual es el mas actualizado y propio de docker y ya no la dependencia de docker-compose)

Luego de clonar solo debe correr

```shell
docker compose up -docker
// O la alternativa antigua
docker-compose up -d
```

Agregare una carpeta de docker y docker-compose.yml, solo necesita clonar los 2 proyetos backend en la raiz de este mismo repo, al hacer eso, podra correr ambos contenedores de forma local, y expuestos en el puerto 8081 y 8082


/POST
http://localhost:8082/api/login
```
{
"email": "pc3presi@gmail.com",
"password": "Asd123456@"
}
```


/POST
http://localhost:8081/api/register
```
{
  "fullName":"Pedro castillo 3",
  "email": "pc6presi@gmail.com",
  "password": "Asd123456@",
  "phone": "999999999"
}
```


/GET http://localhost:8081/api/users
El token se genera al realizar el login, debe reemplazar el de ejemplo de abajo
```
token: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJwYzJwcmVzaUBnbWFpbC5jb20iLCJpYXQiOjE3MzU5NTU5NDcsImV4cCI6MTczNTk1NjAzNH0.hXvIpuEVCur2fw3PxhOOBhUsTgAFMfpOhGUdrI6o03s
```


Para las pruebas 
```maven test```
Por si no tiene instalado maven puede usar
```./mvnw test```


