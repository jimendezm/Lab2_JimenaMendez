# Lab 3

## Selectores de tipo
Aplicados en:
- `header, nav, section, footer` : Padding para separar contenido.
- `h1, h2, h3` : Colores primarios, peso de fuente y márgenes.
- `p` : Margen inferior para dar separación entre párrafos.
- `img` : Tamaño máximo, borde redondeado.
- `ul` : Eliminación de viñetas y márgenes.
- `article` y `aside` : Fondos diferenciados, bordes y padding.

---

## Selectores de clase
Aplicados en:
- `.btn` : Botones con padding, border-radius y transición.
- `.btn-primary`, `.btn-outline` : Variantes de botones con `:hover` y `:focus-visible`.
- `.card` : Contenedor con fondo, sombra, bordes y `position: relative`.
- `.grid` : Uso de **display: grid** con `repeat(auto-fit, minmax())` y `gap`.
- `.badge` y variantes (`.badge-success`, `.badge-danger`) : Indicadores con colores diferenciados.
- `.tag`, `.tag-success`, `.tag-danger` : Etiquetas con estilos de color.
- `.special` (en overrides.css) : Variante de botón con estilos forzados.

---

## Selectores de ID
Aplicados en:
- `#agenda`, `#expositores`, `#registro`, `#talleres`, `#patrocinadores` : Secciones principales.
- `#about .card` (en overrides.css) : Personalización de card específica.

---

## Selectores de atributo
Aplicados en:
- `a[target="_blank"]` : Color acento y negrita para enlaces externos.
- `img[alt]` : Borde gris a imágenes con atributo alt.
- `input[type="email"]` : Estilos específicos en el campo de correo electrónico.
- `form input[type="radio"], form input[type="checkbox"]` : Ajuste en márgenes.

---

## Combinadores
Aplicados en:
- `.card h3` : Títulos dentro de tarjetas con color destacado.
- `.card .badge` : Posicionamiento absoluto dentro de una card.
- `footer .tag` : Estilo sobrescrito de tags dentro del footer.
- `.tag ~ .tag` : Relación de hermanos para aplicar borde entre tags consecutivos.

---

## Pseudo-clases de estado
Aplicadas en:
- `.btn-primary:hover`, `.btn-outline:hover` : Cambio de color y transformación.
- `.btn-primary:focus-visible` : Outline de accesibilidad.
- `form input:focus-visible, form select:focus-visible, form textarea:focus-visible` : Resaltado al enfocar.
- `form input:active` : Cambio de fondo.

---

## Pseudo-clases estructurales
Aplicados en:
- `ul li:first-child` (HTML implícito) : Diferenciar primer elemento.
- `ul li:nth-child()` (usado en agendas o listas) : Estilizar elementos específicos.

---

## Especificidad
- Uso de `!important` en:
  - `h2` (color forzado).
  - `.btn.special` (estilos sobrescritos).
  - `#about .card` (fondo forzado).
  - `footer .tag` (estilos de etiquetas).
  - `.grid .card` (ajuste de ancho al contenido).
- Uso de inline style en `h1` del header (`color:white; margin-bottom:24px;`).

---

## Box model
Aplicado en:
- `.card` : Uso de `padding`, `margin-block`, `border` y `box-shadow`.
- `article`, `aside`, `footer`, `header` : Padding y bordes.

---

## Overflow
- Definido globalmente en `html { overflow-x: hidden; }` para evitar scroll horizontal.

---

## Flexbox
Aplicado en:
- `body` : `display: flex; flex-direction: column;` para estructura general.
- `nav ul` : `display: flex; gap: 15px;` para organizar enlaces de navegación.
- `main` : `display: flex; flex-direction: column; align-items: center;`.

---

## Grid
Aplicado en:
- `.grid` : `display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px;`.
- `.grid .card` (en overrides.css) : Ajuste de ancho dinámico con `width: auto !important;`.

---

## Position relative/absolute
Aplicado en:
- `.card` : `position: relative;` como contenedor.
- `.card .badge` : `position: absolute;` para ubicar etiqueta en la esquina superior derecha.
