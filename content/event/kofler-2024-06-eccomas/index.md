---
title: Application of Structural Optimization on Lattice Structure Design using Superelastic Material

event: 9th European Congress on Computational Methods in Applied Sciences and Engineering
event_url: https://eccomas2024.org/

location: Lisboa, Portugal

summary: An example talk using Hugo Blox Builder's Markdown slides feature.
abstract: 
# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2024-06-03T13:00:00Z'
#date_end: '2030-06-01T15:00:00Z'
all_day: true

# Schedule page publish date (NOT talk date).
publishDate: '2017-01-01T00:00:00Z'

authors:
  - admin
  - Marius Schasching
  - Ondrej Cervinek
  - Florian Zwicke
  - Daniel Koutny
  - Heinz Pettermann
  - Melanie Todt

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

In order to increase aerodynamic efficiency, it is desirable to change the shape of the contour of the wings of an airplane for different flight conditions. This for example can be achieved by a compliant structure, which can be deformed without joints. In this presentation, the mechanical structural optimization of such a compliant mechanism is presented. To achieve high deformability, a lattice structure geometry is developed, consisting of repeated unit cells. For the material, the superelastic Nitinol is chosen, which allows high strain recoverability and maximum strength. However, its nonlinear relation between stress and strain, as well as the geometric nonlinearities resulting from the desired large geometric deformations, make the formulation and solution of the optimization problem challenging. Additional analysis and optimization complexity arise from the large difference in length scale between the whole structure and a single unit cell. This multiscale optimization problem is addressed by first optimizing the design of the unit cell, where both shape and topology optimization methods are employed. The unit cell is then parametrized, to allow a grading of its shape over the whole structure. To handle the nonlinear structural response, the capabilities of the commercial tools Abaqus and Tosca are used. 

**ACKNOWLEDGEMENTS**: *The funding of the project “Building Actions in Smart Aviation with Environmental Gains” by the European Union Programme Horizon Europe under grant agreement no. 101079091 is gratefully acknowledged. The computational results presented have been achieved using the Vienna Scientific Cluster (VSC).*

