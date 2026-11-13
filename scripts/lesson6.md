# Lección 6: Consejos y errores comunes

| | |
|---|---|
| **Duración** | 8 minutos |
| **Empieza a programar** | abre el enlace de JSFiddle de la lección (PENDIENTE), o copia [`starter-files/lesson6/index.html`](../starter-files/lesson6/index.html) en el panel **HTML** y [`starter-files/lesson6/styles.css`](../starter-files/lesson6/styles.css) en el panel **CSS** de JSFiddle y pulsa **Ejecutar** |
| **Solución** | [`completed-examples/lesson6/index.html`](../completed-examples/lesson6/index.html) y [`styles.css`](../completed-examples/lesson6/styles.css) |

## Qué vas a aprender

- Que equivocarse es normal y que todos los errores se pueden corregir.
- Los errores más comunes en HTML y en CSS.
- Un método de cinco pasos para revisar tu código.

## Equivocarse es normal

Ya construiste tu página web. Antes de terminar, vamos a revisar el código. Cometer errores es normal; lo
importante es aprender a encontrarlos y corregirlos. Sigue siempre estos cinco pasos:

1. **Observa:** mira el resultado. ¿Qué se ve distinto de lo que querías?
2. **Identifica:** busca en qué parte del código está el problema.
3. **Revisa:** compara lo que escribiste con lo correcto.
4. **Corrige:** arregla **un** error a la vez.
5. **Prueba de nuevo:** pulsa **Ejecutar** y mira si el problema se resolvió.

## Errores comunes en HTML

**Una etiqueta sin cerrar.** Cada etiqueta que abres necesita su cierre:

```html
<h1>Mi página personal      <!-- falta </h1> -->
<h1>Mi página personal</h1> <!-- correcto -->
```

**Una etiqueta mal escrita.** Si el navegador no reconoce el nombre, no la usa. Compáralo con el nombre
correcto:

```html
<il>Escuchar música</il>    <!-- incorrecto -->
<li>Escuchar música</li>    <!-- correcto -->
```

**Una imagen que no aparece.** Revisa que `src` tenga una dirección válida y que no falte `alt`:

```html
<img src="perro.jpg">                                          <!-- la imagen no carga y no tiene alt -->
<img src="https://picsum.photos/id/237/600/400" alt="Un perro negro sobre una superficie de madera.">
```

**Un enlace que no lleva a ningún sitio.** Revisa que `href` tenga la dirección correcta y que el texto
esté dentro de la etiqueta `a`:

```html
<a href="">Explorar Wikipedia</a>                          <!-- href vacío -->
<a href="https://www.wikipedia.org/">Explorar Wikipedia</a> <!-- correcto -->
```

## Errores comunes en CSS

**Falta un punto y coma `;`** al final de una línea, o **falta una llave** `{` o `}`. Cuando eso pasa,
la regla no funciona:

```css
h1 {
  color: #1d4ed8        /* falta el ; */
  text-align: center;
}
```

```css
h1 {
  color: #1d4ed8;
  text-align: center;
}
```

## Recomendaciones para principiantes

- **Escribe un poco, ejecuta y revisa.** Es más fácil encontrar un error cuando acabas de escribirlo.
- **Corrige un error a la vez** y pulsa **Ejecutar** después de cada cambio: así sabes qué arregló el problema.
- **Ordena tu código** con sangría (espacios al inicio de la línea) para ver qué elemento está dentro de cuál.
- **Si no sabes cómo se escribe algo, búscalo.** La documentación de [MDN Web Docs](https://developer.mozilla.org/es/)
  explica cada etiqueta y cada propiedad.
- **Revisa tu HTML completo** en [validator.w3.org](https://validator.w3.org/), que te marca los errores.

## ⏸ Tu turno

Abre el JSFiddle de la lección, o copia [`starter-files/lesson6/index.html`](../starter-files/lesson6/index.html)
y [`starter-files/lesson6/styles.css`](../starter-files/lesson6/styles.css) en los paneles de JSFiddle. La
página tiene **5 errores: 4 en el HTML y 1 en el CSS**. Usa los cinco pasos para encontrarlos y corregirlos,
uno por uno. Cuando termines, tu página debe verse como [`completed-examples/lesson6`](../completed-examples/lesson6).

## Los 5 errores de la práctica

| Dónde | Error | Cómo se arregla |
|---|---|---|
| HTML | `<h1>` sin cerrar | agrega `</h1>` |
| HTML | `<il>` en vez de `<li>` | escribe `<li>` y `</li>` |
| HTML | `src="perro.jpg"` no existe y falta `alt` | usa una dirección válida en `src` y agrega `alt` |
| HTML | `href=""` vacío | escribe la dirección completa del enlace |
| CSS | falta el `;` después del color de `h1` | agrega `;` al final de la línea |

## Resumen

- Observa, identifica, revisa, corrige y prueba de nuevo: corrige un error a la vez.
- Los errores más comunes son etiquetas sin cerrar o mal escritas, `src` o `href` incorrectos, y un `;` o una llave que falta en CSS.
- Ejecuta tu código seguido y consulta MDN cuando tengas dudas.

**¡Felicitaciones!** Has creado tu primera página web con HTML y CSS. Sigue practicando: crea otra página
sobre tu tema favorito.
