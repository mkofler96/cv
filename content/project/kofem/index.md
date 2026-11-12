---
title: KoFEM
summary: >-
  Open-source finite element analysis in the browser. Import a STEP file, mesh
  it, apply supports and loads, and solve locally, with no installation and no
  data leaving your machine. A C++ pipeline (OpenCASCADE, Netgen, MFEM) compiled
  to WebAssembly, with a React + Three.js frontend.

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
  caption: 'KoFEM running in the browser'
  focal_point: Center
---

[KoFEM](https://kofem.org/) is an open-source, browser-based finite element solver.

- **Runs in your browser.** No installation; models are solved locally and never uploaded to a server.
- **Full pipeline.** STEP geometry → OpenCASCADE tessellation → Netgen volume mesh → MFEM solve.
- **Tech.** C++ engine compiled to WebAssembly, an experimental Rust FEM module, and a React + Three.js frontend.
- **License.** AGPL-3.0-or-later. Source code on [GitHub](https://github.com/mkofler96/KoFEM).
