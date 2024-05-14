# PDD - Aplicacion CRUD
Consiste en un sistema el cual puede registrar alumnos, en los cuales estos al momento de ser agregados permiten ser visualizados de manera automatica, tambien dando la opcion de seleccionar y eliminar
Este esta enlazado a una base de datos creada en FireBase

## Patron MVC
Si ha trabajado con React o cualquier otro marco de front-end, o para el caso, cualquier aplicación web lo suficientemente grande, lo más probable es que se haya encontrado con el patrón de diseño MVC. Gracias al diseño del ecosistema de react y a las necesidades de nuestra última aplicación, terminamos implementando el patrón MVC por accidente.
- React (react-native), por sí mismo se conoce como la V en MVC, que significa View. Le ayuda a crear el componente visible de la aplicación.
- Si tiene más de una pantalla, es posible que deba realizar un seguimiento de los datos globales, lo que se puede hacer con algo como FireBase. Esa será la M, que representa el modelo.
- Y, por último, está la C, que representa el controlador. Estas son las interfaces que se exponen a los usuarios para modificar el estado.

[Representacion del comportamientodo de un patron de diseño de MVC](https://www.figma.com/proto/EWuRq2CV2iJQcGm0abNZXc/Untitled?node-id=2-2&starting-point-node-id=2%3A2&show-proto-sidebar=1&t=QTBFbmwyrey2OWvB-1)

### Funcion
La aplicacion tiene una pagina de inicio donde puedes agregar a un alumno a la lista.
Cuando este haga clic, se pedira sus datos(nombre, apellido y matricula), al momento de ser ingresados, esto se refleja en el inicio
Puedes todos los alumnos en la lista registrados
Seleccionas uno y te despliega la informacion que contiene este, y tambien con la opcion de borrar

Ahora, ese es el ciclo completo del patrón MVC. Como puedes ver, hay tres componentes. En primer lugar, están las vistas que se muestran al usuario. Luego están los controladores como el botón que afecta al estado global, el modelo. Y, por último, está el modelo que afecta a la vista de la segunda página, como resultado de haber sido alterado por el controlador.

![1_D65HaJVw7DaHQ9SEV4Ux6Q (1)](https://github.com/GabrielHernandezZam/PDD/assets/112035117/b05ef184-b1c4-4a07-a5f4-00222b648ba7)
