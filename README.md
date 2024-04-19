# Integradora II
[![Contribuidores][contribuidores-shield]][contributors-url]

## Contenido
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
El proyecto abarcó el desarrollo de un módulo para asignar fechas de liberación a los reportes que estaban completos y preparados para avanzar al siguiente módulo. Además, se integró un filtro para buscar estos reportes utilizando diversos campos. Una vez que se asignaba una fecha de liberación a una historia, ésta se agrupaba por sistema y dejaba de mostrarse dentro del módulo de historias terminadas, asignándole un estado para su liberación completa. El proyecto se enfocó en cumplir con los requisitos de tiempo, costo y calidad establecidos.
En cuanto al tiempo, el proyecto requirió un total de cuatro meses para su finalización. La metodología utilizada fue una combinación de enfoques ágiles y tradicionales, adaptándose a las necesidades del equipo y del proyecto. Esta estrategia permitió una planificación eficaz y una ejecución fluida para concluir el trabajo de manera exitosa.

Los riesgos identificados durante el proyecto incluyeron posibles cambios en los requisitos del cliente, la complejidad de implementar el procedimiento almacenado ya que era muy
difícil mandarlo llamar desde el modulo y posibles demoras en la disponibilidad de recursos clave como la activacion de la herramienta FortiClient VPN.

El equipo estuvo compuesto por seis integrantes, cada uno con roles específicos:
- Eduardo Antonio Zapatero Arellano, scrum master: Responsable de la coordinación general del equipo, gestión de riesgos y comunicación con el cliente.
- Juan David Lara Robles, administrador de Base de Datos: Responsable de garantizar una buena integridad y disponibilidad de los datos necesarios para el proyecto.
- Juan Diego Juárez Cruz desarrollador: Encargada del desarrollo e implementación del módulo y incluyendo el filtro de búsqueda.
- Valeria Gómez Herrera, desarrollador: Encargada de la lógica de asignación de fechas.
- Estrella Guadalupe Aguayo Exiga, desarrollador: Encargada de el diseño del modulo.

Los interesados del proyecto incluyo el departamento de tecnología de la información de la empresa NAD Global, quienes se encargaron de proporcionar el soporte técnico necesario.

<!-- Objetivos -->
#### Objetivos.
Se ha desarrollado e implementado un módulo de asignación de fechas de liberación para reportes concluidos con funcionalidad, usabilidad y fiabilidad óptimas. Este módulo cumple cabalmente con los requerimientos solicitados y las expectativas del cliente, asegurando una gestión eficiente y organizada de los reportes por sistema. Además, se ha integrado un sistema de filtrado de datos que facilita y agiliza la búsqueda de reportes específicos dentro del sistema implementado.Satisfacer los requerimientos y expectativas establecidos, asegurando que el módulo cumpliera con todos los aspectos solicitados y garantizando su correcto funcionamiento.

<!-- Organigrama -->
#### Organigrama.
![Organigrama](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Organigrama.png)

<!-- Diagrama Gantt -->
#### Diagrama Gantt.
![Diagrama de Gantt imagen 1](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Diagrama%20de%20Gantt%201.png)
![Diagrama de Gantt imagen 2](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Diagrama%20de%20Gantt%202.png)

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

#### Historias de usuario.
Historias de usuario: https://docs.google.com/document/d/1e4j0NltUpJdYK0rq6DVgfddsS8wkJzx16AcxFAEEpwc/edit?usp=sharing

#### Pantallas de historias de usuario.
Pantallas de Historias de usuario: https://docs.google.com/document/d/1SRFEF85qDJ02bDKS9VtaBucjzcFMeil-DgA21s_NusA/edit?usp=sharing

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
![Diagrama de Clases](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Diagrama%20de%20clases%20correcto.jfif)

<!-- Diagrama de Componentes -->
#### Diagrama de Componentes.
![Diagrama de Componentes](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Diagrama%20de%20componentes%20correcto.jfif)

#### Diagrama de Actividades.
![Diagrama de Actividades](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Diagrama%20de%20actividades%20correcto.jfif)

<!-- Implementación del proyecto -->
## Implementación.
Para llevar a cabo la implementación del módulo de asignación de fechas de liberación, se procedió a desarrollar la solución propuesta basada en los requerimientos proporcionados. Esta solución logró satisfacer los siguientes objetivos:

- Se implementó un botón que permite la asignación de fechas de liberación. Al seleccionar una o varias historias, este botón ejecuta la acción de asignar la fecha y cambia el estado de las historias a "en espera", lo que facilita el paso al siguiente módulo y obtención de un estado diferente.

- Para cumplir con la solicitud de agrupar los reportes por el nombre del sistema, se diseñó la funcionalidad de manera que al seleccionar los reportes, estos se agrupen automáticamente según el nombre del sistema al que pertenecen. Esto agiliza el procedimiento de asignación de fechas al organizar los reportes de manera coherente.

- Para mejorar la eficiencia en la asignación de fechas de liberación, se implementó un filtro que permite buscar los reportes por diversos campos. Esto facilita la identificación de los reportes deseados y agiliza el proceso de asignación de fechas.

<!-- Estándares de Codificación -->
#### Estándares de Codificación.
Estandares de Codificaciòn de base de datos: https://docs.google.com/document/d/1i8lkzp329RRrHhN9hIkFhgoltLPJIAxOIOccSPy1zXg/edit?usp=sharing
Estandares Javascript y .Net Framework: https://docs.google.com/document/d/1yUMDuFzVtQsiRzHWV5bTI9Qao3p5AIYmlPoXGbe6Klc/edit?usp=sharing

#### Arquitectura.
![Modelo Vista Controlador](https://github.com/EstrellaAE/Modulo-Historias-Terminadas/blob/main/Modelo%20MVC.jfif)
<!-- Código Fuente -->
#### Código Fuente.
Por cuestiones de seguridad no es posible compartir el código.

## Pruebas.
Casos de prueba: https://docs.google.com/spreadsheets/d/1rm5fZNyM01lEzEqW5YG1JWtt0OtXT_vShMChDIZJvJg/edit#gid=0

<!-- Ejecución Casos de prueba -->
#### Ejecución.
Ejecucion casos de prueba: https://docs.google.com/spreadsheets/d/1_GUFwyHRhuaTdsvuYjla47tF713eRp2D0bjfbRRNe2k/edit?usp=sharing

#### Pantallas de ejecución.
Pantallas de ejecucion: https://docs.google.com/document/d/1PXNEGHfd-5-TQ8t6OqIqN0PIE4DvRMl8fvbbqXu38xE/edit?usp=sharing

<!-- Requisitos -->
### Requisitos
*SQL
*FortiClient VPN
*Visual Studio
*TortoiseSVN

<!-- Instalación -->
### Instalacion
Instalacion: https://docs.google.com/document/d/1R7yIIpENt73me5Ao57PzQnjkfDK5Owm0YOTF9qOCZAU/edit

## Participantes
* Estrella Guadalupe Aguayo Exiga
* Juan Diego Juárez Cruz
* Valeria Gómez Herrera
* Juan David Lara Robles
* Eduardo Antonio Zapatero Arellano

[contribuidores-shield]: https://img.shields.io/github/contributors/github_username/repo_name.svg?style=for-the-badge
[contributors-url]: https://github.com/github_username/repo_name/graphs/contributors

