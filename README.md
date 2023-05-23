#Manual Técnico
1. Sistema/Aplicación
	a. Nombre del sistema
		Sistema de Gestión bibliotecario Web
b. Descripción y delimitación del sistema
Es un sistema encargado de la administración y gestión de información relacionada con los libros, revistas, artículos y otros materiales de la biblioteca, así como información sobre los usuarios, préstamos, reservas y otros aspectos de la gestión de la biblioteca.

Este sistema  podría incluir tablas para almacenar información sobre los libros, como el título, autor, editorial, año de publicación, número de ejemplares, ubicación, categoría, etc. También se puede contar con tablas para almacenar información sobre los usuarios de la biblioteca, como su nombre, dirección, número de identificación, historial de préstamos, multas, etc.
Además, la base de datos podría incluir tablas para almacenar información sobre los préstamos, reservas y devoluciones de los libros, incluyendo la fecha de préstamo, fecha de devolución, nombre del usuario, título del libro, etc. También podría haber tablas para almacenar información sobre las interacciones con los usuarios, como las solicitudes de información, sugerencias y quejas.
c. Objetivo general
Permitir la búsqueda y recuperación eficiente de información de la biblioteca, así como la gestión de préstamos, reservas y devoluciones de libros.
d. Objetivos específicos
Permitir a los usuarios buscar y filtrar los libros ofrecidos por el sistema por género.
Facilitar el proceso de renta de libros.
Mantener un inventario actualizado de los libros disponibles para renta.
De igual forma llevar un control de las multas por retardo al momento de entregar los libros.
e. Descripción de tipos de usuarios
		Público General Registrado
		Público General No Registrado
f. Entorno operativo del sistema
El sistema está diseñado para funcionar como una página web accesible desde los navegadores web comunes. 
2. Especificación de requerimientos
a. Requerimientos funcionales
El sistema debe permitir el registro de nuevos libros con todos los datos correspondientes.
El sistema debe validar que el libro registrado no exista previamente en la base de datos.
El sistema debe permitir a los usuarios registrarse en la página web proporcionando su nombre, apellido, dirección, número de teléfono, correo electrónico y contraseña.
El sistema debe validar que el correo electrónico del usuario sea único.
El sistema debe almacenar la información del usuario en la base de datos.
El sistema debe permitir a los usuarios buscar libros por título o género.
Los usuarios deben poder ver los resultados de búsqueda y seleccionar un libro para obtener más información.
El sistema debe permitir a los usuarios alquilar libros disponibles.
El sistema debe verificar la disponibilidad del libro y registrar el alquiler en la base de datos.
El sistema debe mantener un registro de los libros alquilados por cada usuario.
El sistema debe verificar que el libro se devuelva dentro del tiempo correspondiente y sin daños.
En caso de retraso en la devolución, el sistema debe generar una multa y registrarla en la base de datos.
El sistema debe permitir a los usuarios consultar el estado de sus alquileres y multas asociadas.
Los usuarios deben poder ver una lista de los libros que tienen actualmente y cualquier multa pendiente.
