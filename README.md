# Casa Segura — versión Offline / CodePen

## Funciones incorporadas
- Evaluación guiada de condiciones visibles de la vivienda.
- Semáforo y porcentaje general.
- Porcentajes por vivienda, entorno y preparación.
- Geolocalización del navegador mediante permiso del usuario.
- Registro de riesgos del entorno.
- Registro fotográfico guiado desde el celular.
- Mochila de emergencia.
- Plan familiar.
- Guardado local con localStorage.
- Modo oscuro.
- PWA / Service Worker para funcionamiento offline después de la primera carga.

## Importante sobre la ubicación
La app obtiene coordenadas mediante el navegador. En esta versión no consulta automáticamente SIGRID/CENEPRED: registra la ubicación y permite contextualizar la evaluación sin inventar un nivel oficial de peligro. Para una versión productiva se debe integrar una fuente oficial/API o capas descargadas y actualizadas.

## Importante sobre IA y fotografías
Las fotografías se almacenan localmente y se presentan como evidencia visual. Esta versión no afirma detectar estructuralmente grietas, daños ocultos ni certificar seguridad. Para añadir análisis de imágenes con IA se requiere integrar un modelo de visión, lo que normalmente requerirá procesamiento adicional y, según la implementación, conexión.

## CodePen
CodePen no ejecuta el Service Worker de la misma manera que un sitio HTTPS propio. Para probar el modo offline completo, usa la carpeta en un servidor HTTPS/local compatible y publica en GitHub Pages. Para CodePen, copia:
- HTML: contenido de index.html dentro de body
- CSS: style.css
- JS: script.js

## GitHub Pages
Sube todos los archivos manteniendo `assets/`, `manifest.json` y `sw.js`. Luego activa GitHub Pages desde Settings > Pages.
