# Base-de-datos-SQL_Universidad


Desde la universidad del dato nos han solicitado una base de datos para almacenar la información referente a las asignaturas, alumnos, profesores y los cursos.


Cada curso se identifica por un código (1,2,3,4,5 y 6) y tiene un nombre descriptivo asignado (primero, segundo, tercero, cuarto, máster, doctorado). Asimismo, nos interesa saber el número de asignaturas del curso.


En cada curso hay varias asignaturas, que se identifican por un código numérico. Además, cada asignatura tiene nombre, número de créditos, número de cuatrimestre en que se imparte (1 ó 2) y el carácter (obligatoria u optativa).


Un profesor puede impartir varias asignaturas, como mínimo una. Y una asignatura puede ser impartida por profesores diferentes. Todas las asignaturas tienen un profesor coordinador (no todos los profesores son coordinadores). Cada profesor se identifica por un código que le asigna la universidad, aunque también podría ser identificado por su NIF. También se guarda de cada profesor su nombre, apellidos, teléfonos de contacto, dirección postal y dirección electrónica, así como la categoría, una de las siguientes:
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


Los alumnos pueden matricularse en varias asignaturas. Dentro de la categoría de asignaturas optativas, podría ocurrir que alguna asignatura no tuviera ningún alumno matriculado. Cada uno de los alumnos se identifica por un código que le asigna la universidad, aunque también se puede identificar alternativamente por su NIF. Además, de cada alumno se debe guardar su nombre y apellidos y sus direcciones postal y electrónica. Por último, también se desea saber para cada alumno si tiene beca o no. No necesitamos conocer el tipo o la cuantía de la beca, sólo si tiene o no. Además, nos gustaría saber la nota del alumno en cada una de las asignaturas.
