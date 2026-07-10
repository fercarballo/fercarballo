<div align="center">
  <img width="100%" src="https://raw.githubusercontent.com/fercarballo/fercarballo/main/assets/new-banner.jpeg" alt="Fernando Carballo — QA Engineer · Automation & SDET" />
</div>

<div align="center">
  <a href="https://fercarballo.com">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3500&pause=900&color=E8B341&center=true&vCenter=true&width=850&height=50&lines=QA+Automation+%26+SDET;Frameworks+E2E%2C+API%2C+mobile+y+performance;CI%2FCD+con+quality+gates+que+bloquean+de+verdad;Evidencia+real%3A+si+no+se+ejecut%C3%B3%2C+lo+digo" alt="QA Automation & SDET" />
  </a>
</div>

<div align="center">
  <a href="https://fercarballo.com"><img src="https://img.shields.io/badge/Portfolio-fercarballo.com-1B5E20?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio" /></a>
  <a href="https://www.linkedin.com/in/fercarballo/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:fercarballodev@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <img src="https://komarev.com/ghpvc/?username=fercarballo&label=Visitas&color=E8B341&style=for-the-badge" alt="Visitas al perfil" />
</div>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:1B5E20,100:E8B341&height=3" width="100%" alt="" />
</div>

## 🎯 Sobre mí

**QA Engineer** enfocado en **automatización y SDET**. Vengo del desarrollo full-stack, y uso ese criterio de ingeniería para construir automatización de calidad de punta a punta: frameworks **E2E**, de **API** y **mobile**, pipelines **CI/CD** con quality gates, **performance**, **seguridad shift-left** y **testing de aplicaciones con IA**.

🌱 **Actualmente:** profundizando en arquitectura de frameworks SDET y en el testing de sistemas no deterministas (LLMs).

## 🧪 Cómo trabajo

> El diferencial no es la herramienta: es **poder demostrar cada afirmación**.

- **🧬 Un dueño por riesgo.** Selenium no reimplementa lo que ya prueba la API; Katalon no duplica la regresión de Selenium. Cada herramienta cubre el riesgo que le corresponde, y nada se prueba dos veces.
- **🚦 Los gates bloquean de verdad.** Y verifico también su **modo de fallo**: un gate que nunca falla no prueba nada.
- **📐 Evidencia honesta.** Cada repositorio distingue explícitamente lo que **se ejecutó** de lo que **no**:

<div align="center">

| | Significado |
|:---:|:---|
| 🟢 | **Ejecutado y verificado.** Hay salida real, reproducible con un comando. |
| 🔴 | **No ejecutado** en ese entorno (licencia, emulador o cuenta cloud). El código es real; la limitación se declara. |

</div>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:1B5E20,100:E8B341&height=3" width="100%" alt="" />
</div>

## 🏦 Nexo Finanzas · ecosistema de calidad para banca

<div align="center">
  <img src="https://img.shields.io/badge/7_repositorios-integrados-1B5E20?style=for-the-badge" alt="7 repositorios" />
  <img src="https://img.shields.io/badge/CI-7%2F7_en_verde-2EA043?style=for-the-badge&logo=githubactions&logoColor=white" alt="CI 7 de 7" />
  <img src="https://img.shields.io/badge/datos-100%25_ficticios-E8B341?style=for-the-badge" alt="Datos ficticios" />
</div>

No son siete tutoriales sueltos: es **un producto financiero ficticio** con sus siete capas de calidad, que se integran entre sí.

```mermaid
flowchart TB
    api["🏦 transfer-api<br/>Spring Boot · idempotencia"]
    web["🌐 web-banking-e2e<br/>Selenium · Cucumber"]
    mob["📱 wallet-mobile<br/>Appium · Page Objects"]
    kat["🔀 cross-channel<br/>Katalon · smoke"]
    perf["⚡ performance-lab<br/>JMeter · SLOs como gate"]
    tower["🗼 control-tower<br/>Jira/Xray · trazabilidad"]
    plat["🚀 quality-platform<br/>Docker · K8s · GitLab CI"]

    api -->|contrato| web
    api -->|contrato| mob
    api --> perf
    web --> kat
    mob --> kat
    api --> kat
    kat --> tower
    perf --> tower
    plat -.->|orquesta los quality gates| api
    plat -.-> tower

    classDef core fill:#1B5E20,stroke:#0d3b12,color:#ffffff,stroke-width:2px
    classDef chan fill:#2E7D32,stroke:#1B5E20,color:#ffffff
    classDef tool fill:#E8B341,stroke:#a97c1f,color:#1b2416
    classDef infra fill:#0D1117,stroke:#E8B341,color:#E8B341,stroke-width:2px
    class api core
    class web,mob chan
    class kat,perf,tower tool
    class plat infra
```

| # | Repositorio | Qué demuestra | Evidencia | CI |
|:--:|---|---|:--:|---|
| 1 | **[nexo-transfer-api](https://github.com/fercarballo/nexo-transfer-api)** | API de transferencias: **idempotencia**, autorización por titularidad, trazabilidad · `Spring Boot` | 🟢 | ![](https://github.com/fercarballo/nexo-transfer-api/actions/workflows/ci.yml/badge.svg) |
| 2 | **[nexo-web-banking-e2e](https://github.com/fercarballo/nexo-web-banking-e2e)** | Framework UI mantenible: **Page Object Model**, esperas web-first · `Selenium` `Cucumber` | 🟢 | ![](https://github.com/fercarballo/nexo-web-banking-e2e/actions/workflows/ci.yml/badge.svg) |
| 3 | **[nexo-wallet-mobile](https://github.com/fercarballo/nexo-wallet-mobile)** | Abstracción de **dos modos**: la suite corre sin emulador · `Appium` | 🟢🔴 | ![](https://github.com/fercarballo/nexo-wallet-mobile/actions/workflows/ci.yml/badge.svg) |
| 4 | **[nexo-cross-channel-regression](https://github.com/fercarballo/nexo-cross-channel-regression)** | Smoke cross-channel + **validador estático propio** como gate · `Katalon` | 🟢🔴 | ![](https://github.com/fercarballo/nexo-cross-channel-regression/actions/workflows/ci.yml/badge.svg) |
| 5 | **[nexo-performance-lab](https://github.com/fercarballo/nexo-performance-lab)** | Hipótesis → **capacidad medida (~460 rps)**; SLOs como gate · `JMeter` | 🟢 | ![](https://github.com/fercarballo/nexo-performance-lab/actions/workflows/ci.yml/badge.svg) |
| 6 | **[nexo-quality-control-tower](https://github.com/fercarballo/nexo-quality-control-tower)** | Matriz **requisito → prueba → resultado**; gate ante requisitos sin cobertura · `Jira/Xray` | 🟢🔴 | ![](https://github.com/fercarballo/nexo-quality-control-tower/actions/workflows/ci.yml/badge.svg) |
| 7 | **[nexo-quality-platform](https://github.com/fercarballo/nexo-quality-platform)** | Entorno reproducible; **rolling update con 0 fallos** · `Docker` `K8s` `GitLab CI` | 🟢 | ![](https://github.com/fercarballo/nexo-quality-platform/actions/workflows/ci.yml/badge.svg) |

<details>
<summary><b>📌 Tres hallazgos que valen más que el código</b></summary>

<br>

- **⚡ El p99 se rompe antes que el p95.** En el laboratorio de performance, a 300 usuarios el promedio decía `304 ms` y mentía: el p99 era `1154 ms`. La cola de la distribución es la alarma temprana, no el promedio.
- **🚀 Un rolling update sin corte no es magia.** Son tres líneas de manifiesto: `maxUnavailable: 0`, dos réplicas y una `readinessProbe` distinta de la liveness. Lo medí: **0 peticiones fallidas** durante el despliegue.
- **🕳️ El hueco más peligroso es el requisito que nadie prueba.** Ninguna suite lo detecta — porque no existe. Por eso la torre de control **falla el pipeline** cuando un requisito no tiene ni una prueba.

</details>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:1B5E20,100:E8B341&height=3" width="100%" alt="" />
</div>

## 🧰 Suite de Automatización de Calidad

<div align="center">
  <img src="https://img.shields.io/badge/10_repositorios-de_fundamentos_a_SDET-1B5E20?style=for-the-badge" alt="10 repositorios" />
</div>

Diez proyectos que recorren el ciclo de testing completo, de los fundamentos a las prácticas propias de un rol SDET. Cada uno con tests ejecutados, documentación técnica y CI.

<details>
<summary><b>🧱 Fundamentos</b> &nbsp;—&nbsp; E2E · API · CI/CD · flakiness · visual & contract</summary>

<br>

| Proyecto | Foco | Stack |
|---|---|---|
| [Framework E2E de UI](https://github.com/fercarballo/playwright-e2e-framework-saucedemo) | Page Object Model, fixtures, cross-browser | `Playwright` `TypeScript` |
| [Testing de API](https://github.com/fercarballo/api-testing-framework-restful-booker) | Contract testing, casos negativos, encadenamiento | `Playwright` `Zod` |
| [Pipeline CI/CD](https://github.com/fercarballo/qa-automation-cicd-pipeline) | Quality gates, dos velocidades, matriz + sharding | `GitHub Actions` |
| [Estabilidad y flakiness](https://github.com/fercarballo/flakiness-hunting-playwright) | Diagnóstico y erradicación: **85 % → 0 %** | `Playwright` |
| [Regresión visual & contract](https://github.com/fercarballo/visual-and-contract-testing) | Screenshots + Pact consumer-driven | `Playwright` `Pact` |

</details>

<details>
<summary><b>🚀 Avanzado (SDET)</b> &nbsp;—&nbsp; performance · integración · DevSecOps · tooling · IA</summary>

<br>

| Proyecto | Foco | Stack |
|---|---|---|
| [Performance & load testing](https://github.com/fercarballo/performance-testing-k6) | Escenarios de carga, thresholds como gate | `k6` |
| [Integración con dependencias reales](https://github.com/fercarballo/integration-testing-testcontainers) | Postgres efímero, constraints y tipos reales | `Testcontainers` `PostgreSQL` |
| [DevSecOps](https://github.com/fercarballo/devsecops-pipeline) | Seguridad shift-left: SAST · SCA · DAST como gates | `Semgrep` `npm audit` |
| [Tooling interno de QA](https://github.com/fercarballo/qa-insights) | Test impact analysis + detección de flaky tests | `TypeScript` |
| [Evals de aplicaciones con IA](https://github.com/fercarballo/llm-evals-harness) | Golden dataset, scorers y umbral como gate | `LLM testing` |

</details>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:1B5E20,100:E8B341&height=3" width="100%" alt="" />
</div>

## ⚙️ Stack

<div align="center">

**Testing & Automatización**

<img src="https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white" alt="Playwright" />
<img src="https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white" alt="Selenium" />
<img src="https://img.shields.io/badge/Appium-662D91?style=for-the-badge&logo=appium&logoColor=white" alt="Appium" />
<img src="https://img.shields.io/badge/Cucumber-23D96C?style=for-the-badge&logo=cucumber&logoColor=white" alt="Cucumber" />
<img src="https://img.shields.io/badge/Katalon-4A9F45?style=for-the-badge" alt="Katalon" />
<img src="https://img.shields.io/badge/JUnit_5-25A162?style=for-the-badge&logo=junit5&logoColor=white" alt="JUnit 5" />
<img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white" alt="Postman" />
<img src="https://img.shields.io/badge/Pact-11B5E4?style=for-the-badge" alt="Pact" />

**Performance & Confiabilidad**

<img src="https://img.shields.io/badge/Apache_JMeter-D22128?style=for-the-badge&logo=apachejmeter&logoColor=white" alt="Apache JMeter" />
<img src="https://img.shields.io/badge/k6-7D64FF?style=for-the-badge&logo=k6&logoColor=white" alt="k6" />
<img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white" alt="Grafana" />

**Lenguajes**

<img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" />
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
<img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js" />
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/Groovy-4298B8?style=for-the-badge&logo=apachegroovy&logoColor=white" alt="Groovy" />

**CI/CD & Infraestructura**

<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" alt="GitHub Actions" />
<img src="https://img.shields.io/badge/GitLab_CI-FC6D26?style=for-the-badge&logo=gitlab&logoColor=white" alt="GitLab CI" />
<img src="https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white" alt="Jenkins" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
<img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes" />
<img src="https://img.shields.io/badge/Testcontainers-291A38?style=for-the-badge&logo=testcontainers&logoColor=white" alt="Testcontainers" />
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />

**Calidad, Seguridad & IA**

<img src="https://img.shields.io/badge/Jira_%2F_Xray-0052CC?style=for-the-badge&logo=jira&logoColor=white" alt="Jira / Xray" />
<img src="https://img.shields.io/badge/Semgrep-1B2C3F?style=for-the-badge&logo=semgrep&logoColor=white" alt="Semgrep" />
<img src="https://img.shields.io/badge/OWASP_ZAP-000000?style=for-the-badge&logo=owasp&logoColor=white" alt="OWASP ZAP" />
<img src="https://img.shields.io/badge/LLM_Evals-8A63D2?style=for-the-badge&logo=anthropic&logoColor=white" alt="LLM Evals" />

</div>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:1B5E20,100:E8B341&height=3" width="100%" alt="" />
</div>

## 📊 Actividad

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=fercarballo&theme=github_dark" />
    <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=fercarballo&theme=default" width="100%" alt="Resumen del perfil" />
  </picture>
</div>

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=fercarballo&theme=github_dark" />
    <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=fercarballo&theme=default" height="200" alt="Lenguajes por repositorio" />
  </picture>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=fercarballo&theme=github_dark" />
    <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=fercarballo&theme=default" height="200" alt="Lenguajes con más commits" />
  </picture>
</div>

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com?user=fercarballo&theme=dark&hide_border=true&background=0D1117&stroke=E8B341&ring=E8B341&fire=E8B341&currStreakLabel=E8B341" />
    <img src="https://streak-stats.demolab.com?user=fercarballo&hide_border=true&stroke=1B5E20&ring=1B5E20&fire=E8B341&currStreakLabel=1B5E20" alt="Racha de contribuciones" />
  </picture>
</div>

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-activity-graph.vercel.app/graph?username=fercarballo&bg_color=0D1117&color=E8B341&line=2EA043&point=FFFFFF&area=true&hide_border=true" />
    <img src="https://github-readme-activity-graph.vercel.app/graph?username=fercarballo&bg_color=FFFFFF&color=1B5E20&line=2E7D32&point=E8B341&area=true&hide_border=true" width="100%" alt="Gráfico de actividad" />
  </picture>
</div>

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/fercarballo/fercarballo/output/github-snake-dark.svg" />
    <img src="https://raw.githubusercontent.com/fercarballo/fercarballo/output/github-snake.svg" width="100%" alt="Snake del gráfico de contribuciones" />
  </picture>
</div>

<div align="center">
  <br>
  <i>«Un gate que nunca falla no prueba nada.»</i>
  <br><br>
  <a href="https://fercarballo.com"><img src="https://img.shields.io/badge/Ver_el_portfolio_completo-fercarballo.com-1B5E20?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Ver el portfolio completo" /></a>
</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:E8B341,100:1B5E20&height=120&section=footer" width="100%" alt="" />
