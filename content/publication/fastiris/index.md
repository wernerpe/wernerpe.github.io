---
title: 'Faster Algorithms for Growing Collision-Free Convex Polytopes in Robot Configuration Space'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
    - Peter Werner
    - Thomas Cohn*
    - Rebecca H. Jiang*
    - Tim Seyde
    - Max Simchowitz
    - Russ Tedrake
    - Daniela Rus
    
# Author notes (optional)
# author_notes:
#   - 'Equal contribution'
#   - 'Equal contribution'

date: '2024-10-01T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
#publication: In *Wowchemy Conference*
#publication_short: In *ICW*

abstract: We propose two novel algorithms for constructing convex collision-free polytopes in robot configuration space. Finding these polytopes enables the application of stronger motion-planning frameworks such as trajectory optimization with Graphs of Convex Sets [1] and is currently a major roadblock in the adoption of these approaches. In this paper, we build upon IRIS-NP (Iterative Regional Inflation by Semidefinite & Nonlinear Programming) [2] to significantly improve tunability, runtimes, and scaling to complex environments. IRIS-NP uses nonlinear programming paired with uniform random initialization to find configurations on the boundary of the free configuration space. Our key insight is that finding near-by configuration-space obstacles using sampling is inexpensive and greatly accelerates region generation. We propose two algorithms using such samples to either employ nonlinear programming more efficiently (IRIS-NP2 ) or circumvent it altogether using a massively-parallel zero-order optimization strategy (IRIS-ZO). We also propose a termination condition that controls the probability of exceeding a user-specified permissible fraction-in-collision, eliminating a significant source of tuning difficulty in IRIS-NP. We compare performance across eight robot environments, showing that IRIS-ZO achieves an order-of-magnitude speed advantage over IRIS-NP. IRISNP2, also significantly faster than IRIS-NP, builds larger polytopes using fewer hyperplanes, enabling faster downstream computation.

# Summary. An optional shortened abstract.
summary: We propose two new algorithms for constructing collision-free convex polytopes in robot configuration space. Our key insight is that finding near-by configuration-space obstacles using sampling is inexpensive and greatly accelerates region generation. Our two algorithms use such samples to either employ nonlinear programming more efficiently (IRIS-NP2 ) or circumvent it altogether using a massively-parallel zero-order optimization strategy (IRIS-ZO). We show that IRIS-ZO achieves an order-of-magnitude speed advantage over its predecessor IRIS-NP. IRISNP2, also significantly faster than IRIS-NP, builds larger polytopes using fewer hyperplanes, enabling faster downstream computation. <font size="4"> <br> *[arXiv, 2024]*</font>

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
links:
 - name: Website
   url: 'https://sites.google.com/view/fastiris/home'

url_pdf: 'https://arxiv.org/abs/2410.12649'
# url_code: 'https://github.com/AlexandreAmice/drake/tree/iris_from_clique_cover/cspace_lightweight'
#url_dataset: 'https://github.com/wowchemy/wowchemy-hugo-themes'
#url_poster: ''
#url_project: ''
#url_slides: ''
#url_source: 'https://github.com/wowchemy/wowchemy-hugo-themes'
# url_video: 'https://www.youtube.com/watch?v=x37fPVST6Zk'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
#   - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
#slides: example
---
<!-- 
{{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}} -->

<!-- Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://wowchemy.com/docs/content/writing-markdown-latex/). -->
