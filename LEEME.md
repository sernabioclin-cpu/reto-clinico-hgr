# Reto Clínico HGR — sitio del reto

## Estructura
- `index.html` — portada con la convocatoria y el calendario de 6 días (detecta automáticamente qué día es "hoy" según la fecha del dispositivo de quien visita).
- `dia1.html` … `dia6.html` — cada día empieza en estado "próximamente" (candado). El día que le toca a cada meta, se reemplaza el bloque marcado `ESTADO: PRÓXIMAMENTE` por el caso real.
- `plantilla-caso.html` — ejemplo ya armado con el caso de AESP 1, para copiar la estructura del caso, las opciones y el botón hacia el formulario.
- `ganadores.html` — página de resultados; se le agrega una tarjeta por día conforme se van cerrando los retos.
- `style.css` — estilos compartidos por todas las páginas (paleta institucional).

## Publicar cada día
1. Escríbeme (o edítalo tú mismo) el caso clínico del día y el link del Google Form correspondiente.
2. En el archivo `diaN.html` de ese día, sustituye el `<div class="locked">…</div>` por el bloque de caso (copiado de `plantilla-caso.html`), y pega el link real del formulario en el botón "Responder al reto".
3. Sube el cambio a GitHub — con tu flujo habitual de GitHub Pages se refleja solo.

## Publicar un ganador
Agrega una tarjeta en `ganadores.html` (hay un ejemplo comentado en el archivo) con el nombre, servicio/turno y la justificación premiada, y quita el bloque de "aún no hay resultados" cuando ya tengas el primero.

## Sugerencia de despliegue
Mismo patrón que tus otros proyectos (QUIROX, MECIC, Estudio Sombra): repo en `sernabioclin-cpu` + GitHub Pages. Por ejemplo, quedaría en:
`sernabioclin-cpu.github.io/reto-clinico-hgr/`
