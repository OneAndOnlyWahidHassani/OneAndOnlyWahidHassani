<p align="center">
  <img src="./assets/banner.svg" alt="Wahid Hassani — full-stack developer in Malmö, Sweden" width="100%" />
</p>

<p align="center">
  <a href="mailto:Wahid_Hassani@outlook.com"><img src="https://img.shields.io/badge/Email-1b1733?style=for-the-badge&logo=maildotru&logoColor=ffb95e" alt="Email" /></a>
  <a href="https://www.linkedin.com/in/wahid-hassani-wh"><img src="https://img.shields.io/badge/LinkedIn-1b1733?style=for-the-badge&logo=linkedin&logoColor=ffb95e" alt="LinkedIn" /></a>
  <img src="https://img.shields.io/badge/Malmö,_Sweden-1b1733?style=for-the-badge&logo=googlemaps&logoColor=ffb95e" alt="Based in Malmö, Sweden" />
  <img src="https://komarev.com/ghpvc/?username=OneAndOnlyWahidHassani&style=for-the-badge&color=5c2a5e&label=Profile+views" alt="Profile views" />
</p>

<br />

I like turning a vague "wouldn't it be nice if…" into something that actually runs. Lately that means a real-time social platform written in **Go** and **Svelte**, local LLM services built with a team for **Beijer Electronics**, and a steady stream of smaller apps in whatever stack fits the problem: React, .NET, Flutter or plain C.

Most of my work lives in private repos, so here's a tour instead.

<br />

## 🔭 What I'm building now

### Counterpart

A real-time social platform for web and desktop, with friends and presence, voice rooms with end-to-end encryption, MFA and account security, file uploads to Cloudflare R2, and an admin panel for moderation. Built solo, 100+ commits and counting.

It's designed to serve 10,000–50,000 users on a single machine, and the architecture lets it grow both vertically and horizontally from there. Currently in testing ahead of launch.

<p>
  <img src="https://img.shields.io/badge/Status-In_testing-1b1733?style=flat-square&labelColor=5c2a5e" />
</p>

<p>
  <img src="https://img.shields.io/badge/Go-1b1733?style=flat-square&logo=go&logoColor=00ADD8" />
  <img src="https://img.shields.io/badge/WebSockets-1b1733?style=flat-square&logo=socketdotio&logoColor=ffffff" />
  <img src="https://img.shields.io/badge/SvelteKit-1b1733?style=flat-square&logo=svelte&logoColor=FF3E00" />
  <img src="https://img.shields.io/badge/TypeScript-1b1733?style=flat-square&logo=typescript&logoColor=3178C6" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-1b1733?style=flat-square&logo=tailwindcss&logoColor=06B6D4" />
  <img src="https://img.shields.io/badge/Tauri-1b1733?style=flat-square&logo=tauri&logoColor=FFC131" />
  <img src="https://img.shields.io/badge/PostgreSQL-1b1733?style=flat-square&logo=postgresql&logoColor=4169E1" />
  <img src="https://img.shields.io/badge/Redis-1b1733?style=flat-square&logo=redis&logoColor=FF4438" />
  <img src="https://img.shields.io/badge/Cloudflare_R2-1b1733?style=flat-square&logo=cloudflare&logoColor=F38020" />
  <img src="https://img.shields.io/badge/Nginx-1b1733?style=flat-square&logo=nginx&logoColor=009639" />
  <img src="https://img.shields.io/badge/Docker-1b1733?style=flat-square&logo=docker&logoColor=2496ED" />
</p>

<br />

## 📄 Research

### Dense vs. Mixture-of-Experts transformers on consumer hardware

*Bachelor's thesis, Malmö University, 2026, with [@AdamMheisen](https://github.com/AdamMheisen)*
<!-- When the thesis is published, I'll link it here, like in [Read the thesis](https://...) -->

Do MoE models actually save energy outside the datacenter? We trained two ~1B-parameter language models from scratch on 10B tokens using JAX/Flax on a Cloud TPU v4-32: a dense transformer and a Switch-style MoE with 8 experts and top-1 routing, matched to within 0.03% in parameter count. We then benchmarked inference on a single RTX 5080, measuring GPU power through NVML across a grid of batch sizes and sequence lengths.

The MoE model was more energy efficient in all 30 paired runs: up to **43% more tokens per joule** and **21% less GPU energy** over the full workload, while also running faster. The catch is quality. At this training budget, the dense model reached clearly better perplexity and accuracy, so the result is a real efficiency–quality trade-off rather than a free lunch.

<p align="center">
  <img src="./assets/thesis-chart.svg" alt="Tokens per joule, dense vs MoE. MoE wins in all six configurations, from +9.5% to +43.1%." width="100%" />
</p>

<p>
  <img src="https://img.shields.io/badge/JAX-1b1733?style=flat-square&logo=google&logoColor=ffffff" />
  <img src="https://img.shields.io/badge/Flax-1b1733?style=flat-square&logo=google&logoColor=ffffff" />
  <img src="https://img.shields.io/badge/Cloud_TPU_v4-1b1733?style=flat-square&logo=googlecloud&logoColor=4285F4" />
  <img src="https://img.shields.io/badge/Python-1b1733?style=flat-square&logo=python&logoColor=3776AB" />
  <img src="https://img.shields.io/badge/NVIDIA_NVML-1b1733?style=flat-square&logo=nvidia&logoColor=76B900" />
</p>

<br />

## 🧩 Selected projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>LLM services for Beijer Electronics</h3>
      <p>Commissioned student project in a team of five: an MCP server and insight backend that let Beijer's platforms use locally hosted LLMs, with GPU and CPU inference, a simulator and Dockerised deployment.</p>
      <img src="https://img.shields.io/badge/Python-1b1733?style=flat-square&logo=python&logoColor=3776AB" />
      <img src="https://img.shields.io/badge/C%23-1b1733?style=flat-square&logo=dotnet&logoColor=512BD4" />
      <img src="https://img.shields.io/badge/llama.cpp-1b1733?style=flat-square&logo=meta&logoColor=ffffff" />
      <img src="https://img.shields.io/badge/MCP-1b1733?style=flat-square&logo=anthropic&logoColor=ffffff" />
      <img src="https://img.shields.io/badge/Docker-1b1733?style=flat-square&logo=docker&logoColor=2496ED" />
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://g7studytracky.netlify.app">StudyTracky</a></h3>
      <p>A Pomodoro study app built with two classmates. Run focus sessions, add courses, see charts of how much you've studied and generate a quick AI quiz on what you just read. Everything stays in the browser, no account needed.</p>
      <img src="https://img.shields.io/badge/React-1b1733?style=flat-square&logo=react&logoColor=61DAFB" />
      <img src="https://img.shields.io/badge/Vite-1b1733?style=flat-square&logo=vite&logoColor=646CFF" />
      <img src="https://img.shields.io/badge/Recharts-1b1733?style=flat-square&logo=chartdotjs&logoColor=FF6384" />
      <img src="https://img.shields.io/badge/Netlify-1b1733?style=flat-square&logo=netlify&logoColor=00C7B7" />
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>GameVault</h3>
      <p>A Flutter app for keeping lists of every game you care about, with progress, ownership, prices and release dates in one place.</p>
      <img src="https://img.shields.io/badge/Flutter-1b1733?style=flat-square&logo=flutter&logoColor=02569B" />
      <img src="https://img.shields.io/badge/Dart-1b1733?style=flat-square&logo=dart&logoColor=0175C2" />
    </td>
    <td width="50%" valign="top">
      <h3>Healy</h3>
      <p>A rehab companion that helps patients and people who train follow their exercises, and gives physiotherapists a way to guide their patients.</p>
      <img src="https://img.shields.io/badge/Kotlin-1b1733?style=flat-square&logo=kotlin&logoColor=7F52FF" />
      <img src="https://img.shields.io/badge/Swift-1b1733?style=flat-square&logo=swift&logoColor=F05138" />
      <img src="https://img.shields.io/badge/React_Native-1b1733?style=flat-square&logo=react&logoColor=61DAFB" />
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>MazeGen</h3>
      <p>A maze generator and level editor our team of seven took over from a previous group and kept building on across sprints: custom levels you can create, play and test, a JUnit 5 test suite with Allure reports, and CI that runs the tests on every push.</p>
      <img src="https://img.shields.io/badge/Java-1b1733?style=flat-square&logo=openjdk&logoColor=ED8B00" />
      <img src="https://img.shields.io/badge/Maven-1b1733?style=flat-square&logo=apachemaven&logoColor=C71A36" />
      <img src="https://img.shields.io/badge/JUnit_5-1b1733?style=flat-square&logo=junit5&logoColor=25A162" />
      <img src="https://img.shields.io/badge/GitHub_Actions-1b1733?style=flat-square&logo=githubactions&logoColor=2088FF" />
    </td>
    <td width="50%" valign="top">
      <h3>YourAssistant</h3>
      <p>A scheduling web assistant built in a team of four, with a Java backend that scrapes and matches data, user login over HTTPS and a containerised deployment with Docker.</p>
      <img src="https://img.shields.io/badge/Java-1b1733?style=flat-square&logo=openjdk&logoColor=ED8B00" />
      <img src="https://img.shields.io/badge/JavaScript-1b1733?style=flat-square&logo=javascript&logoColor=F7DF1E" />
      <img src="https://img.shields.io/badge/Maven-1b1733?style=flat-square&logo=apachemaven&logoColor=C71A36" />
      <img src="https://img.shields.io/badge/Docker-1b1733?style=flat-square&logo=docker&logoColor=2496ED" />
    </td>
  </tr>
</table>

<details>
  <summary><b>Smaller builds from my .NET coursework</b></summary>
  <br />

  | Project | What it is | Stack |
  |---|---|---|
  | **BudgetMaster** | A personal-finance app that's nicer to look at than WinForms has any right to be | C#, Windows Forms |
  | **Taskmanager** | A to-do manager with file save/load and menus | C#, Windows Forms |
  | **PortfolioX** | A portfolio web app | ASP.NET, C#, HTML/CSS |
  | **Language Learner** | A cross-platform vocabulary app using MVVM | .NET MAUI, XAML |

</details>

<br />

## 🛠️ Toolbox

**Languages**
<br />
<img src="https://skillicons.dev/icons?i=go,ts,js,py,cs,java,c,kotlin,swift,dart&theme=dark" />

**Frontend & mobile**
<br />
<img src="https://skillicons.dev/icons?i=svelte,react,nuxtjs,tailwind,vite,html,css,tauri,flutter&theme=dark" />

**Backend & data**
<br />
<img src="https://skillicons.dev/icons?i=nodejs,spring,dotnet,postgres,redis,mysql,mongodb,nginx,cloudflare&theme=dark" />

**Tools**
<br />
<img src="https://skillicons.dev/icons?i=git,github,githubactions,docker,maven,linux,vscode,idea,visualstudio&theme=dark" />

<sub>Also worked with: Verilog/HDL, Assembly, Vaadin, .NET MAUI, Windows Forms, WPF and llama.cpp.</sub>

<br />

## 📈 Activity

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/OneAndOnlyWahidHassani/OneAndOnlyWahidHassani/output/snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/OneAndOnlyWahidHassani/OneAndOnlyWahidHassani/output/snake-light.svg" />
  <img alt="Contribution graph being eaten by a snake" src="https://raw.githubusercontent.com/OneAndOnlyWahidHassani/OneAndOnlyWahidHassani/output/snake-dark.svg" />
</picture>

<br />

## 🎲 Off the keyboard

Hiking around Skåne, gaming, reading, going far too deep into Warhammer 40K lore, and learning whatever caught my attention this week.

<br />

<p align="center">
  <sub>Always up for talking about side projects, LLM tooling or a good build. Say hej!</sub>
</p>
