<p align="center">
  <img src="./assets/hero.svg" width="100%" alt="Peephole — Explore before you clone. Analyze public GitHub repositories and preview eligible projects in isolation." />
</p>
<p align="center">
  <img src="./assets/peephole-128" width="100%" alt="Peephole Logo" />
</p>
<p align="center">
  <strong>Understand a public GitHub repository before cloning it.</strong><br />
  Inspect its stack, structure, requirements, and preview eligibility — right inside GitHub.
</p>

<p align="center">
  <a href="https://chromewebstore.google.com/detail/peephole/fieofkhijgngfoflgpkbghbkaidhdgel"><strong>Install for Chrome</strong></a>
  &nbsp; · &nbsp;
  <a href="https://github.com/The-peephole/peephole"><strong>Explore the source</strong></a>
  &nbsp; · &nbsp;
  <a href="https://github.com/The-peephole/peephole/releases/latest"><strong>Releases</strong></a>
</p>

<p align="center">
  <a href="./README.ko.md">한국어 소개</a>
</p>

---

### A clearer first look at any public repository

| Inspect | Choose | Preview |
| :--- | :--- | :--- |
| Discover frameworks, package managers, repository structure, backend dependencies, and blockers. | Explore supported branches and frontend/backend targets, with analysis pinned to an exact commit. | Build eligible frontends in isolated gVisor sandboxes and inspect the result inside a Chrome Side Panel. |

<p align="center">
  <img src="https://raw.githubusercontent.com/The-peephole/peephole/main/image/peephole-demo.gif" width="880" alt="Peephole repository analysis and static frontend preview in the GitHub Side Panel" />
</p>

<p align="center"><sub>Static preview demonstration. Full-stack preview is not shown in this recording.</sub></p>

### Designed for real-world repository discovery

- **Repository intelligence:** Understand a project's detected stack, build plan, environment requirements, and compatibility without starting with a clone.
- **Scoped execution:** Supported static projects can be built and previewed; a narrower Vite + React frontend and Express backend shape also supports full-stack previews.
- **Temporary dependencies:** Supported full-stack flows can use an ephemeral PostgreSQL database and non-sensitive configuration under their documented constraints.
- **Explicit limitations:** Unsupported frameworks, backend combinations, and other repositories remain analysis-only, with reasons rather than a misleading runnable preview.

**Preview support is deliberately narrower than analysis support.** See the [supported-project matrix](https://github.com/The-peephole/peephole#supported-projects) for exact requirements and exclusions.

### Built with isolation in mind

Peephole treats repository code and dependency scripts as untrusted. Previews are commit-pinned, built or run in resource-limited **gVisor** sandboxes, and delivered over isolated HTTPS origins. The backend and extension have different trust boundaries.

These controls reduce risk; they are not a claim that arbitrary code is safe to execute. See the project's [security model](https://github.com/The-peephole/peephole#security-model) and [verification status](https://github.com/The-peephole/peephole#current-verification) for evidence, remaining limitations, and release-stage distinctions.

### Get started

1. [Install Peephole](https://chromewebstore.google.com/detail/peephole/fieofkhijgngfoflgpkbghbkaidhdgel) and visit a **public** GitHub repository.
2. Open **Peephole** from the repository action area and inspect the analysis in the Side Panel.
3. For a supported target, connect GitHub when prompted and start the available preview flow.

<p align="center">
  <a href="https://github.com/The-peephole/peephole#readme">Documentation</a>
  &nbsp; · &nbsp;
  <a href="https://github.com/The-peephole/peephole/issues">Issues & feedback</a>
  &nbsp; · &nbsp;
  <a href="https://github.com/The-peephole/peephole/actions/workflows/ci.yml">CI</a>
</p>

<p align="center"><sub>Open source, built for developers who want to explore before they clone.</sub></p>
