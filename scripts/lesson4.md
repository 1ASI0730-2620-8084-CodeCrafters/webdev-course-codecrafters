# Lección 4: Introducción a CSS y estilos sencillos

| | |
|---|---|
| **Duración** | 10 minutos |
| **Empieza a programar** | abre el [JSFiddle de la lección](https://jsfiddle.net/s0fkh9u2/), o copia [`starter-files/lesson4/index.html`](../starter-files/lesson4/index.html) en el panel **HTML** y [`starter-files/lesson4/styles.css`](../starter-files/lesson4/styles.css) en el panel **CSS** de JSFiddle y pulsa **Ejecutar** |
| **Solución** | [`completed-examples/lesson4/index.html`](../completed-examples/lesson4/index.html) y [`styles.css`](../completed-examples/lesson4/styles.css) |

## Qué vas a aprender

- Qué es CSS y cómo se escribe una regla: selector, propiedad y valor.
- Cómo cambiar colores, fondos, la fuente y el tamaño de la letra.
- Cómo centrar el texto y cómo centrar una caja en la página.
- Cómo agregar espacio interior, bordes y esquinas redondeadas.
- Cómo usar una clase para darle estilo a un solo elemento.

## Seguimos con la misma página

En la lección anterior tu página ganó un subtítulo, una lista, una imagen y un enlace. Todo funciona, pero
se ve en blanco y negro, pegado al borde izquierdo y con una imagen enorme. Hoy le damos estilo con **CSS**.

Recuerda: **HTML es el contenido** y **CSS es la apariencia**. En JSFiddle cada uno tiene su propio panel, y
el CSS que escribes en el panel **CSS** se aplica solo a tu HTML: no tienes que conectarlo.

Además, desde hoy en el panel **HTML** escribimos solo lo que va dentro de `<body>`. JSFiddle agrega por
nosotros `<!DOCTYPE html>`, `<html>`, `<head>` y `<body>`, así que el código queda más corto.

## Cómo se escribe una regla CSS

```css
h1 {
  color: blue;
}
```

- `h1` es el **selector**: dice a qué elementos se aplica la regla.
- `color` es la **propiedad**: qué cosa queremos cambiar.
- `blue` es el **valor**: cómo queremos que quede.
- Las propiedades van **entre llaves** `{ }` y cada una termina en **punto y coma** `;`.

Los colores se pueden escribir con su nombre en inglés (`blue`, `white`, `purple`) o con un código que empieza
con `#`, como `#1d4ed8`. El código permite elegir entre millones de tonos.

## Paso 1: una caja para todo el contenido

Para tratar todo el contenido como un bloque, lo metemos en una caja con `<div>` y le ponemos una **clase**:

```html
<div class="card">
  <h1>Mi página personal</h1>
  ...
  <p>
    <a href="https://www.wikipedia.org/" target="_blank">Explorar Wikipedia</a>
  </p>
</div>
```

- `<div>` es una caja que agrupa otros elementos. Por sí sola no se ve.
- `class="card"` le pone un nombre a esa caja para darle estilo desde el CSS.

## Paso 2: el fondo, el color del texto y la fuente

```css
body {
  background-color: #f0f4f8;
  color: #1f2937;
  font-family: Arial, sans-serif;
  line-height: 1.6;
  margin: 20px;
}
```

- `background-color` es el color de fondo; `color`, el color del texto.
- `font-family` elige la fuente. Si `Arial` no está disponible, el navegador usa otra parecida (`sans-serif`).
- `line-height` separa un poco las líneas para que se lean mejor.

## Paso 3: un título centrado

```css
h1 {
  color: #1d4ed8;
  text-align: center;
}
```

`text-align: center` centra el texto dentro de su espacio.

## Paso 4: el tamaño de la letra

```css
p {
  font-size: 18px;
}
```

`font-size` cambia el tamaño de la letra. `px` significa píxeles, los puntitos de la pantalla.

## Paso 5: la caja con estilo y centrada

Para elegir un elemento por su clase, el selector empieza con un **punto**:

```css
.card {
  background-color: white;
  max-width: 500px;
  margin: 20px auto;
  padding: 20px;
  border: 1px solid #cbd5e1;
  border-radius: 12px;
}
```

- `max-width` impide que la caja sea más ancha de 500 píxeles.
- `margin: 20px auto` deja 20 píxeles arriba y abajo, y con `auto` reparte el espacio sobrante a los lados: así
  **la caja queda centrada** en la página.
- `padding` es el espacio **interior**, entre el borde y el contenido.
- `border` dibuja un borde: grosor, estilo (`solid` es una línea continua) y color.
- `border-radius` redondea las esquinas.

## Paso 6: una imagen que cabe en la caja

```css
img {
  max-width: 100%;
  height: auto;
  border-radius: 10px;
}
```

- `max-width: 100%` hace que la imagen no sea más ancha que la caja.
- `height: auto` ajusta la altura para que la imagen no se deforme.

## Paso 7: el color del enlace

```css
a {
  color: #1d4ed8;
}
```

## ⏸ Tu turno

Abre el JSFiddle de la lección, o copia los archivos de [`starter-files/lesson4`](../starter-files/lesson4) en
los paneles **HTML** y **CSS**. Sigue los pasos de los comentarios y pulsa **Ejecutar** después de cada regla
para ver el cambio. Luego haz tuya la página: cambia los colores, el tamaño de la letra o el redondeo de las
esquinas. Si te atascas, compara con [`completed-examples/lesson4`](../completed-examples/lesson4).

## Errores típicos

| Error | Qué pasa | Cómo se arregla |
|---|---|---|
| Olvidar el `;` al final de una propiedad | esa propiedad y la siguiente no se aplican | termina cada propiedad con `;` |
| Olvidar cerrar la llave `}` | las reglas siguientes dejan de funcionar | cierra cada regla con `}` |
| Escribir `card { }` sin el punto | la caja no cambia | las clases se seleccionan con punto: `.card` |
| Escribir mal una propiedad o un color, como `colr` o `bleu` | el navegador la ignora | revisa la ortografía; las propiedades y los colores van en inglés |
| Escribir `margin: 20px` sin `auto` | la caja no se centra | usa `margin: 20px auto` |

## Resumen

- Una regla CSS tiene un **selector**, y entre llaves, **propiedades** con su **valor**.
- `color`, `background-color`, `font-family` y `font-size` cambian el color, el fondo, la fuente y el tamaño.
- `text-align: center` centra el texto; `margin: 20px auto` centra una caja con `max-width`.
- `padding`, `border` y `border-radius` dan espacio interior, bordes y esquinas redondeadas.
- Una clase (`class="card"`) se selecciona en CSS con un punto (`.card`).

**Siguiente:** [Lección 5: Crea tu página de perfil personal](lesson5.md) — juntarás todo lo aprendido para
construir tu propio perfil.
