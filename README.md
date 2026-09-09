# eusse-post1-u2 – Laboratorio HTML5

Repositorio único con dos prácticas de la asignatura de Desarrollo Web.

## Parte 1 – Página web semántica (`parte-1-pagina-semantica/`)

Sitio de portafolio personal que incluye:

- **Estructura semántica:** `header`, `nav`, `main`, `section`, `article`, `aside`, `footer`.
- **Logros:** Lista `<ul>` simple (Opción B) — se eligió esta estructura porque cada certificado tiene sentido por sí mismo fuera del sitio, cumpliendo el criterio de “contenido autónomo”.
- **Multimedia:** Etiqueta `<audio>` con archivo `audio/intro.mp3` y transcripción en `<details>/<summary>` para accesibilidad (principio *Perceptible* de WCAG).
- **Preguntas Frecuentes:** Usa `<details>`/`<summary>` con palabra clave resaltada con `<mark>`.

## Parte 2 – Formulario de registro (`parte-2-formulario-registro/`)

Formulario universitario con más de 10 tipos de input de HTML5 (`text`, `email`, `tel`, `date`, `password`, `url`, `number`, `radio`, `select`, `range`, `color`, `checkbox`, `file`, `textarea`, `hidden`). Incluye validación nativa (`required`, `minlength`, `maxlength`, `pattern`) y el campo **teléfono** es opcional, marcado con `aria-describedby` que apunta a un párrafo explicativo (Opción B), garantizando consistencia visual y de accesibilidad.

## Decisiones de diseño justificadas

1. **Lista simple de logros (Opción B):** Cada certificación Udemy es un bloque de información autónomo; presentarlas como `<ul>` facilita la lectura y mantiene el markup limpio sin necesidad de envolver cada una en `<article>`.

2. **Audio con transcripción (Opción B):** La etiqueta `<audio>` permite que la presentación sea escuchada, y el `<details>`/`<summary>` brinda una transcripción textual, cumpliendo el principio **Perceptible** de WCAG (los usuarios pueden elegir modo texto o audio).

3. **`aria-describedby` para teléfono opcional (Opción B):** Al no alterar el `<label>` y vincular el input a un `<p>` explicativo, se mantiene la apariencia visual intacta mientras se comunica claramente que el campo es facultativo, satisfaciendo tanto la consistencia de diseño como las directrices de accesibilidad.