# Agencia de Marketing, Publicidad y Desarrollo Full-Stack

## Descripción

Esta es la página web de la nueva agencia que ofrece servicios integrales de marketing, publicidad, community management y desarrollo full-stack.

## Tecnologías

* **React**
* **Next.js** (Framework React con SSR/SSG)
* **TypeScript**
* **Tailwind CSS**
* **Headless CMS** (opcional: Strapi, Sanity)
* **Git** con **Gitflow** para el control de versiones

## Instalación

```bash
# Clona el repositorio
git clone <URL-del-repositorio>
cd <nombre-del-proyecto>

# Instala dependencias
npm install

# Levanta el servidor de desarrollo
npm run dev
```

## Estructura de carpetas

```
├── components/        # Componentes UI reutilizables
├── pages/             # Rutas y API routes de Next.js
│   ├── api/           # Endpoints de servidor (Serverless Functions)
│   └── index.tsx      # Página principal
├── public/            # Archivos estáticos (imágenes, favicon, etc.)
├── styles/            # Archivos CSS globales y configuración de Tailwind
│   └── globals.css
├── lib/               # Utilidades, clientes de API y configuraciones
├── .github/           # Workflows de GitHub Actions (CI/CD)
├── tailwind.config.js # Configuración de Tailwind CSS
├── tsconfig.json      # Configuración de TypeScript
└── package.json       # Scripts y dependencias
```

## Flujo de trabajo con Git (Gitflow)

1. `master` – siempre deployable
2. `develop` – integra features antes de release
3. `feature/<nombre>` – para nuevas funcionalidades
4. `release/<versión>` – pre-release, pruebas finales
5. `hotfix/<fix>` – correcciones urgentes en `master`

### Principales comandos Gitflow

```bash
# Iniciar Gitflow
git flow init

# Crear nueva feature
git flow feature start <nombre>
# Finalizar feature
git flow feature finish <nombre>

# Crear release
git flow release start <versión>
# Finalizar release
git flow release finish <versión>

# Crear hotfix
git flow hotfix start <versión>
# Finalizar hotfix
git flow hotfix finish <versión>
```

## Despliegue

* **Vercel** o **Netlify**: Deploy automático desde `main`
* Se recomienda configurar previews de Pull Request para QA

---

