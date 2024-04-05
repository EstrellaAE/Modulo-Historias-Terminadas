# Integradora II
[![Contribuidores][contribuidores-shield]][contributors-url]

## contenido
<details>
  <summary>Tabla contenidos</summary>
  <ol>
    <li>
      <a href="#acerca-del-proyecto">Acerca del Proyecto</a>
      <ul>
        <li><a href="#descripción">Descripción</a></li>
        <li><a href="#objetivos">Objetivos</a></li>
        <li><a href="#organigrama">Organigrama</a></li>
        <li><a href="#diagrama-gantt">Diagrama Gantt</a></li>
      </ul>
    </li>
    <li>
      <a href="#análisis-de-la-solución">Análisis de la Solución</a>
      <ul>
        <li><a href="#requerimientos">Requerimientos</a></li>
        <li><a href="#diagrama-casos-de-uso">Diagrama de Casos de Uso</a></li>
      </ul>
    </li>
    <li>
      <a href="#diseño-de-la-solución">Diseño de la Solución</a>
      <ul>
        <li><a href="#modelo-relacional">Modelo Relacional</a></li>
        <li><a href="#diagrama-de-clases">Diagrama de Clases</a></li>
        <li><a href="#diagrama-de-componentes">Diagrama de Componentes</a></li>
      </ul>
    </li>    
    <li>
      <a href="#implementación">Implementación</a>
      <ul>
        <li><a href="#estándares-codificación">Estándares Codificación</a></li>
        <li><a href="#arquitectura">Arquitectura</a></li>
        <li><a href="#código-fuente">Código Fuente</a></li>
      </ul>
    </li>      
    <li>
      <a href="#pruebas">Pruebas</a>
      <ul>
        <li><a href="#casos-de-prueba">Casos de prueba</a></li>
        <li><a href="#ejecución">Ejecución</a></li>
      </ul>
    </li>       
    <li><a href="#guias">Guias</a></li>
    <li><a href="#contribucion">Contribución</a></li>
    <li><a href="#licencia">licencia</a></li>
    <li><a href="#contacto">Contacto</a></li>
    <li><a href="#participantes">Participantes</a></li>
  </ol>
</details>

<!-- Acerca del proyecto -->
## Acerca del proyecto
Requisitos.
El proyecto implicó la implementación de un módulo para asignar fechas de liberación a los informes que han sido concluidos. La liberación de los informes se lleva a cabo agrupándolos por el nombre del sistema.

<!-- Descripción -->
#### Descripción.
La descripción del proyecto abarcó el desarrollo de un módulo para asignar fechas de liberación a los informes que estaban completos y preparados para avanzar al siguiente módulo. Además, se integró un filtro para buscar estos informes utilizando diversos campos. Una vez que se asignaba una fecha de liberación a una historia, ésta se agrupaba por sistema y dejaba de mostrarse dentro del módulo de historias terminadas, otorgándole un estado para su liberación completa. El proyecto se enfocó en cumplir con los requisitos de tiempo, costo y calidad establecidos por los stakeholders.

En cuanto al tiempo, el proyecto requirió casi cuatro meses para su finalización, considerando los diversos requisitos y el esfuerzo dedicado al mismo. Este período se vio influenciado por la dedicación del equipo, que trabajó de manera comprometida y realizó una planificación y ejecución efectiva del proyecto.

En relación con la calidad, se buscó entregar un trabajo que ofreciera funcionalidad, usabilidad y fiabilidad dentro del módulo desarrollado. El objetivo era satisfacer los requerimientos y expectativas establecidos, asegurando que el módulo cumpliera con todos los aspectos solicitados y garantizando su correcto funcionamiento.

<!-- Objetivos -->
#### Objetivos.
Indicar los objetivos del proyecto.
Se desarrolló e implementó un módulo de asignación de fechas de liberación para reportes concluidos con funcionalidad, usabilidad y fiabilidad óptimas. Este módulo cumple con los requerimientos solicitados y las expectativas del cliente, garantizando una gestión eficiente y ordenada de los reportes por sistema. Además, se integró un sistema de filtrado de datos para facilitar y agilizar la búsqueda de los reportes deseados.

<!-- Organigrama -->
#### Organigrama.
Organigrama.
![Organigrama](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/commit/f4edd06e1ced2a3a951762dd9a62f8d402133ad2)

<!-- Diagrama Gantt -->
#### Diagrama Gantt.
Diagrama Gantt.


<!-- Análisis del proyecto -->
## Análisis de la Solución.
En esta sección se detallan los artefactos generados como parte de la solución. El desarrollo e implementación del módulo de asignación de fechas de liberación para reportes concluidos implicó la creación de varios artefactos clave para el éxito del proyecto.

Se generó una descripción detallada de las características principales del módulo, como la asignación de fechas de liberación, la agrupación por sistema y la implementación de un filtro de búsqueda. Además, se elaboró un diseño de interfaz de usuario del módulo, priorizando la usabilidad y la experiencia del usuario.

La implementación del módulo se llevó a cabo conforme a los requisitos y el diseño establecidos, asegurando una integración fluida y coherente con el sistema existente. Se realizaron pruebas exhaustivas para garantizar la calidad y fiabilidad del módulo, identificando y corrigiendo cualquier error o fallo detectado durante este proceso. Este enfoque permitió asegurar un funcionamiento adecuado del módulo antes de su despliegue y uso en producción.

<!-- Requerimientos -->
#### Requerimientos.
Listado de los requerimientos (código requerimiento, descripción)
REQ-01: La aplicación muestra una lista de todas las historias de usuario, título de historia, asunto, grupo y sistema.

REQ-02: La aplicación muestra una lista de las historias de usuario que están en estado "terminado", con su título y sistema.

REQ-03: La aplicación permite al usuario seleccionar las historias de usuario que quiere liberar mediante un checkbox.

REQ-04: La aplicación agrupa las historias de usuario por sistema en el listado de historias de usuario terminadas.

REQ-05: La aplicación permite al usuario asignar una fecha de liberación a las historias de usuario que ha seleccionado

REQ-06: La aplicación guarda la fecha de liberación y la historia de usuario en la base de datos

REQ-07: Se crea una nueva tabla en la base de datos para almacenar la información de las historias de usuario que se desean liberar, con los campos título, sistema, fecha de liberación y estado.

<!-- Diagrama de Casos de Uso -->
#### Diagrama Casos de Uso.
Agregar la imagen de los Casos de Uso.



<!-- Diseño del proyecto -->
## Diseño de la Solución.
En ésta sección se indicarán los artefactos generados en base a la solución.
Se implementará una arquitectura basada en microservicios para garantizar la escalabilidad y la flexibilidad del sistema.

Asignación de Fechas:Asignación de fechas de liberación a los reportes concluidos.
Agrupación por Sistema:Agrupar los reportes por el nombre del sistema al que pertenecen.
Búsqueda:Proporciona funcionalidades de búsqueda para encontrar reportes utilizando diferentes criterios.
Interfaz de Usuario: La interfaz de usuario será una aplicación web que permitirá a los usuarios interactuar con el sistema de manera intuitiva.

<!-- Modelo Relacional -->
#### Modelo Relacional.
Esquema de la base de datos (nombre de campo, tipo de datos, restricciones, etc)


<!-- Diagrama de Clases -->
#### Diagrama de Clases.
Esquema de las clases empleadas (atributos y sus métodos).



<!-- Diagrama de Componentes -->
#### Diagrama de Componentes.
Esquema de los componentes que interactúan (Modelo, Vista, Controlador, Servidor Web, Servidor de base de datos)


<!-- Implementación del proyecto -->
## Implementación.
En ésta sección se describen  los artefactos generados en base a la solución.
Para llevar a cabo la implementación del módulo de asignación de fechas de liberación que fue nuestra parte para desarrollar y en base a los requerimientos que se brindaron implementamos la solución que propusimos logrando así lo siguiente.

Se solicitaba la asignación de fechas, logrando la implantación de un botón que realizará esta acción dando como resultado cuando se seleccione una o varias historias se pueda asignar su fecha y esto a su vez genera el estatus de espera esto para pasar a el siguiente módulo y obtener un status distinto.
Para poder asignar fechas de liberación de los reportes se solicitó que fueran agrupados, para poder lograr esto hacemos que todos los que coincidieran con el nombre del sistema al momento de seleccionarlos se agruparan y agilice el procedimiento.
Para poder agilizar la asignación de fecha de liberación se implementó un filtro donde podemos buscar la prueba por sus diferentes campos que contiene y hacer su identificación más fácil.

<!-- Estándares de Codificación -->
#### Estándares de Codificación.
Estándares empleados en la codificación
Convenciones de Nomenclatura Consistentes:

Utiliza nombres descriptivos y significativos para las tablas, columnas, procedimientos almacenados y otros objetos de la base de datos.
Consistente con la capitalización y la estructura de los nombres. Por ejemplo, camelCase o snake_case.
Evita abreviaturas poco claras o ambiguas. Prioriza la claridad sobre la brevedad.
Documentación Clara:

Documenta el propósito, la estructura y el funcionamiento de cada tabla y procedimiento almacenado.
Proporciona comentarios en el código SQL para explicar la lógica detrás de consultas complejas o partes críticas del código.
Utiliza herramientas de documentación de bases de datos si es posible para mantener la documentación actualizada y accesible.
Normalización de Datos:

Diseña la estructura de la base de datos de acuerdo con los principios de normalización para minimizar la redundancia y mantener la integridad de los datos.
Divide la información en tablas relacionadas de manera lógica, evitando la duplicación de datos siempre que sea posible.
Utiliza claves primarias y foráneas para establecer relaciones entre las tablas y mantener la coherencia de los datos.
Pruebas Exhaustivas:

Realiza pruebas unitarias para cada consulta SQL y procedimiento almacenado para garantizar que funcionen según lo esperado.
Considera casos de prueba que cubran diferentes escenarios, como datos válidos e inválidos, condiciones de error y casos límite.
Utiliza conjuntos de datos de prueba representativos para evaluar el rendimiento y la escalabilidad del código SQL.
Además de estos estándares generales, aquí hay algunas prácticas recomendadas específicas para definir tablas y procedimientos almacenados:

Definición de Tablas:

Utiliza claves primarias para identificar de manera única cada registro en una tabla.
Define claves foráneas para establecer relaciones entre tablas y garantizar la integridad referencial.
Asegúrate de asignar los tipos de datos apropiados a cada columna para optimizar el almacenamiento y garantizar la consistencia de los datos.
Evalúa y revisa periódicamente la estructura de las tablas para asegurarte de que sigan siendo adecuadas para las necesidades del sistema.
Definición de Procedimientos Almacenados:

Divide la lógica de negocio en procedimientos almacenados modulares y reutilizables para mejorar la mantenibilidad y la legibilidad del código.
Utiliza parámetros de entrada y salida para comunicarte con el procedimiento almacenado desde otras partes de la aplicación.
Implementa manejo de errores para capturar y gestionar excepciones de manera adecuada, proporcionando mensajes claros y significativos en caso de fallo.
Realiza pruebas exhaustivas del procedimiento almacenado en un entorno de desarrollo antes de implementarlo en producción.

<!-- Arquitectura MVC y Middleware -->
#### Arquitectura.
Definir los patrones empleados y de seguridad.

<!-- Código Fuente -->
#### Código Fuente.
Código Fuente de la solución


<!-- Pruebas proyecto -->
## Pruebas.
En ésta sección se describen los artefactos generados en base a la solución.

<!-- Casos de prueba -->
#### Casos de prueba.
Indicar los casos de prueba


<!-- Ejecución Casos de prueba -->
#### Ejecución.
Evidencia de Ejecución de Casos de prueba.


<!-- Iniciando -->
## Iniciando
Iniciando.

<!-- Requisitos -->
### Requisitos
Requisitos de Instalación.

<!-- Instalación -->
### Instalacion
Instalación del Software


## Guias
Guias de Uso.

## contribucion
Contribucion.

## Licencia
Licencia.

## Contacto
Contacto.

## Participantes
* [participante 1]()
* [participante 2]()
* [participante 3]()

[contribuidores-shield]: https://img.shields.io/github/contributors/github_username/repo_name.svg?style=for-the-badge
[contributors-url]: https://github.com/github_username/repo_name/graphs/contributors

