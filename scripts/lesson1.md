# Lección 1: ¿Qué es el desarrollo web?

| | |
|---|---|
| **Duración** | 5 minutos |
| **Empieza a programar** | abre el enlace de JSFiddle de la lección (PENDIENTE), o copia [`starter-files/lesson1/index.html`](../starter-files/lesson1/index.html) en el panel **HTML** y [`starter-files/lesson1/styles.css`](../starter-files/lesson1/styles.css) en el panel **CSS** de JSFiddle y pulsa **Ejecutar** |
| **Solución** | [`completed-examples/lesson1/index.html`](../completed-examples/lesson1/index.html) y [`styles.css`](../completed-examples/lesson1/styles.css) |

## Qué vas a aprender

- Qué es una página web y de qué está hecha.
- Qué hace HTML y qué hace CSS.
- Cómo escribir tu primer título y cambiarle el color.

## Una página web está hecha de partes

¿Sabías que cada página que visitas, desde un video hasta una tienda en línea, está construida con
HTML, y casi todas usan CSS para verse bien?

Una página web puede mostrar textos, imágenes, videos y enlaces. Cada uno cumple una función, y juntos
presentan la información. El navegador lee el código de la página y lo convierte en lo que ves en
pantalla.

Para construirla usamos dos tecnologías que trabajan juntas:

| Tecnología | Qué hace | Ejemplos |
|---|---|---|
| **HTML** | organiza el **contenido** | títulos, párrafos, imágenes, listas |
| **CSS** | define la **apariencia** | colores, tamaños, espacios |

Piensa en una casa: **HTML es la estructura** (paredes, puertas, ventanas) y **CSS es la pintura y la
decoración**. Si cambias el texto en HTML, cambia el contenido. Si cambias el color en CSS, cambia la
apariencia.

## El editor online

No hace falta instalar nada. Usaremos JSFiddle, un editor que funciona en tu navegador. Tiene estas
partes:

- **el panel HTML**, donde escribes el contenido de la página;
- **el panel CSS**, donde escribes la apariencia;
- **el botón Ejecutar**, que muestra tu página;
- **el panel Resultado**, donde aparece cómo se ve.

El panel JavaScript no lo usaremos en este curso.

## Tu primer título con HTML

En el panel **HTML** escribe:

```html
<h1>Hola, mundo</h1>
```

Pulsa **Ejecutar** y en el Resultado aparece el título.

- `<h1>` es el **título principal** de la página.
- El texto va **entre** la etiqueta que abre `<h1>` y la que cierra `</h1>`.

Puedes agregar un párrafo debajo con la etiqueta `p`:

```html
<h1>Hola, mundo</h1>
<p>Estoy aprendiendo desarrollo web.</p>
```

## Dale color con CSS

En el panel **CSS** escribe:

```css
h1 {
  color: blue;
}
```

Pulsa **Ejecutar** y el título se vuelve azul.

- `h1` indica **a qué elemento** se aplica la regla.
- `color` indica **qué cambiamos**.
- `blue` es el **nuevo valor**.
- Las llaves `{ }` encierran la regla y cada línea termina en punto y coma `;`.

La regla dice: "a todos los títulos `h1`, ponles color azul". El texto y su estructura vienen de HTML; el
color viene de CSS.

## ⏸ Tu turno

Abre el JSFiddle de la lección y sigue los pasos de los comentarios: escribe un título con tu nombre y
cambia `blue` por otro color, como `red`, `green` o `purple`. Pulsa **Ejecutar** para ver el cambio.
Si te atascas, compara con [`completed-examples/lesson1`](../completed-examples/lesson1).

## Errores típicos

| Error | Qué pasa | Cómo se arregla |
|---|---|---|
| Escribir el código CSS en el panel HTML | el código aparece como texto en la página | pon el HTML en el panel **HTML** y el CSS en el panel **CSS** |
| Olvidar cerrar `</h1>` | el texto que sigue puede verse grande y en negrita, como un título | cierra la etiqueta con `</h1>` |
| Olvidar el `;` o una llave `}` en la regla CSS | el color no cambia | revisa que la regla tenga sus llaves `{ }` y el `;` |
| Escribir mal el nombre del color | el color no cambia | usa nombres válidos como `blue`, `red` o `green` |

## Resumen

- Una página web se construye con **HTML** (el contenido) y **CSS** (la apariencia).
- `<h1>Hola, mundo</h1>` crea un título en HTML y `h1 { color: blue; }` le cambia el color con CSS.

**Siguiente:** [Lección 2: Tu primera página HTML](lesson2.md) — aprenderás cómo se estructura un
documento HTML: etiquetas, elementos y atributos.