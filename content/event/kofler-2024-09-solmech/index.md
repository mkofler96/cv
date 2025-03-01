---
title: Optimization of the Spatially Graded Superelastic Lattice in a Morphing Structure
event: 43rd Solid Mechanics Conference 
event_url: https://solmech.pl/

location: Wrocław, Poland

abstract: 
# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2024-09-18T13:00:00Z'
#date_end: '2030-06-01T15:00:00Z'
all_day: true

# Schedule page publish date (NOT talk date).
publishDate: '2017-01-01T00:00:00Z'
authors:
  - admin
  - Marius Schasching
  - Ondrej Cervinek
  - Tim Munhowen
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
The aerodynamic efficiency in different flight conditions can be increased by morphing the wings. Morphing wings require high deformability and high strain recoverability, both of which can be achieved by
using optimized structures made of additive manufactured superelastic lattice materials. To obtain an
optimized structure of such a wing for certain flight conditions, a mechanical structural optimization of
the corresponding trailing edge is presented.

The optimization of the wing is challenging due to the geometric nonlinearities resulting from the desired
large geometric deformations as well as the highly nonlinear relationship between stress and strain of the
superelastic material. The latter requires adequate material models to capture the response of the experimentally characterized parent material, which often deviates from the idealized constitutive relations.
For the optimization, additional complexity arises from the large difference in scale between the desired
structure and a single lattice cell.

The resulting multiscale optimization problem is addressed by first optimizing the design of the single
lattice cell, where both shape and topology optimization methods are employed. The unit cell is then
parametrized, to allow a grading over the whole structure. To handle the nonlinear structural response,
the capabilities of the commercial tools ABAQUS 2023/Standard (*Dassault Systemes Simulia Corp.*, 
Providence, RI, USA) and Tosca 2023 (*Dassault Systemes Simulia Corp.*, Providence, RI, USA) are used.
Further optimization of the macroscopic structure is limited in Tosca. However, the use of beam elements, which is often more efficient than the use of continuum elements, is an initial step toward a
custom optimization process. To give adequate predictions using beam-based models, a user-defined
uniaxial hypoelastic material model is implemented to account for the superelastic constitutive behavior.
The results show that superelastic materials can be used in the optimization-driven design of parts of a
morphing wing. Furthermore, the capabilities of analyzing the mechanical response of lattice materials
by means of beam-based representations in combination with hypoleastic material models are investigated.

**ACKNOWLEDGEMENT**: *The funding of the project ”Building Actions in Smart Aviation with Environmental Gains” by the European Union Programme Horizon Europe under grant agreement no.
101079091 is gratefully acknowledged. The computational results presented have been achieved using
the Vienna Scientific Cluster (VSC).*
