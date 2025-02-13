# Documentación Técnica - Aula Virtual
https://markdown.es/
## Portada
![Portada del proyecto](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.istockphoto.com%2Fes%2Ffotos%2F%25C3%25A1lgebra&psig=AOvVaw3CSNBwaZcHTc7IDolj47X0&ust=1739526822763000&source=images&opi=89978449)

**Título del Proyecto:** Aula Virtual con Tailwind CSS  
**Integrantes del Equipo:**  
- Lucas Chacón - Rol diseñador y programador 
- Lucas Sánchez - Rol diseñador y programador
**Fecha de Entrega:** 16/02/2025

---

## Índice
1. Introducción  
2. Arquitectura del Proyecto  
3. Diseño del Proyecto  
4. Tecnologías Utilizadas  
5. Integración de Contenido Multimedia  
6. Responsividad y Accesibilidad  
7. Desafíos y Soluciones  

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
│    ├── summarizes-the-axioms-that-define-groups-rings-and-field.png
│    ├── task_icon.png
│    ├── user_profile_icon.png
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
├── NOTAS.txt
└── README.md

```

### Dependencias utilizadas



---

## Diseño del Proyecto
### Descripción del diseño inicial en Figma
Se crearon prototipos en Figma para definir la estructura visual, con especial énfasis en la usabilidad y navegación intuitiva.

### Traducción del diseño al código
Se usó Tailwind CSS para replicar el diseño de Figma, permitiendo una implementación eficiente con clases reutilizables.

---

## Tecnologías Utilizadas
- **Tailwind CSS**: Framework de utilidades para estilos rápidos y flexibles.
- **JavaScript**: Para interactividad y dinámica en la plataforma.

- **Tailwind CSS**: Framework CSS para estilos rápidos y personalizados, permitiendo una maquetación flexible y eficiente mediante clases utilitarias.
- **HTML**: Lenguaje de marcado utilizado para estructurar el contenido de la página web.
- **CSS**: Lenguaje de estilo utilizado para diseñar y dar formato a la estructura HTML.
- **JavaScript Vanilla**: Lenguaje de programación utilizado para los desplegables y botones de audio.
- **SASS**: Preprocesador CSS que permite escribir estilos más organizados y reutilizables mediante características como variables, anidamiento y mixins, mejorando la mantenibilidad del código.

---

## Integración de Contenido Multimedia
### Tipos de contenido multimedia incluidos
- Imágenes en formatos optimizados (WebP, PNG, JPG).
- Videos incrustados desde plataformas como YouTube y Vimeo.
- Documentos PDF y archivos descargables.

### Gestión y optimización de estos recursos
- Uso de lazy loading para mejorar el rendimiento.
- Compresión de imágenes sin perder calidad.
- Carga diferida de videos para evitar bloqueos en la navegación.

---

## Responsividad y Accesibilidad
### Adaptación del diseño a dispositivos móviles y escritorio
- Uso de clases de Tailwind para diseño adaptable (flex, grid, media queries).
- Optimización para diferentes resoluciones y tamaños de pantalla.

### Medidas de accesibilidad aplicadas
- Uso de etiquetas semánticas en HTML.
- Contrastes adecuados en colores y tipografía.
- Compatibilidad con lectores de pantalla.

---

## Desafíos y Soluciones
### Problemas encontrados durante el desarrollo y soluciones
- **Problema:** Dificultades con la configuración inicial de Tailwind.  
  **Solución:** Se revisó la documentación y se ajustó la configuración en `tailwind.config.js`.

- **Problema:** Carga lenta de contenido multimedia.  
  **Solución:** Se implementó lazy loading y optimización de archivos.

- **Problema:** Adaptabilidad a diferentes dispositivos.  
  **Solución:** Se usaron clases responsivas de Tailwind y pruebas en distintos tamaños de pantalla.

---

## Conclusión
El desarrollo del aula virtual con Tailwind CSS ha permitido construir una plataforma moderna, optimizada y accesible. Se lograron implementar buenas prácticas de desarrollo y diseño, garantizando una experiencia de usuario intuitiva y eficiente.

