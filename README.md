# Sondeo Vendedores GQM — Octubre 2026

Dashboard resumen del sondeo digital realizado con **Sales Machine** a los vendedores de Grupo Quality Motors (59 respuestas, 19–21 de octubre de 2026; actualizado desde la hoja de respuestas el 21 de octubre).

Cuatro pestañas: **Resumen** (indicadores y gráficos), **Por vendedor** (tabla ordenable con las respuestas de cada vendedor), **Comentarios** (respuestas abiertas, filtrables por tema y pregunta) y **S.O.S. Vendedores** (listas de vendedores a convocar a entrenamientos de Bitrix24).

> Este repositorio es público e incluye nombres de vendedores con sus respuestas.

## Contenido

| Archivo | Uso |
|---|---|
| `index.html` | Dashboard autocontenido (HTML + datos + JS, sin dependencias externas). Se puede abrir directo en el navegador o servir con GitHub Pages. |
| `embed/codigo-iframe-bitrix24.html` | Código listo para pegar en un bloque **Otros → Código HTML** de Bitrix24 Sites. Trae el dashboard dentro de un `iframe` (`srcdoc`) que ajusta su altura solo. |

## Insertar en un landing

**Bitrix24 Sites (sin hosting):** copie todo el contenido de `embed/codigo-iframe-bitrix24.html` y péguelo en un bloque de Código HTML.

**Con GitHub Pages:** active Pages en *Settings → Pages* (rama `main`, carpeta raíz) e inserte:

```html
<iframe src="https://liftbrand.github.io/gqm-vendedores-sondeo/"
        style="width:100%;height:2300px;border:0" loading="lazy"
        title="Sondeo Vendedores GQM"></iframe>
```

## Notas

- Los temas de las respuestas abiertas se clasificaron a partir de las tres preguntas abiertas; un vendedor puede mencionar varios.
- La capacidad promedio cuenta "150 o más" como 150.
- Los datos están fijos al 20 de octubre de 2026. Para actualizar, regenere `index.html` y el código de `embed/` con el nuevo export de respuestas.
