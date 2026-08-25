<h1 align="center">Hi, I'm <strong>Julio Mejía</strong> 👋</h1>

<p align="center">
  <a href="https://github.com/julioMejiaRdz">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&center=true&vCenter=true&width=650&lines=Systems+Engineer;Full-Stack+Developer;" alt="Typing SVG" />
  </a>
</p>

<p align="center">
 <em>University of El Salvador (UES)</em><br/>
  Web, mobile &amp; desktop software
</p>

## <p align="center">
##  <img src="https://img.shields.io/badge/Open%20to%20opportunities-2ea44f?style=for-the-badge" alt="Open to opportunities"/>
##  &nbsp;
##  <img src="https://img.shields.io/badge/Based%20in-El%20Salvador%20%F0%9F%87%B8%F0%9F%87%BB-informational?style=for-the-badge" alt="El Salvador"/>
## </p>

<p align="center">
  <a href="https://www.linkedin.com/in/julio-mejia-51287733a"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:julayrodriguez5022001@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

---

## About Me

Full-stack developer experienced in building **web, mobile and desktop software**. In my current role I work on **each project end to end** — from requirements and problem analysis through development, unit and integration testing, production deployment and maintenance — designing clean, maintainable architectures and secure APIs.

Across my work I've built **real-time systems**, **enterprise management platforms** and **industrial IoT** integrations. I work under **agile** methodologies and I'm comfortable both driving a project on my own and collaborating within a team.

Above all, I focus on choosing the *right* solution for each problem and shipping it to production.

<details>
<summary>🇪🇸 Español</summary>

<br/>

Desarrollador full-stack con experiencia en desarrollo de **software web, móvil y escritorio**. En mi rol actual me desempeño en **cada proyecto de extremo a extremo** — desde el análisis de requerimientos y del problema, el desarrollo, las pruebas unitarias y de integración, el despliegue en producción y el mantenimiento — diseñando arquitecturas mantenibles, limpias y APIs seguras.

En mi carrera he tenido experiencia en el desarrollo de sistemas **en tiempo real**, **de gestión empresarial** e integraciones de tecnologías **IoT industriales**. Trabajando bajo metodologías **ágiles**, me siento cómodo tanto liderando un proyecto por mi cuenta como colaborando dentro de un equipo.

Sobre todo, me enfoco en elegir la solución *correcta* para cada problema hasta llevarla a producción.

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
Industrial IoT platform for water-resource monitoring under **ASA regulations**. PLCs publish over **MQTT** into a real-time pipeline — a **Node.js MQTT→Redis bridge** feeds **Django Channels**, streaming live readings to the dashboard over **WebSocket**, with dual-database storage (**PostgreSQL** for config + **MongoDB** 24h TTL for readings) and **Celery** workers processing the stream 24/7. In production, monitoring **10 wells** across El Salvador.
**Stack:** Next.js · Django · Django Channels · Celery · PostgreSQL · MongoDB · Redis · MQTT · WebSocket · Docker · NGINX · Azure
🔗 [c0m3.com](https://c0m3.com/)

### 📍 Compres Sync — GPS Field Tracking &nbsp;<img src="https://img.shields.io/badge/Live-brightgreen?style=flat-square" alt="Live"/> <img src="https://img.shields.io/badge/Enterprise%20%C2%B7%20private-lightgrey?style=flat-square" alt="Private"/>
Enterprise system for **real-time GPS monitoring** of a field workforce — one **Express/Socket.IO** backend serving a **Kotlin/Compose** mobile app (background tracking + an **offline queue** that auto-syncs) and an **Electron** supervisor panel (live map, route history, fuel-reimbursement module, **Gemini AI** journey analysis). Deployed as **silo multi-tenancy**: an isolated instance per country (🇸🇻 El Salvador · 🇬🇹 Guatemala) with its own database and config, behind a domain-routed **NGINX reverse proxy** — **28 field users** in production.
**Stack:** Express · TypeScript · MongoDB · Socket.IO · Electron · React · Kotlin · Jetpack Compose · NGINX

<details>
<summary>🇪🇸 Proyectos (Español)</summary>

<br/>

**Telemetría Hídrica** — <img src="https://img.shields.io/badge/En%20producci%C3%B3n-brightgreen?style=flat-square" alt="En producción"/>
Plataforma IoT industrial para el monitoreo de recursos hídricos bajo **normativa ASA**. **PLCs** publican vía **MQTT** hacia un pipeline en tiempo real, un **bridge Node.js (MQTT + Redis)** alimenta **Django Channels**, que transmite las lecturas al panel por **WebSocket**, con doble base de datos (**PostgreSQL** para configuración + **MongoDB** TTL 24h para lecturas históricas) y workers **Celery** procesando el flujo 24/7. En producción, monitoreando **10 pozos** de clientes en El Salvador.
🔗 [c0m3.com](https://c0m3.com/)

**📍 Compres Sync — Rastreo GPS de campo** — <img src="https://img.shields.io/badge/En%20producci%C3%B3n-brightgreen?style=flat-square" alt="En producción"/>
Sistema empresarial interno para el **monitoreo GPS en tiempo real** de la fuerza en campo — un backend **Express/Socket.IO** que sirve a una **app móvil Kotlin/Compose** (tracking en segundo plano + cola offline idempotente que auto-sincroniza) y a un **panel Electron** (mapa en vivo, historial de rutas, módulo de combustible, análisis de jornada con **IA Gemini**). Desplegado como **multi-tenancy tipo silo**: una instancia aislada por sucursal (país) (🇸🇻 El Salvador · 🇬🇹 Guatemala) con su propia base de datos y configuración, tras un **proxy inverso NGINX** enrutado por dominio — **28 usuarios de campo (18 SV + 10 GT)** en producción.

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
