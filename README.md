# Escuadrado de pérgola (PWA offline)

App para comprobar en obra si la estructura de una pérgola está a escuadra.

- Ancho y largo del hueco (a mano, o leídos del nombre del plano tipo `3020x5450`) → diagonal teórica.
- Las dos diagonales medidas (1→3 y 2→4) y la tolerancia (5 mm por defecto) → **A ESCUADRA** / **FUERA DE ESCUADRA**, con qué esquinas mover y cuántos mm.
- El plano en PDF se ve en el propio navegador (pdf.js en `vendor/`), no se sube a ningún sitio.
- Guarda las últimas medidas en el dispositivo. Funciona sin conexión una vez abierta e instalada.

## Publicar en GitHub Pages

**Settings → Pages → Source → Deploy from a branch → main / (root)**. La URL queda en
`https://andresfh81-boop.github.io/escuadrado-pergola/`.

## Actualizar la app

Cada vez que cambies `index.html`, súbelo y sube en 1 el número de `CACHE_NAME` en `sw.js`
(p. ej. `escuadrado-v2`).
