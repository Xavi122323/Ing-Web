Introducción al Framework

La arquitectura de angular on rails permite una poderosa combinación de dos 
frameworks, por un lado, el uso de Angular proporciona diversas herramientas 
para la construcción de estructuras complejas de usuarios, mientras que Rails 
o Ruby on Rails facilita la creación de un backend facilitando la gestión de
tareas, el manejo de la base de datos, la comunicación con un frontend por
medio del enrutamiento y una facilidad en la autenticación.

De igual manera se aprovecha del uso de una API RESTful para facilitar la 
comunicación y el envío de datos entre las capas de la aplicación.


Diseño de Ingeniería

El diagrama se encuentra en:

Ing-Web/Angular on rails.jpg

Los frameworks utilizados permitieron crear un frontend y un backend

En el frontend Rails crea los modelos de los usuarios en base a la información 
proporcionada envía a la creación de estos en la base de datos, en este caso una 
sqlite3, lo interesante de esto es que para el mapeo y el modelo de datos Rails 
solo redirecciona rutas para que la aplicación lea directamente la base de datos 
y de esta manera mapee los datos en base a lo existente en la base

De igual manera los controladores utilizan una fácil interfaz para crear los diversos
métodos que se utilizarán en la API y de igual manera crea una ruta unificada para
poder acceder a estos. De igual manera utiliza un plugin para poder generar
comunicaciones seguras entre el frontend y el backend pudiendo limitar las acciones
que frontend realiza

Finalmente el frontend contiene las vistas y un cliente del backend que al momento
de hacer la conexión llama a los métodos del controlador y por medio del uso de plugin
propios de angular facilita la obtención de los datos, el envío seguro de estos y
la comunicación efectiva con el backend


