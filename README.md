# WEB investors aluri

Rediseño de la plataforma aluri para inversionistas, exportado desde Claude Design
(proyecto "Rediseño plataforma Aluri").

## Contenido

| Archivo | Descripción |
| --- | --- |
| `index.html` | **Prototipo interactivo navegable** del portal del inversionista — HTML/CSS/JS autónomo, sin dependencias |
| `aluri Inversionista WEB.dc.html` | Documento de diseño (canvas) de la plataforma web — fuente de la que se construyó el prototipo |
| `aluri Móvil IOS.dc.html` | Documento de diseño de la app móvil iOS |
| `support.js` | Runtime de Claude Design (`dc-runtime`) que renderiza los `.dc.html` |
| `android-frame.jsx` / `ios-frame.jsx` | Componentes de marco de dispositivo usados por los mockups |
| `uploads/` | Imágenes y capturas referenciadas por los diseños |

## Prototipo interactivo (`index.html`)

Abre `index.html` en cualquier navegador (doble clic, o sírvelo con
`python3 -m http.server`). Es un único archivo, sin build ni dependencias.

Pantallas y flujos navegables:

- **Inicio** — capital vigente, gráfica de crecimiento, ganancias, alerta de mora
- **Marketplace** — tarjetas de oportunidad con barra de fondeo → botón *Invertir*
- **Fondear una inversión** — asistente de 3 pasos (monto con proyección en vivo →
  cuenta bancaria → tracker de firmas/notaría/registro/desembolso)
- **Mis Inversiones** — panel de portafolio + Diversificación
- **Detalle de crédito** — pestañas Detalles / Abonos (con desglose expandible) /
  Documentos / Cobranza (solo aparece si el crédito está en mora)
- **Notificaciones** — agrupadas por Hoy / Esta semana / Antes
- **Perfil** — Datos personales / adicionales / Documentos / Cuentas bancarias
  (con alta de cuenta propia vs. de tercero) / Seguridad (toggle de 2FA con QR)
- **Programar firma**, **pantalla de desembolso**, modales de **Contacto** y **Extracto**

## Documentos de diseño (`.dc.html`)

Abre cualquiera de los `.dc.html` en un navegador. Cada archivo carga `./support.js`,
que monta el canvas con las 15 iteraciones de diseño.
