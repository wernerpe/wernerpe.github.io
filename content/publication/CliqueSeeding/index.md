---
title: 'Approximating Robot Configuration Spaces with few Convex Sets using Clique Covers of Visibility Graphs'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
    - Peter Werner
    - Alexandre Amice
    - Tobia Marcucci
    - Daniela Rus
    - Russ Tedrake
    
# Author notes (optional)
# author_notes:
#   - 'Equal contribution'
#   - 'Equal contribution'

date: '2023-08-01T00:00:00Z'
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

abstract: Many computations in robotics can be dramatically accelerated if the robot configuration space is described as a collection of simple sets. For example, recently developed motion planners rely on a convex decomposition of the free space to design collision-free trajectories using fast convex optimization. In this work, we present an efficient method for approximately covering complex configuration spaces with a small number of polytopes.The approach constructs a visibility graph using sampling and generates a clique cover of this graph to find clusters of samples that have mutual line of sight. These clusters are then inflated into large, full-dimensional, polytopes. We evaluate our method on a variety of robotic systems and show that it consistently covers larger portions of free configuration space, with fewer polytopes, and in a fraction of the time compared to previous methods.

# Summary. An optional shortened abstract.
summary: We propose an algorithmic appraoch to approximating robot configuration space with a small collection of convex sets. First, the algorithm constructs a visibility graph using sampling, then a small clique cover of the visibility graph is computed, and finally the cliques are inflated to full-dimensional polytopes that are collision free. <font size="4"> <br> *[arXiv, 2023]*</font>

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/abs/2310.02875'
#url_code: 'https://github.com/tseyde/decqn'
#url_dataset: 'https://github.com/wowchemy/wowchemy-hugo-themes'
#url_poster: ''
#url_project: ''
#url_slides: ''
#url_source: 'https://github.com/wowchemy/wowchemy-hugo-themes'
#url_video: 'https://youtu.be/HbDL8EWZ5h8'

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
