# Nexyana (static)

Sitio estático (solo `index.html`) publicado automáticamente en **GitHub Pages** vía **GitHub Actions**, usando el dominio **`nexyana.com`**.

## Estructura

- `index.html`: landing page
- `assets/`: archivos estáticos (imágenes, etc.)
- `CNAME`: dominio personalizado para GitHub Pages
- `.github/workflows/deploy.yml`: workflow de deploy a GitHub Pages

## Deploy (GitHub Pages)

El workflow `.github/workflows/deploy.yml` publica el contenido del repositorio (directorio raíz) en GitHub Pages cada vez que haces push a `main` o `master`.

### Configuración requerida en GitHub

1. Ve a **Settings → Pages**
2. En **Build and deployment**, selecciona **Source: GitHub Actions**

## Dominio `nexyana.com`

Este repo incluye `CNAME` con `nexyana.com`. Para que el dominio apunte correctamente:

- **Apex (nexyana.com)**: crea/actualiza registros DNS **A** hacia GitHub Pages.
- **Opcional (www.nexyana.com)**: crea un **CNAME** de `www` apuntando a `<tu-usuario-o-org>.github.io`.

GitHub mantiene la guía oficial (incluyendo IPs actuales) para custom domains; úsala como referencia si tu DNS provider lo requiere.


