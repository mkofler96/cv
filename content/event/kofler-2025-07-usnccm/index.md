---
title: Optimization of Lattice Structures Using Neural Networks as Immersed Boundary Representations 
event: '18th U.S. National congress on computational mechanics'
event_url: https://usnccm18.usacm.org/

location: Chicago, US

abstract: 
# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2025-07-21T10:00:00Z'
#date_end: '2030-06-01T15:00:00Z'
all_day: true

# Schedule page publish date (NOT talk date).
publishDate: '2017-01-01T00:00:00Z'

authors:
  - admin
  - Maute, Kurt 
  - Wunsch, Nils
  - Evans, John
  - Elgeti, Stefanie

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
links: 
  - name: Zenodo
    url: 'https://zenodo.org/records/16903138'

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
Lattice structures consist of repeated similar shaped unit cells and are commonly found in modern engineering applications such as crash structures, acoustic components, or energy-efficient thermal applications. However, the design, analysis and optimization of such structures is still subject of current research. In this presentation we want to show how neural networks can be used to implicitly define their geometry and how immersed boundary methods can be used to analyse their physical behaviour as a part of an optimization process.
Unlike other lattice structure optimization methods, we neither assume a large separation of scale nor periodicity. Instead, in each optimization step we perform a full-scale structural analysis. In theory, this enables the use of conventional topology optimization methods such as e.g. the SIMP or the Level-Set method. However, the complex geometry of lattice structures results in an infeasible high number of design parameters.  
One approach to reduce the number of design parameters is to rely on shape optimization and define a parametrized unit cell using explicit geometrical representations, e.g. [1]. However, only a comparatively small set of geometries can be represented and finding a parametrization for complex geometries is not straight forward, especially if topological changes are desired. 
In our approach, we employ the DeepSDF [2] method, where a continuous and low-dimensional latent space is introduced to encode the geometric information. Since each single unit cell is characterized by a different latent vector, a spatially graded lattice structure can be created by continuously varying the latent vector over the structure. The neural network is then used to map the geometry from the latent space back to its signed distance representation. This geometrical definition makes this approach especially suited for immersed boundary methods.

[1] Zwar, J., Elber, G. & Elgeti, S. Shape Optimization for Temperature Regulation in Extrusion Dies Using Microstructures. *Journal of Mechanical Design* 145, (2022). 
[2] Park, J. J., Florence, P., Straub, J., Newcombe, R. & Lovegrove, S. DeepSDF: Learning Continuous Signed Distance Functions for Shape Representation. *In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition* 165–174 (2019).