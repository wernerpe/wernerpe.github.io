---
title: 'Superfast Configuration-Space Convex Set Computation on GPUs for Online Motion Planning'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
    - Peter Werner
    - Richard Cheng
    - Tom Stewart
    - Russ Tedrake
    - Daniela Rus
    
# Author notes (optional)
# author_notes:
#   - 'Equal contribution'
#   - 'Equal contribution'

date: '2024-12-01T00:00:00Z'
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

abstract: In this work, we leverage GPUs to construct probabilistically collision-free convex sets in robot configuration space on the fly. This extends the use of modern motion planning algorithms that leverage such representations to changing environments. These planners rapidly and reliably optimize high-quality trajectories, without the burden of challenging nonconvex collision-avoidance constraints. We present an algorithm that inflates collision-free piecewise linear paths into sequences of convex sets (SCS) that are probabilistically collision-free using massive parallelism. We then integrate this algorithm into a motion planning pipeline, which leverages dynamic roadmaps to rapidly find one or multiple collision-free paths, and inflates them. We then optimize the trajectory through the probabilistically collision-free sets, simultaneously using the candidate trajectory to detect and remove collisions from the sets. We demonstrate the efficacy of our approach on a simulation benchmark and a KUKA iiwa 7 robot manipulator with perception in the loop. On our benchmark, our approach runs 17.1 times faster and yields a 27.9% increase in reliability over the nonlinear trajectory optimization baseline, while still producing high-quality motion plans.
# Summary. An optional shortened abstract.
summary: We leverage GPUs to create probabilistically collision-free convex sets in configuration space on-the-fly, enabling high-quality trajectory optimization without challenging collision avoidance constraints. Our approach runs 17× faster with 28% higher reliability than traditional methods, validated on both simulations and a KUKA robot with real-time perception. <font size="4"> <br> *[RSS, 2025]*</font>

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
links:
 - name: Website
   url: 'https://sites.google.com/view/gpupolytopes/home'

url_pdf: 'https://arxiv.org/abs/2504.10783'
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
