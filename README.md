# Kazama Translations

Sitio web personal para traducciones de visual novels al español.

## Requisitos

- Ruby 3.x
- Jekyll 4.x
- Bundler

## Instalación Local

```bash
# Instalar dependencias
bundle install

# Ejecutar servidor local
bundle exec jekyll serve
```

El sitio estará disponible en `http://localhost:4000`

## Despliegue en GitHub Pages

1. Crea un repositorio llamado `yamato6.github.io`
2. Sube todos los archivos de esta carpeta
3. Ve a Settings → Pages → Source: "Deploy from a branch" → main
4. Espera unos minutos y tu sitio estará en `https://yamato6.github.io`

## Estructura

```
kazama-translations/
├── _config.yml          # Configuración de Jekyll
├── _layouts/            # Plantillas HTML
├── _posts/              # Entradas del blog
├── _projects/           # Páginas de proyectos
├── assets/
│   ├── css/style.css    # Estilos
│   ├── js/main.js       # JavaScript
│   └── images/          # Imágenes
├── index.html           # Página de inicio
├── proyectos.html       # Lista de proyectos
├── blog.html            # Lista de posts
├── sobre-mi.md          # Página "Sobre mí"
└── contacto.md          # Página de contacto
```

## Añadir un Proyecto

Crea un archivo en `_projects/` con este formato:

```yaml
---
title: "Nombre del Proyecto"
description: "Descripción breve"
status: "En Progreso"  # Completado, En Progreso, Pausado, Planificado
progress: 50           # Porcentaje 0-100
developer: "Desarrollador"
engine: "Motor del juego"
image: "/assets/images/proyecto.jpg"
date: 2025-01-01
download: "https://link-de-descarga.com"  # Opcional
---

Contenido en Markdown...
```

## Añadir un Post

Crea un archivo en `_posts/` con el formato `YYYY-MM-DD-titulo.md`:

```yaml
---
title: "Título del Post"
date: 2025-01-01
categories: [categoria]
---

Contenido en Markdown...
```

## Personalización

Edita las variables CSS en `assets/css/style.css` bajo `:root` para cambiar colores y estilos.
