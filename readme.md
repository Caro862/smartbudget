
Este proyecto corresponde a la evaluación del Módulo 3 de Desarrollo de la Interfaz de Usuario Web.

## Tecnologías utilizadas

- HTML5
- CSS3
- SASS
- Bootstrap 5 
- JavaScript

## Metodología Utilizada: BEM (Block, Element, Modifier)

### Estructura de Bloques y Elementos:

- *navbar* (Bloque)
  ├── navbar__logo (Elemento)
  ├── navbar__brand--highlight (Modificador)
  ├── navbar__menu (Elemento)
  ├── navbar__item (Elemento)
  ├── navbar__link (Elemento)
  └── navbar__link--cta (Modificador)

- *hero* (Bloque)
  ├── hero__title (Elemento)
  ├── hero__title--gradient (Modificador)
  ├── hero__subtitle (Elemento)
  └── hero__actions (Elemento)

- *button* (Bloque independiente)
  ├── button--primary (Modificador)
  └── button--secondary (Modificador)

- *features* (Bloque)
  ├── features__title (Elemento)
  ├── features__grid (Elemento)
  └── features__item (Elemento)

- *card* (Bloque reutilizable dentro de features)
  ├── card__icon-wrapper (Elemento)
  ├── card__icon (Elemento)
  ├── card__title (Elemento)
  ├── card__text (Elemento)
  └── card--featured (Modificador)

- *footer* (Bloque)
  ├── footer__copy (Elemento)
  ├── footer__social-nav (Elemento)
  ├── footer__social (Elemento)
  └── footer__social-item (Elemento)

*//Se seleccionó BEM porque permite estructurar las hojas de estilo SASS mediante el anidamiento de selectores de forma limpia, reduciendo la especificidad en CSS y previniendo conflictos de nombres de clases al integrar componentes del framework de Bootstrap 4*//

El proyecto organiza sus estilos de forma modular bajo las siguientes directrices:

- *sass/*
  ├── *abstracts/*: Contiene archivos que no generan CSS por sí mismos (variables de colores, fuentes y mixins).
  │   ├── _variables.scss
  │   └── _mixins.scss
  ├── *base/*: Define las reglas globales del sitio y los resets del modelo de cajas.
  │   ├── _base.scss
  │   └── _typography.scss
  ├── *components/*: Archivos independientes para cada bloque o componente reutilizable de la interfaz.
  │   ├── _navbar.scss
  │   ├── _hero.scss
  │   └── _card.scss
  └── *main.scss*: Archivo central encargado de importar todos los partials anteriores en el orden correcto de cascada.
## Autor
Carolina Tello