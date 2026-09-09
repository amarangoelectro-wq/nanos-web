# Nano's — Web V1.2

Web de Nano's (perniles por encargo, González Catán). Sitio standalone: cada HTML incluye sus estilos, script e imágenes embebidas en base64, así que se puede previsualizar abriéndolo directo desde un servidor local (no funciona con `file://` por las restricciones de algunos navegadores).

## Archivos

- `index-standalone.html` — Home pública. Banner, "Cómo pedir" y "Ubicación" siempre visibles; el resto del contenido (Personas, Perniles, Qué incluye, Galería, Opiniones, Preguntas frecuentes) se navega desde el menú superior, que en mobile se muestra como una fila de botones deslizable.
- `admin-standalone.html` — Prototipo de administración (pedidos, clientes, calendario, productos, reseñas, envíos). No es un backend real: los datos se guardan solo en el navegador durante el preview.
- `HANDOFF-ANGELA.md` — Handoff original con el estado aprobado del proyecto y los datos reales definidos (dirección, WhatsApp, seña, etc.).
- `MENSAJE-PARA-CLOUD-CODE.txt` — Instrucciones iniciales de continuidad del proyecto.
- `serve.ps1` + `.claude/launch.json` — Servidor estático local (PowerShell) para previsualizar los HTML en el navegador durante el desarrollo.

## Cómo previsualizar en local

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -File serve.ps1
```

Después abrir `http://localhost:8791` en el navegador.

## Estado

- Identidad visual, hero, secciones y flujo de WhatsApp: aprobados, no rehacer sin confirmar.
- No hay precios, rendimientos, salsas ni testimonios inventados — todo lo que falta se muestra como "a confirmar" hasta que Nano's lo defina.
- Pendiente: datos definitivos de precios, rendimientos, métodos de pago y capacidad diaria; conectar el admin a una base real con autenticación antes de producción.
