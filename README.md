# WEB investors aluri

Rediseño de la plataforma aluri para inversionistas, exportado desde Claude Design
(proyecto "Rediseño plataforma Aluri").

## Contenido

| Archivo | Descripción |
| --- | --- |
| `aluri Inversionista WEB.dc.html` | Documento de diseño (canvas) de la plataforma web para inversionistas |
| `aluri Móvil IOS.dc.html` | Documento de diseño de la app móvil iOS |
| `support.js` | Runtime de Claude Design (`dc-runtime`) que renderiza los `.dc.html` |
| `android-frame.jsx` / `ios-frame.jsx` | Componentes de marco de dispositivo usados por los mockups |
| `uploads/` | Imágenes y capturas referenciadas por los diseños |

## Cómo verlo

Abre cualquiera de los archivos `.dc.html` en un navegador. Cada archivo carga
`./support.js`, que monta el canvas con las distintas opciones de diseño.
