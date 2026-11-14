# Lección 5: Crea tu página de perfil personal

| | |
|---|---|
| **Duración** | 19 minutos, en dos videos: [parte 1](https://youtu.be/AaZfvO7KclM) (10 minutos) y [parte 2](https://youtu.be/F26iCu-69tg) (9 minutos) |
| **Empieza a programar** | abre el [JSFiddle de la lección](https://jsfiddle.net/jev21yrg/), o copia [`starter-files/lesson5/index.html`](../starter-files/lesson5/index.html) en el panel **HTML** y [`starter-files/lesson5/styles.css`](../starter-files/lesson5/styles.css) en el panel **CSS** de JSFiddle y pulsa **Ejecutar** |
| **Solución** | [`completed-examples/lesson5/index.html`](../completed-examples/lesson5/index.html) y [`styles.css`](../completed-examples/lesson5/styles.css) |

## Qué vas a lograr

Vas a juntar todo lo que aprendiste para construir, desde una página en blanco, **tu propio perfil**: un
título, una presentación, una foto, tus pasatiempos y un enlace. Primero organizas el contenido con **HTML** y
después le das diseño con **CSS**.

## Así se verá tu página

| # | Parte de la página | Etiqueta |
|---|---|---|
| 1 | Nombre | título principal `h1` |
| 2 | Presentación | subtítulo `h2` y párrafo `p` |
| 3 | Fotografía | imagen `img` |
| 4 | Pasatiempos | lista `ul` con `li` |
| 5 | Enlace | vínculo `a` a otra página |

## Parte 1: la estructura con HTML

Todo el contenido va dentro de una caja con la clase `card`, como en la lección anterior:

```html
<div class="card">
  <h1>Mi página personal</h1>

  <h2>Sobre mí</h2>

  <p>
    ¡Hola! Soy estudiante y estoy aprendiendo
    a crear páginas web con HTML y CSS.
  </p>

  <img
    src="https://images.pexels.com/photos/29934077/pexels-photo-29934077.jpeg"
    alt="Fotografía de perfil"
  >

  <h2>Mis pasatiempos</h2>

  <ul>
    <li>Escuchar música</li>
    <li>Leer libros</li>
    <li>Practicar deportes</li>
  </ul>

  <a href="https://www.google.com">
    Visita Google
  </a>
</div>
```

Cambia los textos por los tuyos: tu presentación, tus pasatiempos y una página que te guste.

## Parte 2: el diseño con CSS

```css
body {
  background-color: #eef2f7;
  font-family: Arial, sans-serif;
  color: #333333;
  margin: 0;
  padding: 30px;
}

h1 {
  color: #2563eb;
  text-align: center;
}

h2 {
  color: #1e40af;
}

.card {
  background-color: white;
  max-width: 500px;
  margin: 0 auto;
  padding: 25px;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

img {
  width: 100%;
  border-radius: 8px;
  margin-top: 10px;
}

a {
  color: #2563eb;
}
```

Casi todo ya lo conoces de la lección 4. Hay dos novedades:

- `box-shadow` dibuja una **sombra** debajo de la caja: los dos primeros números la mueven hacia un lado y
  hacia abajo, el tercero la difumina, y `rgba(0, 0, 0, 0.1)` es un negro casi transparente.
- `width: 100%` hace que la imagen ocupe todo el ancho de la caja.

## ⏸ Tu turno

Abre el JSFiddle de la lección, o copia los archivos de [`starter-files/lesson5`](../starter-files/lesson5) en
los paneles **HTML** y **CSS**. Sigue los pasos de los comentarios, pulsa **Ejecutar** después de cada uno y
revisa el resultado. Cuando termines, pulsa **Save** para guardar tu página y obtener un enlace que puedes
compartir. Si te atascas, compara con [`completed-examples/lesson5`](../completed-examples/lesson5).

## Resumen

- Primero se organiza el contenido con HTML y después se le da diseño con CSS.
- Una caja con una clase (`.card`) agrupa el contenido y permite darle estilo como un bloque.
- Revisa el resultado después de cada paso: así encuentras los errores más rápido.

**Siguiente:** [Lección 6: Consejos y errores comunes](lesson6.md) — aprenderás a encontrar y corregir los
errores más comunes.
