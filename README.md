## Para poder ejecutar este curd es necesario seguir estos pasos

1. Crear un contenedor de mysql con el siguiente comando:

    ``` 
        podman pull docker.io/library/mysql:latest
    ```

    ```
        podman run --name mysql-container -e MYSQL_ROOT_PASSWORD=root -p 3306:3306 -d mysql:latest
    ```

    ```
        podman exec -it mi_mysql mysql -u root -p
    ```

2. Crear una base de datos con el nombre user

3. Importante este crud es un crud api basico creado con Spring boot y Java 17, por lo que es necesario tener instalado Java 11 y maven para poder ejecutarlo

4. Para ejecutar el crud es necesario ejecutar el siguiente comando en la carpeta del proyecto:
    ```
       mvn spring-boot:run
    ```
   o desde el archivo ApiAppplication

5. Esta api es una api basica que permite crear, actualizar, eliminar y listar usuarios, para poder probarla es necesario tener instalado postman o insomnia

6. Y su proposito es poder realizar pruebas de Automatizacion con Serenity y Screenplay conectando con la base de datos creada en el paso 1
   
