<h1 align="center">Hi, I'm <strong>Julio Mejía</strong> 👋</h1>

<p align="center">
  <a href="https://github.com/julioMejiaRdz">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&center=true&vCenter=true&width=650&lines=Full-Stack+Developer+%F0%9F%9A%80;Web+%C2%B7+Mobile+%C2%B7+Desktop;Real-time+systems+%26+clean+APIs;From+requirements+to+production" alt="Typing SVG" />
  </a>
</p>

<p align="center">
  Systems Engineer — <em>University of El Salvador (UES)</em><br/>
  Building production-ready software across web, mobile &amp; desktop
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Open%20to%20opportunities-2ea44f?style=for-the-badge" alt="Open to opportunities"/>
  &nbsp;
  <img src="https://img.shields.io/badge/Based%20in-El%20Salvador%20%F0%9F%87%B8%F0%9F%87%BB-informational?style=for-the-badge" alt="El Salvador"/>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/julio-mejia-51287733a"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:julayrodriguez5022001@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

---

## About Me

Full-stack developer experienced in building **web, mobile and desktop software**. In my current role I work on **each project end to end** — from requirements and problem analysis through development, unit and integration testing, production deployment and maintenance — designing clean, maintainable architectures and secure APIs.

Across my work I've built **real-time systems**, **enterprise management platforms** and **industrial IoT** integrations. I work under **agile** methodologies and I'm comfortable both driving a project on my own and collaborating within a team.

Above all, I focus on choosing the *right* solution for each problem and shipping it to production.

**Highlights**

- 📡 **Real-time data pipelines** — PLC telemetry from MQTT through a Node.js bridge and Redis Pub/Sub into live WebSocket dashboards (**10 wells** monitored nationwide)
- 🌎 **Multi-tenant, multi-country backend** — one codebase deploying **isolated per-country instances** (database, timezone, locale, branding) behind a domain-routed **NGINX reverse proxy** (🇸🇻 + 🇬🇹)
- 📱 **Offline-first mobile + live tracking** — Kotlin/Compose GPS client with an **idempotent** offline queue that auto-syncs on reconnect; **28 field users** on a live map via Socket.IO
- ⚙️ **End-to-end ownership** — requirements, development, unit & integration testing, production deployment and maintenance

<details>
<summary>🇪🇸 Español</summary>

<br/>

Desarrollador full-stack con experiencia en construir **software web, móvil y escritorio**. En mi rol actual me desempeño en **cada proyecto de extremo a extremo** — desde el análisis de requerimientos y del problema, el desarrollo, las pruebas unitarias y de integración, el despliegue en producción y el mantenimiento — diseñando arquitecturas mantenibles, limpias y APIs seguras.

En mi trabajo he tenido experiencia en el desarrollo de **sistemas en tiempo real**, **plataformas de gestión empresarial** e integraciones de **IoT industrial**. Trabajo bajo metodologías **ágiles** y me siento cómodo tanto liderando un proyecto por mi cuenta como colaborando dentro de un equipo.

Sobre todo, me enfoco en elegir la solución *correcta* para cada problema y llevarla a producción.

**Highlights**

- 📡 **Pipelines de datos en tiempo real** — telemetría de PLCs desde MQTT, vía un *bridge* Node.js y Redis Pub/Sub, hacia dashboards web por WebSocket (**10 pozos** monitoreados a nivel nacional)
- 🌎 **Backend multi-tenant y multi-país** — un mismo código despliega **instancias aisladas por país** (base de datos, zona horaria, locale y branding) tras un **proxy inverso NGINX** enrutado por dominio (🇸🇻 + 🇬🇹)
- 📱 **Móvil offline-first + tracking en vivo** — cliente GPS en Kotlin/Compose con cola offline **idempotente** que auto-sincroniza al reconectar; **28 usuarios de campo** en un mapa en vivo vía Socket.IO
- ⚙️ **Ownership end-to-end** — requerimientos, desarrollo, pruebas unitarias y de integración, despliegue en producción y mantenimiento

</details>

---

## Tech Stack

<div align="center">

<!-- Backend -->
<img src="https://skillicons.dev/icons?i=express,nodejs,typescript" height="45" />

<!-- Frontend -->
<img src="https://skillicons.dev/icons?i=react,nextjs,tailwind" height="45" />

<!-- Mobile & Desktop -->
<img src="https://skillicons.dev/icons?i=kotlin,electron" height="45" />

<!-- Databases -->
<img src="https://skillicons.dev/icons?i=postgres,mongodb" height="45" />

<!-- DevOps -->
<img src="https://skillicons.dev/icons?i=docker,nginx,linux" height="45" />

</div>

<p align="center"><sub>Currently going deeper into: DevOps · Cloud infrastructure</sub></p>

---

## Featured Projects

### Telemetría Hídrica &nbsp;<img src="https://img.shields.io/badge/Live-brightgreen?style=flat-square" alt="Live"/>
Platform for monitoring and controlling water-resource usage in compliance with **ASA regulations**. PLCs publish over **MQTT** and a real-time pipeline streams the readings straight to the web dashboard:
- **Ingestion** — a **Node.js MQTT→Redis bridge** feeds **Django Channels**, pushing readings to the browser over **WebSocket** in real time.
- **Dual-database storage** — **PostgreSQL** for machines, variables and config; **MongoDB** (24h TTL) for high-volume live readings; **Redis** for pub/sub and the task queue.
- **Background processing** — **Celery** workers consume the MQTT stream 24/7 and batch-process readings.

Deployed in production with Docker Compose, monitoring **10 wells** at client sites across El Salvador.
**Stack:** Next.js · Django REST · Django Channels · Celery · Tailwind · PostgreSQL · MongoDB · Redis · MQTT · WebSocket · Docker · NGINX · Azure · Linux
🔗 [c0m3.com](https://c0m3.com/)

### 📍 Compres Sync — GPS Field Tracking &nbsp;<img src="https://img.shields.io/badge/Live-brightgreen?style=flat-square" alt="Live"/> <img src="https://img.shields.io/badge/Enterprise%20%C2%B7%20private-lightgrey?style=flat-square" alt="Private"/>
Internal enterprise system for **real-time GPS monitoring** of the field workforce. A single backend (**Express/TypeScript + Socket.IO**) powers two clients:
- **Mobile (Kotlin)** — background GPS tracking (Doze-resistant) with an **offline queue** (Room) that auto-syncs when connectivity returns.
- **Desktop (Electron)** — supervisor panel with a **live map**, route history, a fuel-reimbursement module and **AI-assisted journey analysis** (Gemini).

Deployed with a **silo multi-tenancy** model — a single codebase runs an **isolated instance per country** (🇸🇻 El Salvador · 🇬🇹 Guatemala), each with its own database and country-scoped configuration (timezone, locale, branding) resolved from a central config module, all on a shared server behind an **NGINX reverse proxy** that routes each country's domain to its instance. Currently tracking **28 field users** in production.

**Stack:** Express · TypeScript · MongoDB · Socket.IO · Electron · React · Kotlin · Jetpack Compose · Google Maps · NGINX

<details>
<summary>🇪🇸 Proyectos (Español)</summary>

<br/>

**Telemetría Hídrica** — <img src="https://img.shields.io/badge/En%20producci%C3%B3n-brightgreen?style=flat-square" alt="En producción"/>
Plataforma para el monitoreo y control del aprovechamiento de recursos hídricos conforme a la **normativa ASA**. Los **PLCs** publican vía **MQTT** y un pipeline en tiempo real transmite las lecturas al panel web: un **bridge Node.js (MQTT→Redis)** alimenta **Django Channels**, que empuja los datos al navegador por **WebSocket**; almacenamiento en doble base de datos (**PostgreSQL** para configuración + **MongoDB** con TTL de 24h para lecturas), con **Redis** para pub/sub y la cola de **Celery** (workers 24/7). Desplegada en producción con Docker, monitoreando **10 pozos** de clientes en El Salvador.
🔗 [c0m3.com](https://c0m3.com/)

**📍 Compres Sync — Rastreo GPS de campo** — <img src="https://img.shields.io/badge/En%20producci%C3%B3n-brightgreen?style=flat-square" alt="En producción"/>
Sistema interno empresarial para el **monitoreo GPS en tiempo real** de la fuerza en campo. Un único backend (**Express/TypeScript + Socket.IO**) que sirve a dos clientes: una **app móvil Kotlin** con tracking en segundo plano y cola offline (Room), y un **panel de supervisión Electron** con mapa en vivo, historial de rutas, módulo de combustible y análisis de jornada con IA (Gemini). Desplegado con un modelo de **multi-tenancy tipo silo** — un mismo código ejecuta una **instancia aislada por país** (🇸🇻 El Salvador · 🇬🇹 Guatemala), cada una con su propia base de datos y configuración por país (zona horaria, locale, branding) resuelta desde un módulo de configuración central, todo sobre un servidor compartido tras un **proxy inverso NGINX** que enruta el dominio de cada país a su instancia. Hoy monitoreando **28 usuarios de campo** en producción.

</details>

---

## GitHub Activity

<div align="center">

<img
  src="https://github-stats-six-opal.vercel.app/api?username=julioMejiaRdz&show_icons=true&count_private=true&include_all_commits=true&hide_border=true&theme=transparent"
  height="160"
/>

<img
  src="https://github-stats-six-opal.vercel.app/api/top-langs/?username=julioMejiaRdz&layout=compact&langs_count=10&hide_border=true&theme=transparent"
  height="160"
/>

</div>

---

## Contact

- 📧 **Email:** julayrodriguez5022001@gmail.com
- 💼 **LinkedIn:** [julio-mejia](https://www.linkedin.com/in/julio-mejia-51287733a)
