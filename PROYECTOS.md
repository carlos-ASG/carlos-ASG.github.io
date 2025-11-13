# Guía para Agregar Nuevos Proyectos

Esta guía explica cómo agregar nuevos proyectos a tu portafolio de forma sencilla usando archivos Markdown.

## Cómo Funciona el Sistema

Los proyectos se gestionan mediante archivos `.md` en la carpeta `src/content/projects/`. Cada archivo se convierte automáticamente en:

1. **Una tarjeta** en la página principal (sección Proyectos)
2. **Una página individual** con todo el contenido detallado del proyecto

## Cómo Agregar un Nuevo Proyecto

### Paso 1: Crea un nuevo archivo `.md`

Crea un nuevo archivo en `src/content/projects/` con el nombre de tu proyecto:
- `mi-proyecto.md` → URL: `/proyectos/mi-proyecto`
- `sistema-gestion-tareas.md` → URL: `/proyectos/sistema-gestion-tareas`

### Paso 2: Usa esta plantilla

```markdown
---
title: "Nombre del Proyecto"
description: "Descripción breve (1-2 líneas) que aparecerá en la tarjeta"
image: "/projects/mi-imagen.jpg"
date: 2025-01-15
tags: ["Tecnología 1", "Tecnología 2", "Tecnología 3"]
published: true
---

## Descripción Detallada

Aquí comienza el contenido completo de tu proyecto. Puedes usar todo el Markdown que necesites.

### Subsección

- Lista de características
- Otra característica
- Más detalles

## Tecnologías Utilizadas

Describe las tecnologías...

## Proceso de Desarrollo

Cuenta la historia del desarrollo...

## Resultados

Comparte los resultados y métricas...
```

### Paso 3: Campos del Front Matter

Los campos entre `---` al inicio del archivo:

| Campo | Tipo | Requerido | Descripción |
|-------|------|-----------|-------------|
| `title` | string | ✅ Sí | Título del proyecto |
| `description` | string | ✅ Sí | Descripción breve para la tarjeta (1-2 líneas) |
| `image` | string | ✅ Sí | Ruta a la imagen de cabecera |
| `date` | date | ✅ Sí | Fecha del proyecto (formato: YYYY-MM-DD) |
| `tags` | array | ❌ No | Lista de tecnologías o categorías |
| `published` | boolean | ❌ No | Si es `false`, el proyecto no se mostrará |

### Paso 4: Agregar Imágenes

1. Coloca tus imágenes en la carpeta `/public/projects/`
2. Referencia la imagen: `image: "/projects/mi-imagen.jpg"`
3. Recomendación: Mínimo 1200px de ancho

**Formatos recomendados:**
- JPG para fotografías
- PNG para capturas de pantalla
- SVG para gráficos vectoriales

## Ejemplo Completo

Ver el archivo `src/content/projects/proyecto-ejemplo.md` como referencia.

## Estructura de Contenido Recomendada

```markdown
## Descripción del Proyecto
Contexto y problema que resuelve...

## Características Principales
1. **Característica 1**: Descripción
2. **Característica 2**: Descripción

## Tecnologías Utilizadas
- **Frontend**: Lista de tecnologías
- **Backend**: Lista de tecnologías

## Proceso de Desarrollo
Describe las fases del desarrollo...

## Desafíos y Soluciones
Los retos que enfrentaste...

## Resultados
Métricas, feedback, impacto...

## Aprendizajes
Qué aprendiste del proyecto...
```

## Consejos

### Para la descripción breve:
- Máximo 2 líneas
- Resume lo más importante
- Lenguaje claro y directo

### Para el contenido completo:
- Usa títulos (`##`, `###`) para organizar
- Usa listas para facilitar la lectura
- Usa **negritas** para destacar términos importantes
- Explica el problema, proceso y resultados

## Orden de Visualización

Los proyectos se ordenan automáticamente por fecha (más recientes primero). Para cambiar el orden, modifica la fecha en el front matter.

## Ocultar un Proyecto Temporalmente

```markdown
---
published: false
---
```

## Previsualización

1. Guarda el archivo
2. El servidor de desarrollo recargará automáticamente
3. Ve a la página principal para ver la tarjeta
4. Haz clic en "Ver detalles" para ver la página completa

## ¿Necesitas Ayuda?

- [Guía de Markdown](https://www.markdownguide.org/basic-syntax/)
- Revisa `proyecto-ejemplo.md` como referencia
- Consulta la documentación de Astro Content Collections
