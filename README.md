# Documentación Técnica - Aula Virtual

### Enlace [FIGMA](https://www.figma.com/design/P4VQQfrHCStX575haD8IvE/AulaVirtual1.0?node-id=0-1&p=f&t=VvwrYf9ojQCg7R1O-0)

### Enlace [presentación pdf](https://github.com/lucaschacon3/AulaVirtual1.0/blob/main/Aula-Virtual-con-Tailwind-CSS-Lucas-al-Cuadrado.pdf) 

### Enlace [presentación web](https://gamma.app/docs/Aula-Virtual-con-Tailwind-CSS-Lucas-al-Cuadrado-lbmypz76q9yf5yl?mode=doc)

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

El diseño virtual en clase es una aplicación de Internet con CSS Tailwind, una estructura que lo ayuda a crear interfaces de usuario de manera rápida y efectiva mediante el uso de capas predefinidas. Esta estructura le permite desarrollar componentes visuales de manera flexible y puede configurar sin guardar una gran cantidad de códigos CSS desde el principio. Esta aplicación tiene como objetivo promover la interacción de los estudiantes con el aula, proporcionando un entorno digital, en el que puede mencionar el entorno digital en el que los materiales educativos y de evaluación y mantener el monitoreo continuo del curso. Además, se ha implementado una estructura de navegación visual desde diferentes dispositivos para garantizar que los usuarios tengan una experiencia conveniente y funcional. Entre las características principales de esta clase virtual se encuentran tareas, visualización de notas, calendarios, monitoreo activo de cursos y acceso a contenido multimedia, incluidas personas con baja visión. El uso de CSS Tailwind garantiza una estructura limpia, moderna y completamente respondida, adaptándose a cualquier tamaño de pantalla para obtener una mejor comodidad en dispositivos móviles, tabletas y formatos. La capa virtual está dedicada a diferentes matemáticas y nos centraremos en el álgebra.

### Objetivos del Proyecto

- Para desarrollar una plataforma ligera para administrar el curso.
- Ingrese un proyecto que sea responsable y barato para todos los dispositivos.
- Crear condiciones para la interacción de los estudiantes con la clase.
- Sistema integrado de gestión de problemas y consulte con comentarios automáticos.
- Proporcione una interfaz intuitiva para navegar y visualizar el contenido educativo. - Encienda la función de monitorear el desarrollo de los estudiantes a través de gráficos y estadísticas.
- Cree condiciones para crear y administrar documentos educativos, como presentaciones, documentos y películas.
- Proporciona compatibilidad con diferentes navegadores web y dispositivos móviles.
- Ingrese un certificado con soporte técnico para ayudar a los usuarios.
- Proporcione actualizaciones continuas de la plataforma, se adapte a nuevas tecnologías y necesidades educativas.

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

**_Descripción del diseño inicial en Figma_**

El diseño inicial del aula virtual fue creado utilizando Figma, con el objetivo de establecer una estructura visual y funcional para el usuario. Sin embargo, el diseño anterior presentaba varios problemas en cuanto a estética y usabilidad. El fondo era excesivamente cargado, lo que dificultaba la lectura y distría al usuario. La paleta de colores estaba basada principalmente en tonos rojos, lo que generaba una sensación de sobrecarga visual. Además, los botones eran obsoletos y poco amigables.


Para mejorar la experiencia del usuario, la capa virtual ha sido completamente rediseñada, enfatizando los siguientes aspectos:

- **Nuevo color**: Se ha aplicado una paleta más moderna y atractiva, centrándose en tonos azules y morados, con trazos amarillos para crear un contraste. Esto no solo mejora la estética, sino que también facilita la diferencia entre los elementos principales de la interfaz. 

- **Simplificación visual**: La complejidad de los fondos se ha reducido y se ha seleccionado un proyecto más limpio, manteniendo el enfoque de contenido sin distracción innecesaria.

- **Botones modernos y funcionales**: Los botones se han rediseñado para hacerlos más interactivos y más fáciles de usar, asegurando que correspondan a la nueva estética sin reservar la funcionalidad. 

- **Usabilidad y navegación visual**: El diseño final se centra en la navegación fácil de usar y visual, siempre tratando de reducir la interacción con la capa virtual. Los prototipos de Figma reflejan la orientación de este usuario, determinando la prioridad de la experiencia educativa.

**_Traducción del diseño al código_**

Para implementar el nuevo diseño, se utilizó Tailwind CSS, una herramienta que facilita la creación de interfaces visualmente atractivas y altamente funcionales a través de clases reutilizables.

Tailwind CSS permitió una personalización rápida y una maquetación flexible, lo que facilitó la adaptación de los distintos componentes del aula virtual a diferentes tamaños de pantalla, garantizando una experiencia óptima tanto en dispositivos móviles como de escritorio.

El diseño del header y del footer se implementó con SASS ya que es el mismo para todas las páginas quitando la de login y la del perfil de usuario.

### Comparación de la Pantalla de Inicio de Sesión

![comparaciones](./imagenes%20Documentacion/comparation_login.png)

En la versión anterior de la pantalla de inicio de sesión, el diseño estaba sobrecargado con muchos elementos y colores intensos que generaban distracción. Los campos de entrada y botones no estaban bien diferenciados, lo que hacía que el usuario tuviera que buscar para encontrar lo que necesitaba. Además, la tipografía y los colores no eran lo suficientemente contrastantes, dificultando la legibilidad, especialmente para usuarios con visión reducida.

En el nuevo diseño, se ha simplificado enormemente la estructura visual. Los botones de inicio de sesión tienen un color distintivo (fuxia) que los hace destacar del fondo, con un contraste mejorado para asegurar que sean fáciles de identificar. El uso de una paleta de colores más suave y moderna también mejora la accesibilidad, mientras que los campos de entrada ahora están mejor alineados y tienen bordes sutiles, lo que permite una mayor claridad y comodidad al usuario.

---

### Comparación de la Página de Usuario

![comparaciones](./imagenes%20Documentacion/comparation_user.png)

El diseño anterior de la página de usuario estaba lleno de elementos con una estética muy anticuada. Los colores predominantes (rojos) creaban un ambiente visualmente denso y desordenado, lo que afectaba la experiencia del usuario.

El rediseño ha mejorado significativamente la organización de los contenidos. Ahora, la información clave, como la barra de progeso y las calificaciones, se encuentran en la parte superior de la página, con un diseño que destaca cada sección y facilita su navegación. Los colores cian y fuxia se usan de manera estratégica para separar visualmente cada bloque de contenido, lo que hace que la página sea más limpia y fácil de seguir. Además, se implementaron iconos claros para representar cada sección, lo que mejora la comprensión visual de la interfaz.

---

### Comparación de la Página de Inicio

![comparaciones](./imagenes%20Documentacion/comparation_home.png)

En el nuevo diseño, la página de inicio se ha simplificado para enfocarse en lo esencial: la presentación de los cursos disponibles y los enlaces directos a las secciones principales. La jerarquía visual está mucho más definida, lo que permite a los usuarios encontrar rápidamente la información que necesitan. Los colores cian y púrpura proporcionan un contraste agradable y la tipografía es más moderna y legible.

---

### Comparación de la Página de Ayuda

![comparaciones](./imagenes%20Documentacion/comparation_help.png)

En el rediseño, la página mantiene el mismo contenido, pero se ha optimizado visualmente con una nueva paleta de colores más suave y contrastante que mejora la legibilidad. Se han implementado pequeños ajustes, como el uso de un fondo más claro y la inclusión de nuevos iconos para hacer la navegación más visual y clara. Además, para mejorar la accesibilidad, se ha añadido un sistema de audio que describe el contenido y facilita la navegación a las personas ciegas o con dificultades visuales. El diseño sigue siendo sencillo, pero ahora más atractivo y funcional, permitiendo que los usuarios puedan acceder a la información de manera más rápida y eficiente.

---

### Comparación de la Página de la Asignatura

![comparaciones](./imagenes%20Documentacion/comparation_subjet.png)

El diseño previo de la página de la asignatura estaba saturado con demasiados elementos visuales que competían entre sí, lo que dificultaba la navegación. Los botones y enlaces no eran fácilmente distinguibles, lo que generaba confusión sobre cómo acceder a los contenidos.

En el nuevo diseño, los materiales y recursos ahora están claramente segmentados, y cada sección tiene su propio espacio y estilo visual, lo que mejora la jerarquía de la información. Se han utilizado tarjetas y bloques bien diferenciados para los diferentes tipos de contenido, y el uso de iconos facilita la comprensión. El diseño ahora es mucho más limpio y sencillo, y la paleta de colores crea un ambiente más relajado y atractivo.

---

### Comparación del Despliegue de la Asignatura

![comparaciones](./imagenes%20Documentacion/subjet_deployment.png)

Este es el desplegable de la asignatura, el cual lleva a los estudiantes a enlaces directos de tareas, teoría y la propia asignatura. En el diseño anterior, los enlaces y recursos estaban desorganizados y resultaban difíciles de encontrar.

Los enlaces están claramente estructurados y categorizados, permitiendo una navegación más sencilla entre las tareas, los materiales teóricos y los contenidos específicos de la asignatura. Este enfoque mejora la accesibilidad y eficiencia, proporcionando una experiencia de usuario más ágil y funcional.

---

### Comparación de la Página de Álgebra Lineal

![comparaciones](./imagenes%20Documentacion/comparation_linear_algebra.png)

Con el nuevo diseño, la página de álgebra lineal es más clara, con un contraste de colores mucho mejor, lo que hace que los contenidos sean fáciles de leer. Los videos y materiales ahora están mejor organizados, con una estructura visual coherente que facilita el acceso. Además, se ha implementado un sistema de navegación de fácil acceso para que los estudiantes puedan saltar entre secciones sin perderse.

---

### Comparación de la Página de Entrega de Tareas

![comparaciones](./imagenes%20Documentacion/comparation_submit.png)

El rediseño ha complementado más esta página. Ahora, los botones de entrega son mucho más visibles y se destacan con colores atractivos, como el cian y el fuxia con amarillo para resaltar, lo que facilita la interacción. Además, la información sobre el estado de las tareas y los plazos se presenta de forma clara, utilizando íconos que permiten a los usuarios estar al tanto de las fechas límite. También se ha mejorado la estructura del formulario de envío para hacerlo más fácil de usar y rápido.

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

### Gestión y optimización de estos recursos

- Las img svg pesan menos y se adaptan mejor a cualquier tamaño sin perder calidad.

---

## Responsividad y Accesibilidad

### Adaptación del diseño a dispositivos móviles y escritorio

- Uso de clases de Tailwind para diseño adaptable (flex, grid, media queries).
- Optimización para diferentes resoluciones y tamaños de pantalla.
- Los tamaños que hemos tenido en cuenta han sido:
  - Diseño móvil: hasta 1024px de ancho (Tailwind es _mobile-first_ por lo que por defecto los estilos son para el móvil).
  - Diseño ordenador: desde 1024px de ancho (En Tailwind se indica con `class="lg:nombre_clase"`).
  - Para la página de home y la de submit_task hemos usado el paso intermedio de 640px (`class="sm:nombre_clase"`).

### Medidas de accesibilidad aplicadas

- Uso de etiquetas semánticas en HTML.
- Contrastes adecuados en colores y tipografía.
- Audios para la gente que no pueda leer la página.

---

## Desafíos y Soluciones

### Problemas encontrados durante el desarrollo y soluciones

- **Problema**: Al principio estábamos usando dos versiones de Tailwind distintas, uno la v3.4.17 y otro la v4.0. Esto causó que al intentar aplicar algunos estilos en el CSS se vieran en las páginas con la última versión, mientras que en las que tenían la versión anterior no se veían.
  - **Solución**: La solución fue muy sencilla, en los archivos con versión más antigua los cambiamos para que tuvieran la v4.0 en vez de la v3.4.17.
