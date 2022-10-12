### MVC

El patrón de arquitectura de **Modelo-Vista-Controlador (MVC)** separa una aplicación en tres componentes principales: Modelo, vista y controlador. El patrón de MVC ayuda a crear aplicaciones que son más fáciles de actualizar y probar que las tradicionales aplicaciones monolíticas.

Las aplicaciones basadas en MVC contienen:

- Modelos: clases que representan los datos de la aplicación. Las clases de modelo usan lógica de validación para aplicar las reglas de negocio para esos datos. Normalmente, los objetos de modelo recuperan y almacenan el estado del modelo en una base de datos. En este tutorial, un modelo Movie recupera datos de películas de una base de datos, los proporciona a la vista o los actualiza. Los datos actualizados se escriben en una base de datos.

- Vistas: Las vistas son los componentes que muestran la interfaz de usuario (IU) de la aplicación. Por lo general, esta interfaz de usuario muestra los datos del modelo.

- Los controladores son clases que:
    - Controlan las solicitudes del explorador.
    - Recuperan datos del modelo.
    - Llaman a plantillas de vista que devuelven una respuesta.



### URL MVC
DOMAIN/CONTROLER/ACTION/ID

ACTION -> Llama a una view
ID -> Puede ser necesaria en alguna Action, para mostrar una view o otra