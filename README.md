# Documentación Técnica - Aula Virtual

![Portada del proyecto](./imagenes%20Documentacion/portada.jpg)

**Título del Proyecto**: Aula Virtual con Tailwind CSS  
**Integrantes del Equipo**:

- Lucas Chacón - Rol diseñador y programador
- Lucas Sánchez - Rol diseñador y programador
  
**Fecha de Entrega**: 16/02/2025

---

## Índice

1. [Introducción](#introducción)
2. [Arquitectura del Proyecto](#arquitectura-del-proyecto)
3. [Diseño del Proyecto](#diseño-del-proyecto)
4. [Tecnologías Utilizadas](#tecnologías-utilizadas)
5. [Integración de Contenido Multimedia](#integración-de-contenido-multimedia)
6. [Responsividad y Accesibilidad](#responsividad-y-accesibilidad)
7. [Desafíos y Soluciones](#desafíos-y-soluciones)
8. [Conclusión](#conclusión)



---

## Introducción

### Descripción del aula virtual

El proyecto de Aula Virtual es una aplicación web realizada con Tailwind CSS, un framework que ayuda a crear interfaces de usuario de manera rápida y eficiente mediante el uso de clases predefinidas. Este framework permite diseñar componentes visuales de forma flexible y personalizable sin necesidad de escribir mucho código CSS desde cero.

La aplicación está orientada a facilitar la interacción de los estudiantes con el aula, proporcionando un entorno digital donde se pueden compartir materiales educativos, realizar evaluaciones, y mantener un seguimiento constante del curso. Además, se ha implementado una estructura de navegación intuitiva, accesible desde diferentes dispositivos, para asegurar que los usuarios tengan una experiencia cómoda y funcional.

Entre las principales características de este Aula Virtual se encuentran la gestión de tareas, la visualización de notas, un calendario, seguimiento activo del curso y el acceso a contenidos multimedia siendo inclusivo para personas con visión reducida. El uso de Tailwind CSS garantiza un diseño limpio, moderno y completamente responsive, adaptándose a cualquier tamaño de pantalla para una mejor usabilidad en móviles, tablets y formato escritorio.

El aula virtual trata sobre diferentes asignaturas de matemáticas y nos vamos a enfocar en la de Álgebra.

### Objetivos del Proyecto

- Desarrollar una plataforma fácil de usar para la gestión de cursos.
- Implementar un diseño responsive y accesible para todos los dispositivos.
- Facilitar la interacción de estudiantes con el aula.
- Integrar un sistema de gestión de tareas y exámenes con retroalimentación automática.
- Proporcionar una interfaz intuitiva para la navegación y visualización de contenidos educativos.
- Incorporar funcionalidades de seguimiento de progreso de los estudiantes a través de gráficos y estadísticas.
- Facilitar la creación y gestión de materiales educativos, como presentaciones, documentos y videos.
- Asegurar la compatibilidad con diferentes navegadores web y dispositivos móviles.
- Implementar una sección de ayuda con soporte técnico para asistir a los usuarios..- Fomentar la participación de los usuarios mediante el uso de gamificación y recompensas por logros educativos.
- Asegurar la actualización continua de la plataforma, adaptándose a nuevas tecnologías y necesidades educativas.

### Alcance del desarrollo en esta etapa

La primera versión del aula virtual incluye:

- Registro e inicio de sesión de usuarios.
- Página de inicio con una breve introducción sobre los cursos.
- Página de la asignatura de Álgebra con un índice de los contenidos de cada sección.
- Tres secciones de materiales didácticos y multimedia.
- Formulario de entrega de tareas.
- Página de usuario donde ver sus tareas y notas de las asignaturas.
- Página de ayuda para saber cómo funciona el aula virtual

---

## Arquitectura del Proyecto

### Estructura de carpetas y archivos

```
Estructura del Proyecto
├── audio
│   ├──  abstract_algebra.mp3
│   ├── elemental_algebra.mp3
│   ├── help.mp3
│   └── linear_algebra.mp3
├── icons
│   ├── audio_icon.svg
│   ├── aulavirtual_icon.svg
│   ├── logo.svg
│   └── pause_icon.svg
├── img
│   ├── background.png
│   ├── fondo2.png
│   ├── forms-equation-of-line.png
│   ├── forms-equation-quadratic.png
│   ├── Group-Action.png
│   ├── icons8-pausa-24.png
│   ├── linear-transformations.jpg
│   ├── pdf_icon.png
│   ├── solving-linear-systems.jpg
│   ├── solving-linear-systems.png
│   ├── summarizes-the-axioms-that-define-groups-rings-and-field.png
│   ├── task_icon.png
│   ├── user_profile_icon.png
│   └── user.png
├── pages
│   ├── abstract_algebra.html
│   ├── elemental_algebra.html
│   ├── help.html
│   ├── home.html
│   ├── linear_algebra.html
│   ├── subject.html
│   ├── submit_task.html
│   └── user.html
├── resources
│   ├── abstract_algebra.pdf
│   ├── elemental_algebra.pdf
│   └── linear_algebra.pdf
├── styles
│   ├── index.css
│   ├── index.css.map
│   └── index.scss
├── portada.jpg
├── NOTAS.txt
└── README.md
```

`¿ASÍ BASTA? --> Listado iframes`

### Dependencias utilizadas

- **iframes**: para los vídeos incrustados en las secciones.
  - _What is Algebra | Don't Memorise_ (elemental_algebra.html)
    ```
    <iframe
      class="w-full h-full"
      src="https://www.youtube.com/embed/5Q0FlxcEEIw?si=W6wMG-oGpyfx41Ur"
      title="YouTube video player"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      referrerpolicy="strict-origin-when-cross-origin"
      allowfullscreen
    ></iframe>
    ```
  - _Algebra Basics: What Are Polynomials? - Math Antics_ (elemental_algebra.html)
    ```
    <iframe
      class="w-full h-full"
      src="https://www.youtube.com/embed/ffLLmV4mZwU?si=YjadaFkDsb2wGLI7"
      title="YouTube video player"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      referrerpolicy="strict-origin-when-cross-origin"
      allowfullscreen
    ></iframe>
    ```
  - _Understanding Vector Spaces_ (linear_algebra.html)
    ```
    <iframe
      class="w-full h-full"
      src="https://www.youtube.com/embed/EP2ghkO0lSk?si=Wb5Q2YnJr0bHk-OZ"
      title="YouTube video player"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      referrerpolicy="strict-origin-when-cross-origin"
      allowfullscreen
    ></iframe>
    ```
  - _Finding Eigenvalues and Eigenvectors_ (linear_algebra.html)
    ```
    <iframe
      class="w-full h-full"
      src="https://www.youtube.com/embed/TQvxWaQnrqI?si=TQrPDy7LJK0LayU5"
      title="YouTube video player"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      referrerpolicy="strict-origin-when-cross-origin"
      allowfullscreen
    ></iframe>
    ```
  - _Groups and subgroups_ (abstract_algebra.html)
    ```
    <iframe
      class="w-full h-full"
      src="https://www.youtube.com/embed/ptRmr8LFfc4?si=30gvyjPZ2_pxUmGJ"
      title="YouTube video player"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      referrerpolicy="strict-origin-when-cross-origin"
      allowfullscreen
    ></iframe>
    ```
  - _Group homomorphisms and isomorphisms_ (abstract_algebra.html)
    ```
    <iframe
      class="w-full h-full"
      src="https://www.youtube.com/embed/lbCQgzHdx1Q?si=-LWp9AGTBsjIJRqT"
      title="YouTube video player"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      referrerpolicy="strict-origin-when-cross-origin"
      allowfullscreen
    ></iframe>
    ```

---

## Diseño del Proyecto

`FALTA`

Descripción del diseño inicial en Figma:
El diseño inicial del aula virtual fue creado utilizando Figma, con el objetivo de establecer una estructura visual coherente y funcional para el usuario. Sin embargo, el diseño anterior presentaba varios problemas en cuanto a estética y usabilidad. El fondo era excesivamente cargado, lo que dificultaba la lectura y distría al usuario. La paleta de colores estaba basada principalmente en tonos rojos, lo que generaba una sensación de sobrecarga visual. Además, los botones eran obsoletos y poco amigables, mientras que la estética general del diseño se asemejaba más a una presentación de PowerPoint que a una interfaz web profesional.

Con el fin de mejorar la experiencia del usuario, se rediseñó por completo el aula virtual, destacando los siguientes aspectos:

Nuevos colores: Se adoptó una paleta de colores más moderna y atractiva, centrada en tonos de cian y púrpura, con toques de amarillo para crear contraste. Esto no solo mejora la estética, sino que también facilita la distinción de elementos clave de la interfaz.

Simplificación visual: Se redujo la complejidad de los fondos y se optó por un diseño más limpio, manteniendo el enfoque en el contenido sin distracciones innecesarias.

Botones modernos y funcionales: Se rediseñaron los botones para hacerlos más interactivos y fáciles de usar, asegurando que se ajustaran a la nueva estética sin sacrificar la funcionalidad.

Usabilidad y navegación intuitiva: El diseño final se centró en la usabilidad y la navegación intuitiva, buscando siempre facilitar la interacción con el aula virtual. Los prototipos en Figma reflejan esta orientación al usuario, priorizando la experiencia de aprendizaje.

Traducción del diseño al código
Para implementar el nuevo diseño, se utilizó Tailwind CSS, una herramienta poderosa que facilita la creación de interfaces visualmente atractivas y altamente funcionales a través de clases reutilizables. Esta elección permitió replicar de manera eficiente los prototipos diseñados en Figma, asegurando que el diseño visual se mantuviera fiel a la propuesta original.

Tailwind CSS permitió una personalización rápida y una maquetación flexible, lo que facilitó la adaptación de los distintos componentes del aula virtual a diferentes tamaños de pantalla, garantizando una experiencia óptima tanto en dispositivos móviles como de escritorio.

![comparaciones](./imagenes%20Documentacion/comparation_help.png)
![comparaciones](./imagenes%20Documentacion/comparation_home.png)
![comparaciones](./imagenes%20Documentacion/comparation_linear_algebra.png)
![comparaciones](./imagenes%20Documentacion/comparation_login.png)
![comparaciones](./imagenes%20Documentacion/comparation_subjet.png)
![comparaciones](./imagenes%20Documentacion/comparation_submit.png)
![comparaciones](./imagenes%20Documentacion/comparation_user.png)
![comparaciones](./imagenes%20Documentacion/subjet_deployment.png)



---

## Tecnologías Utilizadas

- **Tailwind CSS**: Framework CSS para estilos rápidos y personalizados, permitiendo una maquetación flexible y eficiente mediante clases utilitarias.
- **HTML**: Lenguaje de marcado utilizado para estructurar el contenido de la página web.
- **CSS**: Lenguaje de estilo utilizado para diseñar y dar formato a la estructura HTML.
- **JavaScript Vanilla**: Lenguaje de programación utilizado para los desplegables y botones de audio.
- **SASS**: Preprocesador CSS que permite escribir estilos más organizados y reutilizables mediante características como variables, anidamiento y mixins, mejorando la mantenibilidad del código.

---

## Integración de Contenido Multimedia

### Tipos de contenido multimedia incluidos

- Imágenes en formatos optimizados (PNG, JPG).
- Iconos en formato SVG.
- Videos incrustados desde YouTube como iframes.
- Audios en formato mp3.
- Archivos descargables en formato PDF.

### Gestión y optimización de estos recursos `FALTA`

- **Reutilización de código**:
- Las img svg tienen pesan menos

---

## Responsividad y Accesibilidad

### Adaptación del diseño a dispositivos móviles y escritorio `REVISAR`

- Uso de clases de Tailwind para diseño adaptable (flex, grid, media queries).
- Optimización para diferentes resoluciones y tamaños de pantalla.

### Medidas de accesibilidad aplicadas

- Uso de etiquetas semánticas en HTML.
- Contrastes adecuados en colores y tipografía.
- Audios para la gente que no pueda leer la página.

---

## Desafíos y Soluciones

### Problemas encontrados durante el desarrollo y soluciones

- **Problema**: Al principio estábamos usando dos versiones de Tailwind distintas, uno la v3.4.17 y otro la v4.0. Esto causó que al intentar aplicar algunos estilos en el CSS se vieran en las páginas con la última versión, mientras que en las que tenían la versión anterior no se veían.
  - **Solución**: La solución fue muy sencilla, en los archivos con versión más antigua los cambiamos para que tuvieran la v4.0 en vez de la v3.4.17.

---

`FALTA`

## Conclusión

El desarrollo del aula virtual con Tailwind CSS ha permitido construir una plataforma moderna, optimizada y accesible. Se lograron implementar buenas prácticas de desarrollo y diseño, garantizando una experiencia de usuario intuitiva y eficiente.
