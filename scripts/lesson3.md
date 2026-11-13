# Lección 3: Agrega contenido a tu página

| | |
|---|---|
| **Duración** | 10 minutos |
| **Empieza a programar** | abre el enlace de JSFiddle de la lección (PENDIENTE), o copia [`starter-files/lesson3/index.html`](../starter-files/lesson3/index.html) en el panel **HTML** de JSFiddle y pulsa **Ejecutar** |
| **Solución** | [`completed-examples/lesson3/index.html`](../completed-examples/lesson3/index.html) |

## Qué vas a aprender

- Cómo organizar tu página con subtítulos (`h2`).
- Cómo escribir una lista con `ul` y `li`.
- Cómo mostrar una imagen con `img` y sus atributos `src` y `alt`.
- Cómo crear un enlace con `a` y el atributo `href`.

## Seguimos con la misma página

En la lección anterior creaste una página con un título y un párrafo. Hoy le vamos a agregar más
información. Partimos del código con el que terminaste, dentro de `<body>`:

```html
<h1>Mi página personal</h1>
<p>Me gusta aprender, jugar y cuidar a los animales.</p>
```

Todo lo que escribas hoy va dentro de `<body>`, debajo del párrafo.

## Subtítulos con h2

Los títulos tienen niveles. `<h1>` es el más importante y `<h2>` se usa para el subtítulo de cada sección:

```html
<h2>Mis pasatiempos</h2>
```

- Normalmente hay un solo `<h1>` por página: el título principal.
- Los niveles llegan hasta `<h6>`. Mientras más grande es el número, menos importante es el título.

## Listas con ul y li

Para escribir varios elementos uno debajo de otro, usa una lista:

```html
<ul>
  <li>Jugar videojuegos</li>
  <li>Escuchar música</li>
  <li>Cuidar a los animales</li>
</ul>
```

- `<ul>` crea una **lista con viñetas**.
- Cada elemento de la lista va en su propio `<li>`, **dentro** de `<ul>`.
- Si quieres una lista numerada, cambia `ul` por `ol`.

## Imágenes con img

Una imagen se muestra con la etiqueta `<img>`:

```html
<img
  src="https://picsum.photos/id/237/600/400"
  alt="Un perro negro sobre una superficie de madera."
  width="600"
  height="400"
>
```

- `src` es la **dirección** de la imagen.
- `alt` es una **descripción** en texto. La leen los lectores de pantalla y aparece si la imagen no carga.
- `width` y `height` son el ancho y el alto en píxeles.
- `<img>` no tiene etiqueta que cierra: no existe `</img>`.

## Enlaces con a

Un enlace lleva a otra página. Se crea con la etiqueta `<a>`:

```html
<p>
  <a href="https://www.wikipedia.org/" target="_blank">Explorar Wikipedia</a>
</p>
```

- El texto que va **entre** `<a>` y `</a>` es lo que se ve y se puede pulsar.
- `href` es el **destino** del enlace.
- `target="_blank"` abre el enlace en una pestaña nueva. En JSFiddle conviene usarlo, para que el enlace
  no reemplace tu resultado.

## Tu página con todo el contenido

Así queda el código dentro de `<body>`:

```html
<h1>Mi página personal</h1>
<p>Me gusta aprender, jugar y cuidar a los animales.</p>

<h2>Mis pasatiempos</h2>

<ul>
  <li>Jugar videojuegos</li>
  <li>Escuchar música</li>
  <li>Cuidar a los animales</li>
</ul>

<img
  src="https://picsum.photos/id/237/600/400"
  alt="Un perro negro sobre una superficie de madera."
  width="600"
  height="400"
>

<p>
  <a href="https://www.wikipedia.org/" target="_blank">Explorar Wikipedia</a>
</p>
```

## ⏸ Tu turno

Abre el JSFiddle de la lección, o copia [`starter-files/lesson3/index.html`](../starter-files/lesson3/index.html)
en el panel **HTML**. Sigue los pasos de los comentarios: escribe un subtítulo, una lista con tres de tus
pasatiempos, una imagen con su `alt` y un enlace a una página que te guste. Pulsa **Ejecutar** para ver el
resultado. Si te atascas, compara con [`completed-examples/lesson3`](../completed-examples/lesson3).

## Errores típicos

| Error | Qué pasa | Cómo se arregla |
|---|---|---|
| Olvidar `</li>` o `</ul>` | la lista se ve rara o el contenido siguiente queda dentro de ella | cierra cada etiqueta que abres |
| Escribir un `<li>` fuera de `<ul>` | el elemento no se ve como parte de una lista | pon cada `<li>` dentro de `<ul>` |
| Escribir mal la dirección de `src` | la imagen no aparece | copia la dirección completa de la imagen |
| Olvidar el atributo `alt` | quien no puede ver la imagen no sabe qué muestra | agrega `alt` con una descripción corta |
| Dejar `href` vacío o sin escribirlo | el texto no lleva a ningún sitio | escribe la dirección completa del enlace |

## Resumen

- `<h2>` crea un subtítulo; `<ul>` y `<li>` crean una lista.
- `<img>` muestra una imagen con `src` (la dirección) y `alt` (la descripción).
- `<a>` crea un enlace y su atributo `href` indica el destino.

**Siguiente:** [Lección 4: Introducción a CSS y estilos sencillos](lesson4.md) — le darás color, fuente y
bordes a esta misma página.
