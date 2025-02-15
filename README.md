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

### Comparación de la Pantalla de Inicio de Sesión
![comparaciones](./imagenes%20Documentacion/comparation_login.png)

En la versión anterior de la pantalla de inicio de sesión, el diseño estaba sobrecargado con muchos elementos y colores intensos que generaban distracción. Los campos de entrada y botones no estaban bien diferenciados, lo que hacía que el usuario tuviera que buscar para encontrar lo que necesitaba. Además, la tipografía y los colores no eran lo suficientemente contrastantes, dificultando la legibilidad, especialmente para usuarios con visión reducida.

En el nuevo diseño, se ha simplificado enormemente la estructura visual. Los botones de inicio de sesión son más prominentes y tienen un color distintivo (púrpura) que los hace destacar del fondo, con un contraste mejorado para asegurar que sean fáciles de identificar. El uso de una paleta de colores más suave y moderna también mejora la accesibilidad, mientras que los campos de entrada ahora están mejor alineados y tienen bordes sutiles, lo que permite una mayor claridad y comodidad al usuario.

---

### Comparación de la Página de Usuario
![comparaciones](./imagenes%20Documentacion/comparation_user.png)

El diseño anterior de la página de usuario estaba lleno de elementos innecesarios que no facilitaban la navegación. El contenido estaba demasiado agrupado, lo que ocasionaba que los usuarios tuvieran que desplazarse mucho para acceder a la información importante. Los colores predominantes (rojos) creaban un ambiente visualmente denso y desordenado, lo que afectaba la experiencia del usuario.

El rediseño ha mejorado significativamente la organización de los contenidos. Ahora, la información clave, como las tareas pendientes y las calificaciones, se encuentran en la parte superior de la página, con un diseño de tarjeta que destaca cada sección y facilita su navegación. Los colores cian y púrpura se usan de manera estratégica para separar visualmente cada bloque de contenido, lo que hace que la página sea más limpia y fácil de seguir. Además, se implementaron iconos claros para representar cada sección, lo que mejora la comprensión visual de la interfaz.

---

### Comparación de la Página de Inicio
![comparaciones](./imagenes%20Documentacion/comparation_home.png)

La página de inicio en el diseño anterior estaba llena de información irrelevante y un fondo sobrecargado que no contribuía a la experiencia del usuario. Esto hacía que la página fuera difícil de navegar y que el usuario se sintiera perdido entre tantas opciones y textos.

En el nuevo diseño, la página de inicio se ha simplificado para enfocarse en lo esencial: la presentación de los cursos disponibles y los enlaces directos a las secciones principales. La jerarquía visual está mucho más definida, lo que permite a los usuarios encontrar rápidamente la información que necesitan. Los colores cian y púrpura proporcionan un contraste agradable y la tipografía es más moderna y legible. También se optimizó el diseño para dispositivos móviles, lo que asegura que la experiencia sea igual de fluida en pantallas más pequeñas.

---

### Comparación de la Página de Ayuda
![comparaciones](./imagenes%20Documentacion/comparation_help.png)

En la versión anterior, la página de ayuda estaba dispersa y no tenía una estructura clara, lo que dificultaba la navegación. La información no estaba categorizada y el diseño visual no era atractivo ni intuitivo, lo que provocaba confusión entre los usuarios.

El rediseño de la página de ayuda ahora ofrece un formato más organizado y funcional. La información se ha dividido en secciones claras y bien definidas, utilizando iconos y títulos descriptivos para facilitar la búsqueda de contenido. Además, se ha mejorado el contraste de colores y se ha simplificado la tipografía, lo que permite que los usuarios lean con mayor facilidad. La navegación por la página ahora es más rápida, ya que se ha implementado un menú fijo con enlaces rápidos a las secciones más relevantes.

---

### Comparación de la Página de la Asignatura
![comparaciones](./imagenes%20Documentacion/comparation_subjet.png)

El diseño previo de la página de la asignatura estaba saturado con demasiados elementos visuales que competían entre sí, lo que dificultaba la navegación. Los botones y enlaces no eran fácilmente distinguibles, lo que generaba confusión sobre cómo acceder a los contenidos.

En el nuevo diseño, la página de la asignatura ha sido completamente reorganizada. Los materiales y recursos ahora están claramente segmentados, y cada sección tiene su propio espacio y estilo visual, lo que mejora la jerarquía de la información. Se han utilizado tarjetas y bloques bien diferenciados para los diferentes tipos de contenido (documentos, videos, etc.), y el uso de iconos facilita la comprensión. El diseño ahora es mucho más limpio y sencillo, y la paleta de colores crea un ambiente más relajado y atractivo.

---

### Comparación del Despliegue de la Asignatura
![comparaciones](./imagenes%20Documentacion/subjet_deployment.png)

El despliegue de la asignatura en el diseño anterior era confuso, con materiales dispuestos sin un orden lógico. La interfaz era poco atractiva y no favorecía la interacción con los recursos de la asignatura.

En el nuevo diseño, los materiales de la asignatura están organizados de manera lógica y jerárquica, lo que facilita el acceso a los contenidos. El uso de tarjetas visualmente atractivas para cada recurso permite a los estudiantes encontrar rápidamente el material que necesitan, ya sea un video, una presentación o un archivo PDF. El diseño ahora es mucho más fluido y fácil de navegar, lo que contribuye a una experiencia más eficiente y agradable.

---

### Comparación de la Página de Álgebra Lineal
![comparaciones](./imagenes%20Documentacion/comparation_linear_algebra.png)

En el diseño antiguo, la página de álgebra lineal era difícil de leer y navegar debido a la falta de contraste y la sobrecarga de información. Los recursos estaban desorganizados y no eran fácilmente accesibles, lo que resultaba en una experiencia frustrante para los usuarios.

Con el nuevo diseño, la página de álgebra lineal es más clara, con un contraste de colores mucho mejor, lo que hace que los contenidos sean fáciles de leer. Los videos y materiales ahora están mejor organizados, con una estructura visual coherente que facilita el acceso. Además, se ha implementado un sistema de navegación de fácil acceso para que los estudiantes puedan saltar entre secciones sin perderse.

---

### Comparación de la Página de Entrega de Tareas
![comparaciones](./imagenes%20Documentacion/comparation_submit.png)

En el diseño anterior, la página de entrega de tareas tenía un formato desordenado y poco claro. No se podía visualizar fácilmente el estado de las tareas ni había una retroalimentación clara sobre los plazos y resultados.

El rediseño ha simplificado esta página considerablemente. Ahora, los botones de entrega son mucho más visibles y se destacan con colores atractivos, como el cian y el púrpura, lo que facilita la interacción. Además, la información sobre el estado de las tareas y los plazos se presenta de forma clara, utilizando íconos y alertas que permiten a los usuarios estar al tanto de las fechas límite. También se ha mejorado la estructura del formulario de envío para hacerlo más fácil de usar y rápido.





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
