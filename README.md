# Soy Iker Vericat y este es mi portfolio

# Stack

- Usaré Astro con Typescript y TailwindCSS

# 🚀 Plan de Desarrollo del Proyecto

## 📌 Fase 1: Estructura del proyecto y configuración (Base)
**Objetivo:** Dejar el entorno listo con la arquitectura de archivos recomendada.

- [ ] **Estructura de carpetas:** Crear las carpetas principales dentro de `src/`:
  - `src/components/`: Para elementos visuales reutilizables (`Header`, `Footer`, `Cards`).
  - `src/layouts/`: Para la plantilla base HTML/SEO de todas las páginas.
  - `src/content/projects/`: Donde guardaremos la información de cada proyecto en Markdown.
  - `src/pages/`: Las rutas de la web.
- [ ] **Crear Layout principal (`Layout.astro`):** Configurar la etiqueta `<head>`, fuentes, Tailwind CSS e inclusión de metatags básicos.
- [ ] **Configurar Content Collections:** Definir el esquema de datos con TypeScript (Zod) en `src/content/config.ts` para estructurar la información de tus proyectos (título, descripción, tecnologías, enlaces, imagen).

---

## 🎨 Fase 2: Diseño de componentes base (UI/UX)
**Objetivo:** Construir la cáscara visual de la web usando componentes de Astro + Tailwind.

- [ ] **Header / Navegación:** Menú superior responsive con enlaces a las secciones principales (*Sobre mí*, *Proyectos*, *Contacto*) y botón de GitHub/LinkedIn.
- [ ] **Sección Hero (Presentación):** Tu nombre, rol (*Full Stack / Software Developer*), pequeña bio de 2 líneas y botones de llamada a la acción (*Contactar*, *Ver CV*).
- [ ] **Componente `ProjectCard.astro`:** Tarjeta para mostrar individualmente un proyecto con sus etiquetas de tecnologías (*badges*) y botones (*Ver Demo*, *Código GitHub*).
- [ ] **Footer:** Derechos de autor y accesos rápidos a redes.

---

## 📦 Fase 3: Gestión de contenidos e integración (Proyectos)
**Objetivo:** Rellenar la web con tus proyectos reales utilizando Markdown.

- [ ] **Crear archivos de proyectos:** Añadir 3-5 archivos `.md` en `src/content/projects/` con la información detallada de tus desarrollos (software web, apps móviles, scripts).
- [ ] **Listar proyectos en la Home:** Usar `getCollection('projects')` de Astro para iterar sobre tus archivos y renderizarlos automáticamente en la página principal con `ProjectCard`.
- [ ] **Sección "Sobre mí" y Skills:** Añadir tu trayectoria, tecnologías que dominas (*Frontend*, *Backend*, *DevOps*, *DB*) organizadas visualmente por categorías.
- [ ] **Sección de Contacto:** Añadir un formulario sencillo (conectado a Formspree o Resend) o enlaces directos a tu email y LinkedIn.

---

## ⚡ Fase 4: Optimización, SEO y Despliegue
**Objetivo:** Lanzar la web en tu dominio `ikervericat.dev` con máxima velocidad.

- [ ] **Optimización de imágenes:** Pasar todas las imágenes de proyectos a la carpeta `src/assets/` para que Astro las comprima automáticamente a formato WebP.
- [ ] **Ajustes de SEO y Open Graph:** Configurar la vista previa de tu web cuando compartes el enlace por Twitter/LinkedIn/WhatsApp.
- [ ] **Verificación final:** Probar `npm run build` en local para asegurar que no hay errores de TypeScript.
- [ ] **Hacer `git push`:** Enviar los cambios al repositorio para que GitHub Pages despliegue la web.




# Astro Starter Kit: Basics

```sh
npm create astro@latest -- --template basics
```

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
│   └── favicon.svg
├── src
│   ├── assets
│   │   └── astro.svg
│   ├── components
│   │   └── Welcome.astro
│   ├── layouts
│   │   └── Layout.astro
│   └── pages
│       └── index.astro
└── package.json
```

To learn more about the folder structure of an Astro project, refer to [our guide on project structure](https://docs.astro.build/en/basics/project-structure/).

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
