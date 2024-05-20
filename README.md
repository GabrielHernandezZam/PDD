# PDD - Aplicacion CRUD
Consiste en un sistema el cual puede registrar alumnos, en los cuales estos al momento de ser agregados permiten ser visualizados de manera automatica, tambien dando la opcion de seleccionar y eliminar
Este esta enlazado a una base de datos creada en FireBase

### Funcion
La aplicacion tiene una pagina de inicio donde puedes agregar a un alumno a la lista.
Cuando este haga clic, se pedira sus datos(nombre, apellido y matricula), al momento de ser ingresados, esto se refleja en el inicio
Puedes todos los alumnos en la lista registrados
Seleccionas uno y te despliega la informacion que contiene este, y tambien con la opcion de borrar


## Patrones de Diseño Utilizados:
1. **Modelo-Vista-Controlador (MVC)**:
   - Se emplea en la organización general de la aplicación, donde los componentes representan tanto el modelo (datos del alumno), la vista (interfaz de usuario) y el controlador (lógica de negocio y manejo de interacciones).
   - ![1_D65HaJVw7DaHQ9SEV4Ux6Q (1)](https://github.com/GabrielHernandezZam/PDD/assets/112035117/b05ef184-b1c4-4a07-a5f4-00222b648ba7)

2. **Inyección de Dependencias**:
   - Se aplica al importar la instancia de Firebase (`appFirebase`) en varios componentes, lo que facilita la modularidad y testabilidad del código.

3. **Patrón de Navegación**:
   - Se utiliza React Navigation para gestionar la navegación entre las diferentes pantallas de la aplicación, proporcionando una experiencia de usuario fluida y coherente.

4. **Singleton**:
   - El modelo de "Inicialización Única" (Singleton) se emplea para inicializar la aplicación de Firebase (`appFirebase`) una sola vez, garantizando que solo exista una instancia de la aplicación a lo largo de toda la ejecución del programa. Esto evita la inicialización redundante y asegura la coherencia en el uso de la aplicación de Firebase en toda la aplicación.

5. **Modelo de Componentes**:
   - La aplicación sigue el modelo de componentes, donde cada pantalla (ListaAlumno, CreateAlum, ShowAlum) y sus elementos (botones, campos de entrada, etc.) se representan como componentes independientes y reutilizables. Esto promueve la modularidad, la reutilización y la claridad en la estructura del código.

### Funcionalidad del Sistema:
- **Listado de Alumnos**: La aplicación muestra una lista de alumnos, cada uno con su nombre, apellido y matrícula.
- **Agregar Alumno**: Permite agregar un nuevo alumno proporcionando su nombre, apellido y matrícula.
- **Eliminar Alumno**: Permite eliminar un alumno de la lista.
- **Mostrar Detalles del Alumno**: Permite ver los detalles de un alumno específico, incluyendo su nombre, apellido y matrícula.
