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
El proyecto implicó la implementación de un módulo para asignar fechas de liberación a los reportes que han sido concluidos. La liberación de los reportes se lleva a cabo agrupándolos por el nombre del sistema.

<!-- Descripción -->
#### Descripción.
El proyecto abarcó el desarrollo de un módulo para asignar fechas de liberación a los reportes que estaban completos y preparados para avanzar al siguiente módulo. Además, se integró un filtro para buscar estos reportes utilizando diversos campos. Una vez que se asignaba una fecha de liberación a una historia, ésta se agrupaba por sistema y dejaba de mostrarse dentro del módulo de historias terminadas, asignadole un estado para su liberación completa. El proyecto se enfocó en cumplir con los requisitos de tiempo, costo y calidad establecidos.
En cuanto al tiempo, el proyecto requirió casi cuatro meses para su finalización, considerando los diversos requisitos y el esfuerzo dedicado al mismo. Este período se vio influenciado por la dedicación del equipo, que trabajó de manera comprometida y realizó una planificación y ejecución efectiva del proyecto.
Se buscó entregar un trabajo que ofreciera funcionalidad, usabilidad y fiabilidad dentro del módulo desarrollado. El objetivo era satisfacer los requerimientos y expectativas establecidos, asegurando que el módulo cumpliera con todos los aspectos solicitados y garantizando su correcto funcionamiento.

<!-- Objetivos -->
#### Objetivos.
Se ha desarrollado e implementado un módulo de asignación de fechas de liberación para reportes concluidos con funcionalidad, usabilidad y fiabilidad óptimas. Este módulo cumple cabalmente con los requerimientos solicitados y las expectativas del cliente, asegurando una gestión eficiente y organizada de los reportes por sistema. Además, se ha integrado un sistema de filtrado de datos que facilita y agiliza la búsqueda de reportes específicos dentro del sistema implementado.

<!-- Organigrama -->
#### Organigrama.
![Organigrama](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Organigrama1.png)

<!-- Diagrama Gantt -->
#### Diagrama Gantt.
![Diagrama de Gantt](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Captura%20de%20pantalla%202024-04-04%20231108.png)

<!-- Análisis del proyecto -->
## Análisis de la Solución.
Se generó una descripción detallada de las características principales del módulo, como la asignación de fechas de liberación, la agrupación por sistema y la implementación de un filtro de búsqueda. Se elaboró un diseño de interfaz de usuario del módulo,con usabilidad y la experiencia del usuario.
La implementación del módulo se llevó a cabo conforme a los requisitos y el diseño establecidos, asegurando una integración fluida y coherente con el sistema existente. Se realizaron pruebas  para garantizar la calidad y fiabilidad del módulo, identificando y corrigiendo cualquier error o fallo detectado durante este proceso. Este enfoque permitió asegurar un funcionamiento adecuado del módulo antes de su despliegue y uso en producción.

<!-- Requerimientos -->
#### Requerimientos.
REQ-01: La aplicación muestra una lista de todas las historias de usuario, título de historia, asunto, grupo y sistema.

REQ-02: La aplicación muestra una lista de las historias de usuario que están en estado "terminado", con su título y sistema.

REQ-03: La aplicación permite al usuario seleccionar las historias de usuario que quiere liberar mediante un checkbox.

REQ-04: La aplicación agrupa las historias de usuario por sistema en el listado de historias de usuario terminadas.

REQ-05: La aplicación permite al usuario asignar una fecha de liberación a las historias de usuario que ha seleccionado

REQ-06: La aplicación guarda la fecha de liberación y la historia de usuario en la base de datos

REQ-07: Se crea una nueva tabla en la base de datos para almacenar la información de las historias de usuario que se desean liberar, con los campos título, sistema, fecha de liberación y estado.

<!-- Diagrama de Casos de Uso -->
#### Diagrama Casos de Uso.
![Diagrama de caso de Uso](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Historias%20terminadas.png)
![Imagen 1](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Caso%20de%20uso%201.png)
![Imagen 2](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Caso%20de%20uso%202.png)
![Imagen 3](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Caso%20de%20uso%203.png)

<!-- Diseño del proyecto -->
## Diseño de la Solución.
Se implementará una arquitectura basada en microservicios para garantizar la escalabilidad y flexibilidad del sistema.
El primer microservicio se encargará de la asignación de fechas, permitiendo la asignación de fechas de liberación a los reportes concluidos. Otro microservicio estará dedicado a la agrupación por sistema, facilitando la organización de los reportes según el nombre del sistema al que pertenecen. Además, se desarrollará un microservicio específico para la funcionalidad de búsqueda, ofreciendo a los usuarios la capacidad de encontrar reportes utilizando diferentes criterios.
Se diseñará un modulo que permitirá a los usuarios interactuar con el sistema de manera intuitiva. Esta interfaz proporcionará una experiencia de usuario fluida y amigable, facilitando la navegación y utilización de las diferentes funcionalidades ofrecidas por los microservicios.

<!-- Modelo Relacional -->
#### Modelo Relacional.
![Modelo Relacional](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Modelo%20Relacional.png)

<!-- Diagrama de Clases -->
#### Diagrama de Clases.
![Diagrama de Clases](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Diagrama%20de%20Clases.png)

<!-- Diagrama de Componentes -->
#### Diagrama de Componentes.
![Diagrama de Componentes](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Diagrama%20de%20componentes.jfif)

<!-- Implementación del proyecto -->
## Implementación.
Para llevar a cabo la implementación del módulo de asignación de fechas de liberación, se procedió a desarrollar la solución propuesta basada en los requerimientos proporcionados. Esta solución logró satisfacer los siguientes objetivos:

- Se implementó un botón que permite la asignación de fechas de liberación. Al seleccionar una o varias historias, este botón ejecuta la acción de asignar la fecha y cambia el estado de las historias a "en espera", lo que facilita el paso al siguiente módulo y obtención de un estado diferente.

- Para cumplir con la solicitud de agrupar los reportes por el nombre del sistema, se diseñó la funcionalidad de manera que al seleccionar los reportes, estos se agrupen automáticamente según el nombre del sistema al que pertenecen. Esto agiliza el procedimiento de asignación de fechas al organizar los reportes de manera coherente.

- Para mejorar la eficiencia en la asignación de fechas de liberación, se implementó un filtro que permite buscar los reportes por diversos campos. Esto facilita la identificación de los reportes deseados y agiliza el proceso de asignación de fechas.

<!-- Estándares de Codificación -->
#### Estándares de Codificación.
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
![Modelo Vista Controlador](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Modelo%20MVC.jfif)
<!-- Código Fuente -->
#### Código Fuente.
Código Fuente de la solución


<!-- Pruebas proyecto -->
## Pruebas.
En ésta sección se describen los artefactos generados en base a la solución.

<!-- Casos de prueba -->
#### Casos de prueba.
![Imagen 1](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Caso%20de%20prueba%201.png)
![Imagen 2](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Caso%20de%20prueba%202.png)

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
* Estrella Guadalupe Aguayo Exiga
* Juan Diego Juárez Cruz
* Valeria Gómez Herrera
* Juan David Lara Robles
* Eduardo Antonio Zapatero Arellano

[contribuidores-shield]: https://img.shields.io/github/contributors/github_username/repo_name.svg?style=for-the-badge
[contributors-url]: https://github.com/github_username/repo_name/graphs/contributors

