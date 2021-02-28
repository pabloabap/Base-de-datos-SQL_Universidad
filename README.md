# Base-de-datos-SQL_Universidad

## Introducción


Desde la universidad del dato nos han solicitado una base de datos para almacenar la información referente a las asignaturas, alumnos, profesores y los cursos.


Cada **curso** se identifica por un código (1,2,3,4,5 y 6) y tiene un nombre descriptivo asignado (primero, segundo, tercero, cuarto, máster, doctorado). Asimismo, nos interesa saber el número de asignaturas del curso.


En cada curso hay varias **asignaturas**, que se identifican por un código numérico. Además, cada asignatura tiene nombre, número de créditos, número de cuatrimestre en que se imparte (1 ó 2) y el carácter (obligatoria u optativa).


Un **profesor** puede impartir varias asignaturas, como mínimo una. Y una asignatura puede ser impartida por profesores diferentes. Todas las asignaturas tienen un profesor coordinador (no todos los profesores son coordinadores). Cada profesor se identifica por un código que le asigna la universidad, aunque también podría ser identificado por su NIF. También se guarda de cada profesor su nombre, apellidos, teléfonos de contacto, dirección postal y dirección electrónica, así como la categoría, una de las siguientes:
* Catedráticos de Universidad
* Titulares Universidad
* Catedráticos de Escuela Universitaria
* Titulares de Escuela Universitaria
* Eméritos
* Contratados Doctores
* Contratados Doctores Interinos
* Asociados
* Asociado Interino
* Ayudantes Doctores
* Otros Investigadores Doctores
* PDI predoctoral


Queremos saber el curso académico en que se imparten las asignaturas.


Los **alumnos** pueden matricularse en varias asignaturas. Dentro de la categoría de asignaturas optativas, podría ocurrir que alguna asignatura no tuviera ningún alumno matriculado. Cada uno de los alumnos se identifica por un código que le asigna la universidad, aunque también se puede identificar alternativamente por su NIF. Además, de cada alumno se debe guardar su nombre y apellidos y sus direcciones postal y electrónica. Por último, también se desea saber para cada alumno si tiene beca o no. No necesitamos conocer el tipo o la cuantía de la beca, sólo si tiene o no. Además, nos gustaría saber la nota del alumno en cada una de las asignaturas.

## Pasos a seguir

### 1. Diseño conceptual ([BBDDUniverdidad_Diseño conceptual])
Para saber cómo estructurar la base de datos haremos un diagrama con las entidades, sus atributos y sus relaciones.


### 2. Diseño lógico ([BBDDUniversidad_Diseño lógico])
Definida la estructura la convertiremos en un modelo relacional de tablas.

### 3. Creación de la base de datos, las tablas y la carga de datos  ([BBDDUniversidad.sql] - Lineas 1 - 2019])
Con código SQL crearemos toda la estructura que albergará los datos.
La carga de datos la haremos de forma manual en en las tablas de curso, profesor, asignatura y matrícula; y con importaciones de ficheros las tablas de alumno, tlfContactoPRof e impartir

### 4. Consultas ([BBDDUniversidad.sql] - Líneas 2022 - 2128)

Las consultas realizadas será:
* Caracter, nº de alumnos, nota mínima, máxima y media de las asignaturas. Ordenar el resultado por curso primero y nombre de la asignatura después.
* Asignaturas con una nota media inferior a 5 orden por curso y posteriormente por nombre ascendente.
* Conocer el número de profesores por categoría y ordenar la tabla de categoría con más profesores a categoría con menos.
* Conocer curso, asignatura, carácter de la asignatura, coordinador y e-mail de contacto.
* Asignaturas impartidas por profesor de más a menos.
* Mostrar aquellos alumnos que tienen una media superior a 7.00 y su nota media.
* Obtener los créditos totales por curso y carácter de la asignatura. El curso 6 tiene 0 créditos, al ser un doctorado las asignaturas no forman parte de la nota final.
* Obtener aquellas optativas sin alumnos.
* Obtener el número de alumnos de primero que tienen que recuperar cada asignatura.
* Alumnos que tienen que presentarse a la recuperación de Algebra lineal y la nota que sacaron.
* Alumnos de segundo que han sacado un 10 en alguna materia para ponerles mención de honor. Ordenar alfabéticamente por nombre asignatura.
* Conocer número de alumnos totales, los becados y porcentaje de becados respecto al total.
* Conocer nota media de los becados y el curso en el que están. Ordenar resultado alfabeticamente por nombre completo.
* Queremos repartir un bonus a los 10 profesores con mejores medias en las asignaturas que imparten.
* Obtener toda la información de asignaturas que contienen los caracteres 'datos' o 'progra' en su nombre. Ordenar por curso y luego por nombre.
* Obtener listado para enviar un comunicado oficial personalizado con el nombre a todas las personas de la universidad (alumnos y profesores). 


[BBDDUniverdidad_Diseño conceptual]: https://github.com/pabloabap/Base-de-datos-SQL_Universidad/blob/main/BBDDUnviersidad_Dise%C3%B1o%20conceptual.pdf
[BBDDUniversidad_Diseño lógico]: https://github.com/pabloabap/Base-de-datos-SQL_Universidad/blob/main/BBDDUnviersidad_Dise%C3%B1o%20l%C3%B3gico.pdf
[BBDDUniversidad.sql]: https://github.com/pabloabap/Base-de-datos-SQL_Universidad/blob/main/BBDDUniversidad.sql


