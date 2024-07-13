# nestNotas
notas de nodejs

# comando para crear un proyecto de nestjs
```nest g res nombre```  =>  para crear todo un recurso de un servicio de nestjs

# comando para crear un servicio de nestjs
```nest g s nombre```  =>  para crear un servicio de nestjs

# conectores de mongo para nests
 se debe intalar este paquete para nest
-- $ npm i @nestjs/mongoose mongoose



# creacion de conteendores en doker


### configuracion del conyeemdor se dene crear el archivo dentro del proyecto 
  ```docker-compose.yalm   ``` - para la configuracion de la imagen del archivo 
  configuracion de la imagen de mongo
  ```yalm
version: '3'
services:
  db:
    image: mongo:5
    restart: always
    ports:
      - 27017:27017
    environment:
      MONGODB_DATABASE: nest-pokemon
    volumes:
      - ./mongo:/data/db   ```

# este comando ejecuta el contenedor de mongo
    ```docker-compose up -d```      