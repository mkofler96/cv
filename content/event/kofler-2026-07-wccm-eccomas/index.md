---
title: Optimization of Lattice Structures for a Morphing Wing Using Neural Implicit Geometry
event: WCCM-ECCOMAS 2026
event_url: https://wccm-eccomas2026.org/event/contribution/a1b5bd96-df17-11f0-b205-000c29ddfc0c

location: Munich, Germany

abstract: 
# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2026-07-19T00:00:00Z'
#date_end: '2026-07-24T23:59:59Z'
all_day: true

# Schedule page publish date (NOT talk date).
publishDate: '2017-01-01T00:00:00Z'

authors:
  - admin
  - Stefanie Elgeti

tags: []

# Is this a featured talk? (true/false)
featured: false

#image:
#  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/bzdhc5b3Bxs)'
#  focal_point: Right

#links:
#  - icon: twitter
#    icon_pack: fab
#    name: Follow
#    url: https://twitter.com/georgecushen
url_pdf: ''

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
---
Lattice structures consist of repeated, similar-shaped unit cells and are commonly found in modern engineering applications such as crash structures, acoustic components, or energy-efficient thermal applications. However, the design, analysis and optimization of such structures is still subject of current research. In this presentation we want to show how neural networks can be used to implicitly represent and optimize the geometry of spatially graded lattice structures [1].

We employ the DeepSDF [2] method, where a continuous and low-dimensional latent space is introduced to encode the geometric information. In contrast to traditional topology optimization methods, this allows the restriction of the design space to specific geometries. In our case, the latent space is used to represent the geometry of different unit cells, that are stacked to form a lattice structure. Moreover, continuously varying the latent vector over the structure allows a functional grading and optimization.

Unlike other lattice-structure optimization methods, we neither assume a large separation of scale nor periodicity. Instead, we perform a full-scale finite element analysis at each optimization step. The required mesh is obtained by a differentiable extension of the dual marching cubes algorithm [3], which enables gradient-based optimization. We demonstrate the effectiveness of the proposed method on a morphing wing example.

[1] Kofler, M., Giritsch, M. & Elgeti, S. Structural optimization of lattice structures using deep neural networks as geometry representation. *Graphical Models* 142, 101307 (2025).
[2] Park, J. J., Florence, P., Straub, J., Newcombe, R. & Lovegrove, S. DeepSDF: Learning Continuous Signed Distance Functions for Shape Representation. *In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition* 165–174 (2019).
[3] Shen, T. et al. Flexible Isosurface Extraction for Gradient-Based Mesh Optimization. *ACM Trans. Graph.* 42, 1–16 (2023).
