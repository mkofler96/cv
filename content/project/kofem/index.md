---
title: KoFEM
summary: >-
  Open-source finite element analysis directly in the browser. Supports geometry
  import, meshing, load application and postprocessing, all without installation
  or cloud servers. Enabled by compiling existing C++ frameworks such as
  OpenCASCADE, Netgen and MFEM to WebAssembly and calling them with a
  React + Three.js frontend.

date: '2026-05-12T00:00:00Z'

authors:
  - admin

tags:
  - Finite Element Method
  - WebAssembly
  - Open Source

# Clicking the project card opens the KoFEM website.
external_link: https://kofem.org/

links:
  - name: Website
    url: https://kofem.org/
  - name: Code
    url: https://github.com/mkofler96/KoFEM

image:
  caption: 'KoFEM logo'
  focal_point: Center
  # Show the logo whole (not cropped) on narrow screens. featured.png has a
  # transparent background, so the card's own color shows through in both
  # light and dark mode.
  background: transparent
---

[KoFEM](https://kofem.org/) is an open-source, browser-based finite element solver.

- **Runs in your browser.** No installation; models are solved locally and never uploaded to a server.
- **Full pipeline.** STEP geometry → OpenCASCADE tessellation → Netgen volume mesh → MFEM solve.
- **Tech.** C++ engine compiled to WebAssembly, an experimental Rust FEM module, and a React + Three.js frontend.
- **License.** AGPL-3.0-or-later. Source code on [GitHub](https://github.com/mkofler96/KoFEM).
