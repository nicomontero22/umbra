# Umbra - Sitio web estático

Este proyecto corresponde al sitio institucional de **Umbra**, creado con HTML, Bootstrap y una hoja de estilos compilada desde SASS.

## Estructura del proyecto

- `index.html` y páginas dentro de `pages/` contienen la estructura HTML.
- `scss/` concentra los parciales de SASS organizados por base, componentes y secciones.
- `assets/css/style.css` es el archivo generado a partir de `scss/style.scss`.
- `assets/img/` aloja los recursos gráficos.

## Uso de SASS

1. Instala las dependencias del proyecto:
   ```bash
   npm install
   ```
2. Compila la hoja de estilos una única vez:
   ```bash
   npm run build:sass
   ```
3. Para trabajar en modo observador mientras editas SASS:
   ```bash
   npm run watch:sass
   ```

Cada compilación vuelca los cambios de `scss/style.scss` (y sus parciales) en `assets/css/style.css`.

## Despliegue rápido en Netlify

1. Crea un nuevo sitio en [Netlify](https://app.netlify.com/) y conecta este repositorio.
2. Configura los siguientes datos (ya incluidos en `netlify.toml`):
   - **Build command**: `npm run build:sass`
   - **Publish directory**: `.`
3. Ejecuta el despliegue. Netlify instalará las dependencias, compilará SASS y servirá el sitio estático.

> También podés usar otras plataformas de hosting estático como Vercel o Render siguiendo la misma idea: ejecutar `npm run build:sass` antes de publicar.

## Créditos

Proyecto desarrollado por Umbra. Las imágenes incluidas se encuentran en la carpeta `assets/img/`.
