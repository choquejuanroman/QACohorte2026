## README

# QA Automation — Cypress (Technology with Purpose by Santex) 🚀🧪

Descripción
- Repositorio de ejemplo para aprender y practicar QA Automation usando Cypress. ✅
- Contiene tests, configuraciones y recursos organizados para seguir buenas prácticas y aprender conceptos relevantes. 📚
- Enfocado en el contenido y la metodología de "Technology with Purpose" de Santex. 🌱

Estructura propuesta
- /cypress
  - /fixtures — datos de prueba (JSON, imágenes, etc.) 🗂️
  - /integration — specs / tests (organizados por feature) 🧩
  - /support — comandos personalizados y hooks 🛠️
  - /plugins — plugins de Cypress 🔌
- /scripts — scripts útiles (ej.: ejecución en CI, limpieza) 🏃‍♂️
- /reports — reportes generados (mochawesome, junit) 📊
- cypress.json — configuración principal de Cypress ⚙️
- package.json — dependencias y scripts de npm 📦
- .gitignore 🚫
- README.md (este archivo) 📝

Requisitos
- Node.js >= 14 🔧
- npm o yarn 📦
- Cypress (versión especificada en package.json) 🧪
- (Opcional) Java para algunos reporteros, Docker para ejecución en contenedores 🐳

Instalación rápida
1. Clonar el repositorio:
   git clone <url-del-repo> 📥
2. Entrar al proyecto:
   cd <nombre-del-repo> 📁
3. Instalar dependencias:
   npm install
   o
   yarn install ⚙️

Scripts útiles (ejemplos en package.json)
- npm run cypress:open — abre el Test Runner interactivo 🎯
- npm run cypress:run — ejecuta tests en modo headless 🖥️
- npm run cypress:run:chrome — ejecuta en Chrome headless 🌐
- npm run test:ci — ejecución para CI con reporter y salida JUnit/Mochawesome 🧾
- npm run clean:reports — borra carpetas de reportes 🧹

Buenas prácticas incluidas
- Organización por features y datos en fixtures. 🗃️
- Uso de Page Object / Component Object para mantener mantenibilidad. 🧱
- Comandos personalizados en cypress/support/commands.js para acciones repetidas. 🔁
- Variables de entorno y configuración para separar entornos (baseUrl, credentials). 🔐
- Reportes en mochawesome y salida JUnit para CI. 📑
- Captura de screenshots y videos en fallos (configurable). 📸🎥
- Linter y formateo (ESLint + Prettier) para mantener código consistente. ✨

Ejemplos de tests incluidos
- login.spec.js — pruebas de login válidas e inválidas 🔐
- navigation.spec.js — navegación principal y rutas protegidas 🧭
- form.spec.js — validaciones de formularios y envío 📝
- api.spec.js — validaciones básicas de API integradas con UI (si aplica) 🔗

Integración con CI (ejemplo básico)
- Archivo de ejemplo: .github/workflows/ci.yml ⚙️
- Pasos típicos:
  - checkout ✅
  - setup-node 🔧
  - npm install 📦
  - npm run cypress:run 🧪
  - publicar artefactos (reports, videos, screenshots) 📤

Configuración recomendada
- cypress.json (ejemplo mínimo):
  {
    "baseUrl": "http://localhost:3000",
    "video": true,
    "screenshotOnRunFailure": true,
    "integrationFolder": "cypress/integration",
    "fixturesFolder": "cypress/fixtures"
  } ⚙️
- Variables sensibles en CI o .env (nunca commitear credenciales). 🔒

Cómo contribuir
1. Fork y crear una branch feature/tu-cambio 🌿
2. Hacer commits claros y atómicos ✍️
3. Abrir PR describiendo cambios y pruebas realizadas 🔁
4. Mantener consistencia con ESLint/Prettier ✅

Licencia
- Agregar la licencia que prefieras (ej.: MIT). Incluir archivo LICENSE en la raíz. 📜

Contacto
- Autor / Maintainer: Santex (o el nombre/usuario correspondiente) 👤
- Para dudas o sugerencias, abrir un issue en el repositorio. 🐞

Notas finales
- Este repositorio está pensado como entorno de aprendizaje: adaptar configuración, versiones y ejemplos a tus necesidades reales. 🧠
- Mantener tests pequeños, deterministas y rápidos; separar pruebas de integración pesada para suites específicas. ⚡

¡Listo! 🎉
