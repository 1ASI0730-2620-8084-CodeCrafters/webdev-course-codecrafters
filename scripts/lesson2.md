# Lección 2: Tu primera página HTML

| | |
|---|---|
| **Duración** | 10 minutos |
| **Empieza a programar** | abre el enlace de JSFiddle de la lección (PENDIENTE), o copia [`starter-files/lesson2/index.html`](../starter-files/lesson2/index.html) en el panel **HTML** de JSFiddle y pulsa **Ejecutar** |
| **Solución** | [`completed-examples/lesson2/index.html`](../completed-examples/lesson2/index.html) |

## Qué vas a aprender

- Cómo se estructura un documento HTML.
- Qué son las etiquetas, los elementos y los atributos.
- Cómo escribir tu primer título (`h1`) y tu primer párrafo (`p`).

## Todas las páginas empiezan igual

En la lección anterior vimos que HTML organiza el contenido. Todas las páginas web tienen la misma base,
como el esqueleto de una casa:

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mi página personal</title>
</head>
<body>
  <h1>Mi página personal</h1>
  <p>Me gusta aprender, jugar y cuidar a los animales.</p>
</body>
</html>
```

| Parte | Para qué sirve |
|---|---|
| `<!DOCTYPE html>` | avisa al navegador que es un documento HTML moderno |
| `<html lang="es">` | encierra toda la página; `lang="es"` indica que está en español |
| `<head>` | guarda información de la página que **no se ve** en pantalla |
| `<meta charset="UTF-8">` | hace que se vean bien las tildes y la ñ |
| `<meta name="viewport" ...>` | ayuda a que la página se vea bien en celulares |
| `<title>` | el nombre de la página, que aparece en la pestaña del navegador |
| `<body>` | todo lo que **sí se ve** en la página |

> En JSFiddle el título (`title`) no se ve en la pestaña, porque el resultado aparece dentro de la página
> del editor. Si guardas tu código en un archivo `index.html` y lo abres en el navegador, sí se verá.

## Etiquetas, elementos y atributos

| Palabra | Qué es | Ejemplo |
|---|---|---|
| **Etiqueta** | una palabra entre `<` y `>`; casi siempre hay una que abre y otra que cierra (con `/`) | `<p>` y `</p>` |
| **Elemento** | la etiqueta que abre, el contenido y la etiqueta que cierra | `<p>Hola</p>` |
| **Atributo** | información extra dentro de la etiqueta que abre: un nombre y un valor entre comillas | `lang="es"` |

## Tu título y tu párrafo

Dentro de `<body>` va lo que se ve:

```html
<h1>Mi página personal</h1>
<p>Me gusta aprender, jugar y cuidar a los animales.</p>
```

- `<h1>` es el **título principal** de la página.
- `<p>` es un **párrafo**.
- El texto va **entre** la etiqueta que abre y la que cierra.

Pulsa **Ejecutar** y el navegador muestra el título y el párrafo. Si cambias el texto en HTML, cambia lo
que se ve.

## ⏸ Tu turno

Abre el JSFiddle de la lección, o copia [`starter-files/lesson2/index.html`](../starter-files/lesson2/index.html)
en el panel **HTML**. Sigue los pasos de los comentarios: cambia el texto de `title`, escribe un título con
tu nombre y un párrafo con una presentación breve sobre ti. Pulsa **Ejecutar** para ver el resultado. Si te
atascas, compara con [`completed-examples/lesson2`](../completed-examples/lesson2).

## Errores típicos

| Error | Qué pasa | Cómo se arregla |
|---|---|---|
| Olvidar la etiqueta que cierra, como `</p>` | el contenido siguiente se ve raro | cierra cada etiqueta que abres |
| Escribir mal una etiqueta, como `<hl>` en vez de `<h1>` | el navegador no la reconoce y muestra el texto sin formato | compara el nombre con la etiqueta correcta |
| Escribir contenido dentro de `<head>` | el texto no aparece en la página | pon todo lo visible dentro de `<body>` |
| Olvidar una comilla en un atributo, como `lang="es` | el navegador no entiende el resto de la etiqueta | abre y cierra el valor con `"` |

## Resumen

- Todo documento HTML tiene `<!DOCTYPE html>`, `<html>`, `<head>` y `<body>`.
- Una **etiqueta** abre y cierra, un **elemento** es etiquetas más contenido y un **atributo** da información extra.
- `<h1>` crea el título principal y `<p>` crea un párrafo.

**Siguiente:** [Lección 3: Agrega contenido a tu página](lesson3.md) — seguirás sobre esta misma página
para agregar subtítulos, listas, imágenes y enlaces.
