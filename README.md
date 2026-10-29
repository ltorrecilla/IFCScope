<p align="center">
  <a href="https://liteaeco.com/">LiteAeco website</a>
  |
  <a href="https://liteaeco.com/news/">News</a>
  |
  <a href="https://liteaeco.com/info/about.html">About</a>
  |
  <a href="https://liteaeco.com/info/faqs.html">FAQ</a>
  |
  <a href="https://liteaeco.com/info/fund.html">Support</a>
</p>

<h1><img src="https://raw.githubusercontent.com/ltorrecilla/liteaeco/refs/heads/main/img/favicon.ico" width="32"/> Open Source AECO Tools</h1>

## What you will find:
[**liteAECO**](https://liteAECO.com/tools/ifc-viewer-audit.html) · [live](https://liteAECO.com/)
> Here you can find all the files and documentation of the IFC Viewer to continue the development, including all files to deploy it on your own server.
- IFCScope
  - The IFC Viewer is based on web-ifc, more specific the ThatOpen Engine
  - Coordinate several Ifc Models
  - Explore attributes and export element list and schedules
  - Run clash detection over the pairs you want with filtering options
  - Link external excel data to elements in the model
  - Create BCF files or review existing ones

- Source repo, not dist/. Built from the import graph of the page + main.js (2026-10-19).
  - Root
  - package.json, package-lock.json
  - vite.config.js

- Runtime assets (from npm, at build time)
  - web-ifc wasm: served from /src/ (getWasmBasePath() in main.js). Check how it lands in src/ (copy step or public folder) and keep that in the repo.
  - Fragments worker: OBC.FragmentsManager.getWorker() loads from unpkg; src/worker.mjs copy also built.
  - cls_worker.js: copied as a plain file (worker URL built at runtime).
- npm packages (versions from package.json)
  - three, three-viewport-gizmo
  - @thatopen/components, @thatopen/components-front, @thatopen/fragments (3.4.5), @thatopen/ui
  - web-ifc (0.0.77, pinned)
- CDN (no files)
  - Tailwind (cdn.tailwindcss.com)
  - Tabulator 6.2.1 (cdnjs)

## Support the development
Making BIM available for free & open-source, you can support the project via:

[![Ko-fi](https://img.shields.io/badge/%E2%98%95-ko-fi)](https://ko-fi.com/ltorrecilla)

## Contact

- LiteAECO: [liteAECO](https://liteAECO.com)  
- LinkedIn: [Luis Torrecilla](https://www.linkedin.com/in/ltorrecilla)  
- Email: hello@liteaeco.com

## Want to help?

You are welcome! Please get in contact at hello@liteaeco.com
