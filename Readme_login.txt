El login planteado funciona mediante el uso de un plugin llamado devise, este
nos permite administrar el ingreso por medio del backend, de esta manera esta
herramienta nos ayuda encriptando las claves y por medio de un JWT (JSON Web Token)
que se envía entre el frontend y backend para asegurar los enlaces al igual
que juntar a cada usuario con su respectivo token.

Ing-Web/Login Diagram.png

En nuestro diagrama en primer lugar comenzamos con el registro del usuario, nuestro 
frontend al recibir el email y contraseña los envía al frontend y este valida que 
sean validos los almacena en la base de datos y lo junta a un token JWT y mientras 
que el frontend guarda el token localmente y en caso de reenviar la solicitud para 
regresar al login se suprime el token y de igual manera el frontend lo elimina localmente.

Mientras tanto en caso de un sign in se envía de igual manera desde el frontend las 
credenciales del usuario y estas son validadas en nuestro backend, una vez hecho esto 
si comprueba que son validos se remite el token que es almacenado localmente en el 
login, una vez realizado este proceso se permite el ingreso a la aplicación y que se 
puedan realizar las operaciones de la aplicación.