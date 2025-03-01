---
title: Structural Optimization of Lattice Structures Using Neural Networks for Geometry Representation 
event: '3rd IACM Digital Twins in Engineering Conference (DTE 2025) &
1st ECCOMAS Artificial Intelligence and Computational Methods in Applied Science (AICOMAS 2025)'
event_url: https://dte_aicomas_2025.iacm.info/

location: Paris, France

abstract: 
# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2025-02-20T13:00:00Z'
#date_end: '2030-06-01T15:00:00Z'
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
Lattice structures consist of repeated, similarly shaped unit cells and are commonly found in modern engineering applications such as crash structures, acoustic components, or energy-efficient thermal applications. However, the design, analysis and optimization of such structures is still subject of current research. In this presentation we want to show how neural networks can be used to represent the geometry of the individual cells and how this enables an efficient optimization of spatially graded lattice structures. 

Unlike other lattice structure optimization methods, we neither assume a large separation of scale nor periodicity. Instead, we perform a full-scale finite element analysis (FEA) at each optimization step, which requires a large number of elements. Traditional topology optimization methods, such as SIMP, are not suitable because the large number of design parameters requires too many costly forward simulations. One approach to reduce the number of design parameters is to rely on shape optimization and define a parametrized unit cell using explicit geometrical representations, e.g. [1]. However, only a comparatively small set of geometries can be represented and finding a parametrization for complex geometries is not straight forward, especially if topological changes are desired. 

Instead, in our optimization approach, we employ the DeepSDF [2] method, where a continuous and low-dimensional latent space is introduced to encode the geometric information. Since each single unit cell is characterized by a different latent vector, a spatially graded lattice structure can subsequently be created by continuously varying the latent vector over the structure. A differentiable extension of the dual contouring algorithm [3] is used to transform the implicit representation to a computational mesh, which enables gradient based optimization. 

[1] Zwar, J., Elber, G. & Elgeti, S. Shape Optimization for Temperature Regulation in Extrusion Dies Using Microstructures. *Journal of Mechanical Design* 145, (2022). 
[2] Park, J. J., Florence, P., Straub, J., Newcombe, R. & Lovegrove, S. DeepSDF: Learning Continuous Signed Distance Functions for Shape Representation. *In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition* 165–174 (2019). 
[3] Shen, T. et al. Flexible Isosurface Extraction for Gradient-Based Mesh Optimization. *ACM Trans. Graph.* 42, 1–16 (2023).
