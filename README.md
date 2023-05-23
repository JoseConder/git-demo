# Sistema de Gestión bibliotecario Web

## Descripción

El Sistema de Gestión bibliotecario Web es un sistema encargado de la administración y gestión de información relacionada con los libros, revistas, artículos y otros materiales de la biblioteca, así como información sobre los usuarios, préstamos, reservas y otros aspectos de la gestión de la biblioteca.

## Objetivo

El objetivo principal de este sistema es permitir la búsqueda y recuperación eficiente de información de la biblioteca, así como la gestión de préstamos, reservas y devoluciones de libros.

## Objetivos específicos

- Permitir a los usuarios buscar y filtrar los libros ofrecidos por el sistema por género.
- Facilitar el proceso de renta de libros.
- Mantener un inventario actualizado de los libros disponibles para renta.
- Llevar un control de las multas por retardo al momento de entregar los libros.

## Tipos de usuarios

El sistema cuenta con los siguientes tipos de usuarios:

- Público General Registrado
- Público General No Registrado

## Requerimientos

El sistema cumple con los siguientes requerimientos funcionales:

- Permite el registro de nuevos libros con todos los datos correspondientes.
- Valida que el libro registrado no exista previamente en la base de datos.
- Permite a los usuarios registrarse en la página web proporcionando su nombre, apellido, dirección, número de teléfono, correo electrónico y contraseña.
- Valida que el correo electrónico del usuario sea único.
- Almacena la información del usuario en la base de datos.
- Permite a los usuarios buscar libros por título o género.
- Permite ver los resultados de búsqueda y seleccionar un libro para obtener más información.
- Permite a los usuarios alquilar libros disponibles.
- Verifica la disponibilidad del libro y registra el alquiler en la base de datos.
- Mantiene un registro de los libros alquilados por cada usuario.
- Verifica que el libro se devuelva dentro del tiempo correspondiente y sin daños.
- Genera multas y las registra en la base de datos en caso de retraso en la devolución.
- Permite a los usuarios consultar el estado de sus alquileres y multas asociadas.
- Permite ver una lista de los libros que tienen actualmente y cualquier multa pendiente.

# Sistema de Gestión bibliotecario Web

## Descripción

El Sistema de Gestión bibliotecario Web es un sistema encargado de la administración y gestión de información relacionada con los libros, revistas, artículos y otros materiales de la biblioteca, así como información sobre los usuarios, préstamos, reservas y otros aspectos de la gestión de la biblioteca.

## Objetivo

El objetivo principal de este sistema es permitir la búsqueda y recuperación eficiente de información de la biblioteca, así como la gestión de préstamos, reservas y devoluciones de libros.

## Objetivos específicos

- Permitir a los usuarios buscar y filtrar los libros ofrecidos por el sistema por género.
- Facilitar el proceso de renta de libros.
- Mantener un inventario actualizado de los libros disponibles para renta.
- Llevar un control de las multas por retardo al momento de entregar los libros.

## Tipos de usuarios

El sistema cuenta con los siguientes tipos de usuarios:

- Público General Registrado
- Público General No Registrado

## Requerimientos no funcionales

El sistema debe cumplir con los siguientes requerimientos no funcionales:

- Capacidad de manejar grandes volúmenes de datos de forma eficiente y con tiempos de respuesta rápidos.
- Tiempo de respuesta aceptable para consultas y operaciones en la base de datos, garantizando una experiencia de usuario fluida.
- Garantizar la seguridad de los datos almacenados en la base de datos, evitando el acceso no autorizado, la modificación o eliminación indebida de información.
- Implementación de un mecanismo de copias de seguridad y recuperación de la base de datos para garantizar la disponibilidad de los datos en caso de fallas.
- Disponibilidad del sistema las 24 horas del día, los 7 días de la semana, para que los usuarios puedan acceder en cualquier momento.
- Medidas para minimizar el tiempo de inactividad planificado o no planificado, como mantenimiento programado y redundancia de servidores.
- Confiabilidad y disponibilidad del sistema, evitando interrupciones o fallas frecuentes.
- Gestión adecuada de errores y excepciones para minimizar las interrupciones en el funcionamiento normal.

## Arquitectura del Sistema/Aplicación

### Layer/Tier's

El sistema se divide en las siguientes capas o tiers:

- Capa de Presentación (Frontend): Esta capa se encarga de la interfaz de usuario y la interacción con el usuario. Está compuesta por tecnologías web como HTML, CSS y JavaScript, utilizando el framework Materialize CSS para el diseño visual y la interfaz responsiva. Aquí se encuentra la página de inicio, la búsqueda de libros, los detalles del libro, las órdenes y las multas.

- Capa de Aplicación (Backend): Esta capa maneja la lógica de negocio y la funcionalidad de la aplicación. Utiliza Node.js como entorno de ejecución de JavaScript y Express como framework web para el enrutamiento y la gestión de las solicitudes HTTP. Se encarga de manejar las solicitudes del usuario, procesar la lógica de la aplicación y realizar operaciones en la base de datos.

- Capa de Datos (Backend): Esta capa se conecta a la base de datos Oracle utilizando el paquete `oracledb` de Node.js. Se encarga de realizar consultas y actualizaciones en la base de datos, recuperar y almacenar la información relacionada con los usuarios, los libros, las órdenes y las multas.

### Frontend/Backend

El frontend de la aplicación utiliza tecnologías web como HTML, CSS y JavaScript para la interfaz de usuario y la interacción con el usuario. Se emplea el framework Materialize CSS para un diseño visual atractivo y una interfaz responsiva.

El backend de la aplicación utiliza Node.js y Express para manejar las solicitudes del usuario, procesar la lógica de la aplicación y realizar operaciones en la base de datos Oracle. También se utiliza el paquete `oracledb` para interactuar con la base de datos y realizar consultas y actualizaciones.

### Estructura modular del sistema

La estructura modular del sistema sigue un enfoque MVC (Modelo-Vista-Controlador) o similar, donde los componentes del sistema están organizados en módulos y siguen un patrón de separación de responsabilidades. Algunos módulos son los siguientes:

- Módulo de Autenticación: Maneja el registro de usuarios, el inicio de sesión y la gestión de sesiones.
- Módulo de Búsqueda y Filtrado: Permite a los usuarios buscar libros por nombre y filtrar por categorías.
- Módulo de Gestión de Libros: Maneja las operaciones relacionadas con los libros, como obtener detalles, actualizar el stock, etc.
- Módulo de Órdenes de Préstamo: Gestiona la generación de órdenes de préstamo, verificación de stock, fechas de préstamo y caducidad, etc.
- Módulo de Seguimiento de Órdenes: Permite a los usuarios ver el estado de sus préstamos y actualizar el estado de las órdenes (entregado, multa pendiente, etc.).
- Módulo de Multas: Maneja la generación y visualización de multas, así como su estado y pagos.


