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

El archivo [`CNAME`](CNAME) apunta el sitio al dominio `alia.nomaddi.com`. En el DNS de `nomaddi.com` crea un registro `CNAME` de `alia` hacia `nicolasmoreno2914.github.io` y luego activa **Enforce HTTPS** en Settings → Pages.

## Pendiente antes de producción

- Subir la imagen para redes sociales en `og/alia-og.png` (1200×630).
- Completar los enlaces de política de privacidad y tratamiento de datos.
- Mover el bloque SEO (meta, Open Graph, JSON-LD) al `<head>`.
- Configurar `CONFIG.lead.endpoint` (CRM o webhook) para que el formulario de demo envíe datos; mientras sea `null` funciona en modo demostración.
