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

## Agendamiento de demos

Todos los botones "Solicitar demo" abren la página de citas de Google Calendar en una pestaña nueva:
https://calendar.app.google/iiyDMaBumkJmyaqD7

Para cambiarla, reemplaza ese enlace en `index.html` (también está en `CONFIG.scheduler`).
