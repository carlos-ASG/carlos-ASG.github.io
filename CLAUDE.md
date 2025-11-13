# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal portfolio website built with Astro 5.0 and Vue 3 integration. The project is in Spanish and serves as a showcase for DevCarSan's projects, skills, and professional experience.

## Development Commands

```bash
# Install dependencies
npm install

# Start development server (runs on http://localhost:4321)
npm run dev

# Build for production (outputs to ./dist/)
npm run build

# Preview production build locally
npm run preview

# Run Astro CLI commands
npm run astro -- [command]
```

## Tech Stack

- **Framework:** Astro 5.15.5
- **UI Integration:** Vue 3.5.24 via @astrojs/vue
- **TypeScript:** Strict mode enabled (astro/tsconfigs/strict)
- **JSX:** Configured with preserve mode for Vue compatibility

## Architecture

### Astro Configuration
- Vue integration is enabled in [astro.config.mjs](astro.config.mjs)
- This allows using Vue components alongside Astro components
- TypeScript strict mode with JSX preserve setting for Vue

### Directory Structure
- `src/pages/` - File-based routing; each .astro file becomes a page
- `src/layouts/` - Reusable page layouts (e.g., Layout.astro for HTML structure)
- `src/components/` - Reusable Astro and Vue components
- `src/assets/` - Images and static assets (processed by Astro)
- `public/` - Static files served as-is (favicon, etc.)

### Component Architecture
- **Layouts:** [Layout.astro](src/layouts/Layout.astro) provides the base HTML structure with `<slot />` for content injection
- **Pages:** Use layouts and compose components (e.g., [index.astro](src/pages/index.astro) imports Layout and Welcome)
- **Styles:** Scoped styles in `.astro` files are automatically scoped to the component

## Planned Features (from ABOUT.md)

The portfolio aims to include:
- Featured projects section
- Personal blog
- Contact system
- Dark/light theme toggle
- Animations and transitions
- Headless CMS integration

## Content Language

All user-facing content and documentation (ABOUT.md) is in Spanish. Maintain consistency with Spanish language for any new user-facing content.

## Build Output

Production builds are output to `./dist/` and should not be committed (excluded in tsconfig.json).