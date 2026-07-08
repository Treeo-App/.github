# Treeo

**El cliente de escritorio para Firebase Firestore.**

Treeo es una app nativa de macOS para explorar, editar y consultar Firestore sin salir del escritorio: navega colecciones, edita documentos campo por campo con tipos exactos, corre queries visuales o scripts de JavaScript con el Admin SDK, y exporta a JSON/CSV — todo en local.

![Treeo](./build/icon.png)

> Sitio web y documentación: **[treeo.app](https://treeo.app)** · Docs: **[treeo.app/docs](https://treeo.app/docs)**

---

## Características

- **Panel de detalle vertical** — cada documento se abre como una pila de bloques editables, uno por campo, con su tipo exacto (`string`, `number`, `boolean`, `timestamp`, `map`, `array`, `reference`, `geopoint`). Map y array se despliegan de forma recursiva sin salir del panel.
- **Consultas visuales** — filtra (`where`), ordena (`orderBy`) y limita una colección desde una barra de herramientas, con paginación por cursor.
- **Scripts de JavaScript** — editor CodeMirror integrado que ejecuta Node.js real contra tu proyecto usando el Admin SDK, para migraciones y consultas que la interfaz no cubre.
- **Vista de tabla y JSON** — tabla virtualizada para colecciones grandes, o edita el documento completo como JSON.
- **Importación y exportación** — JSON/CSV, documento por documento o la conexión entera.
- **Panel de Firebase Auth** — lista, edita y elimina usuarios de Authentication.
- **Todo en local** — las credenciales de la cuenta de servicio se guardan cifradas en tu máquina; Treeo habla directo con Firestore vía Admin SDK, nunca pasa por un servidor intermedio.

## Requisitos

- macOS (Windows y Linux, próximamente)
- Un proyecto de Firebase con una clave de cuenta de servicio (Firebase Console → Configuración del proyecto → Cuentas de servicio)

## Empezar

1. Descarga la última versión desde [treeo.app](https://treeo.app).
2. Abre la app y sube el JSON de tu cuenta de servicio.
3. Navega colecciones, edita documentos y ejecuta scripts.

Guía paso a paso: [treeo.app/docs/conectar-proyecto](https://treeo.app/docs/conectar-proyecto)

## Desarrollo

```bash
npm install
npm run dev          # electron-vite + Electron, con HMR en el renderer
npm run typecheck    # verifica main/preload y renderer
npm run build:mac    # empaqueta un .dmg/.app sin firmar

Stack

Electron + electron-vite · React 19 + TypeScript · Tailwind v4 + shadcn/ui · @tanstack/react-table + @tanstack/react-virtual · Zustand · firebase-admin

Estado del proyecto

Treeo está en desarrollo activo. Consulta la hoja de ruta (https://treeo.app/docs/roadmap) para ver qué viene después.

Licencia

© Treeo. Todos los derechos reservados.
