# Frontend Mentor - Solución para Insure Landing Page ✨

Esta es una solución al desafío [Insure landing page challenge en Frontend Mentor](https://www.frontendmentor.io/challenges/insure-landing-page-uTU68JV8). Los desafíos de Frontend Mentor te ayudan a mejorar tus habilidades de codificación construyendo proyectos realistas.

## Tabla de Contenidos 📋

- [Resumen 📝](#resumen-📝)
  - [El desafío](#el-desafío)
  - [Captura de pantalla 📸](#captura-de-pantalla-📸)
  - [Enlace 🔗](#enlace-🔗)
- [Mi Proceso 🚀](#mi-proceso-🚀)
  - [Construido con 🏗️](#construido-con-🏗️)
  - [Lo que aprendí 🧠](#lo-que-aprendí-🧠)
  - [Desarrollo Continuo 📈](#desarrollo-continuo-📈)
  - [Recursos Útiles 📚](#recursos-útiles-📚)
- [Autor 🧑‍💻](#autor-🧑‍💻)
- [Agradecimientos 🙌](#agradecimientos-🙌)

## Resumen 📝

### El desafío

Los usuarios deberían poder:

- Ver el diseño óptimo del sitio dependiendo del tamaño de la pantalla de su dispositivo.
- Ver los estados hover para todos los elementos interactivos de la página.

### Captura de pantalla 📸

![Captura de pantalla de la solución de Insure landing page](./design/desktop-design.jpg)

### Enlace 🔗

- URL de la Solución (Repositorio): [https://github.com/josecervera20/insure-landing-page](https://github.com/josecervera20/insure-landing-page)

## Mi Proceso 🚀

### Construido con 🏗️

- Marcado semántico HTML5
- Propiedades personalizadas de CSS (Variables CSS)
- Flexbox (para layouts responsivos y alineación de elementos)
- Diseño Mobile-first
- **Google Fonts: DM Serif Display (para encabezados) y Karla (para el cuerpo del texto)**

### Lo que aprendí 🧠

Durante este proyecto, consolidé y profundicé en varias áreas clave del desarrollo frontend, especialmente en la construcción de layouts responsivos y el manejo de estados interactivos:

- **Diseño Responsivo con Flexbox y Flujo Mobile-First**: Utilicé Flexbox ampliamente para la organización de elementos en diferentes secciones, como la barra de navegación, las "Diferencias" y el footer, asegurando que el diseño se adaptara fluidamente desde móviles hasta escritorio. El enfoque mobile-first me permitió construir la base del diseño para pantallas pequeñas y luego añadir detalles para tamaños mayores.

  ```css
  /* Ejemplo de Flexbox para los elementos diferentes */
  .different__items {
    margin-top: 3.5em;
    display: flex;
    flex-direction: column;
    gap: 3em;
  }

  @media (min-width: 768px) {
    .different__items {
      flex-direction: row;
      gap: 2em;
    }
  }
  ```

- **Implementación de Estados de Hover Suaves con Transiciones**: Practiqué la aplicación de efectos `hover` y transiciones CSS para elementos interactivos clave, como los enlaces de navegación, los botones CTA y los iconos de redes sociales. Esto mejoró significativamente la retroalimentación visual al usuario.

  ```css
  /* Ejemplo de hover para enlaces de navegación (Mobile y Desktop) */
  .nav__link {
    text-decoration: none;
    color: #fff;
    text-transform: uppercase;
    font-weight: 700;
    transition: color 0.3s ease;
  }

  .nav__link:hover {
    color: var(--very-dark-violet);
  }

  /* Ejemplo de hover para botones CTA (nav__link--cta) */
  .nav__link--cta {
    color: #fff;
    border: 1px solid;
    padding: 0.8em 2em;
    transition: background-color 0.3s ease, color 0.3s ease,
      border-color 0.3s ease;
  }

  .nav__link--cta:hover {
    background-color: var(--very-dark-violet);
    color: #fff;
    border-color: var(--very-dark-violet);
  }

  /* Ejemplo de hover para botones CTA (global .cta) */
  .cta {
    display: inline-block;
    border: 1px solid #fff;
    color: #fff;
    padding: 0.8em 2.2em;
    text-transform: uppercase;
    transition: background-color 0.3s ease, color 0.3s ease;
  }

  .cta:hover {
    background-color: #fff;
    color: var(--very-dark-violet);
    font-weight: 700;
  }

  /* Ejemplo de hover para enlaces del footer */
  .footer__link {
    text-decoration: none;
    color: var(--dark-violet);
    font-weight: 700;
    text-transform: uppercase;
    transition: color 0.3s ease;
  }

  .footer__link:hover {
    color: var(--dark-violet);
    text-decoration: underline;
  }

  /* Ejemplo de hover para iconos sociales (usando filtro para SVG) */
  .footer__social {
    transition: filter 0.3s ease;
  }

  .footer__social:hover .footer__icon {
    filter: brightness(0) saturate(100%) invert(8%) sepia(35%) saturate(7400%) hue-rotate(
        250deg
      )
      brightness(97%) contrast(100%);
  }
  ```

- **Variables CSS para Consistencia y Mantenimiento**: Reforcé la práctica de definir variables CSS en `:root` para colores y padding, lo que hizo el código más limpio, mantenible y facilitó las modificaciones globales, como la paleta de colores del diseño.

### Desarrollo Continuo 📈

Me gustaría seguir profundizando en:

- **Accesibilidad (atributos ARIA):** Explorar cómo usar atributos ARIA para mejorar aún más la experiencia de usuario para personas con discapacidades visuales o que usan teclado para navegar.
- **Microinteracciones y Animaciones CSS:** Profundizar en animaciones más complejas usando `keyframes` para añadir un mayor nivel de dinamismo y pulido a la interfaz de usuario.
- **Optimización de rendimiento:** Aprender técnicas más avanzadas para la optimización de imágenes (como `srcset` o formatos de nueva generación) y otros activos para mejorar los tiempos de carga de la página.

### Recursos Útiles 📚

- [Frontend Mentor](https://www.frontendmentor.io/) - Una plataforma excelente para desafíos de codificación.
- [The Markdown Guide](https://www.markdownguide.org/) - Una referencia útil para la sintaxis de Markdown.
- [MDN Web Docs](https://developer.mozilla.org/es/docs/Web) - Siempre una fuente invaluable para entender propiedades CSS y el funcionamiento de HTML.

## Autor 🧑‍💻

- GitHub - [@josecervera20](https://github.com/josecervera20)

## Agradecimientos 🙌

Agradezco a la comunidad de Frontend Mentor por proporcionar desafíos tan valiosos que me permiten mejorar mis habilidades y construir proyectos realistas. También a los recursos en línea como MDN y guías de CSS por ser fuentes invaluables durante el desarrollo.
