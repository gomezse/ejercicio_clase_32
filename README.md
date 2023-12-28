# ejercicio_clase_32
Mocking y manejo de errores 
Para testear desde el FRONT

    ejecutar http://localhost:8080/api/sessions/signout (limpiar cookies);
    acceder al signup : "http://localhost:8080/signup";
    registrarte de manera local
    una vez generado el user acceder a "http://localhost:8080/login"
    loguearse con el mail y password del item 3
    esto arrojara el msj con el token generado.
 

***Mocking hecho en el endpoint (100 productos) --> http://localhost:8080/api/products/mockingproducts

Archivos involucrados:
 - faker.js
 - products-router.js
 - product.controller.js
 

***Manejo de errores
Por ejemplo ingresando mal la contraseña en el login, puede verse el error customizado en pantalla.

Carpeta errors creada con archivos:

- error.enum.js
- error.generator.js

Middleware error: errors.middleware.js

Archivos en los cuales se incluyó el uso de errores customizados:
- cart.controller.js
- product.controller.js
- sessions.controller.js