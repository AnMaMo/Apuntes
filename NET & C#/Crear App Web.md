#### Que son los paquetes NuGet
Una herramienta esencial para cualquier plataforma de desarrollo moderno, es un mecanismo a través del cual los desarrolladores pueden crear, compartir y consumir código útil. A menudo, este código se integra en "paquetes" que contienen código compilado (como archivos DLL) y otro contenido necesario en los proyectos que utilizan estos paquetes.
(Lo que viene a ser Maven o Graddle en JAVA un gestor de dependencias para usar codigo y caracteristicas hechas por otros programadores).


### Que es Scaffolding
En Visual Studio existe una funcionalidad llamada "Scaffolding" que permite crear pantallas de edición, visualización, creación y eliminación de los registros de la base de datos. En un par de clics tienes montada la típica pantalla de mantenimiento de una tabla.
(Basicamente creando un scaffolding de un modelo en c# puedes crear automaticamente un controlador que se encarga de gestionar las paginas (views) de "Create, Read, Update y Delete (CRUD)", generadas automaticamente. Para trabajar con una tabla de la base de datos).


### Migracion base de datos
Las migraciones son un conjunto de herramientas que crean y actualizan una base de datos para que coincida con el modelo de datos.


### Instancia DbContext
Una instancia de DbContext representa una sesión con la base de datos y se puede usar para consultar y guardar instancias de las entidades. DbContext es una combinación de los patrones Unit Of Work y Repository.


### Codigo Asincrono
Un servidor web tiene un número limitado de subprocesos disponibles y, en situaciones de carga alta, es posible que todos los subprocesos disponibles estén en uso. Cuando esto ocurre, el servidor no puede procesar nuevas solicitudes hasta que los subprocesos se liberen. Con el código sincrónico, se pueden acumular muchos subprocesos mientras no estén realizando ningún trabajo porque están a la espera de que finalice la E/S. Con el código asincrónico, cuando un proceso está a la espera de que finalice la E/S, se libera su subproceso para el que el servidor lo use para el procesamiento de otras solicitudes. Como resultado, el código asincrónico permite que los recursos de servidor se usen de forma más eficaz, y el servidor está habilitado para administrar más tráfico sin retrasos.