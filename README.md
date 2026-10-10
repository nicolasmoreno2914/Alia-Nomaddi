# ALIA · Sitio web

Landing comercial de ALIA, el tutor con inteligencia artificial para Moodle.

El sitio es un único archivo estático: [`index.html`](index.html) (estilos, scripts e imágenes incluidos en línea).

## Ver en local

Abre `index.html` en el navegador, o sirve la carpeta:

```bash
python3 -m http.server 8000
```

## Publicar con GitHub Pages

En el repositorio: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, elige la rama y la carpeta `/ (root)`.

## Pendiente antes de producción

- Reemplazar los marcadores `{{SITE_URL}}`, `{{EMAIL_CONTACTO}}` y `{{CIUDAD_PAIS}}`.
- Mover el bloque SEO (meta, Open Graph, JSON-LD) al `<head>`.
- Configurar `CONFIG.lead.endpoint` (CRM o webhook) para que el formulario de demo envíe datos; mientras sea `null` funciona en modo demostración.
