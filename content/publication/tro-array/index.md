---
title: "Towards High Fidelity Remote Palpation System"
authors:
  - admin
  - Gwilym Couch
  - Thomas K. Ferris
  - M. Cynthia Hipwell
  - Rebecca F. Friesen
date: "2026-02-11T00:00:00Z"
doi: ""
type: publication
# Schedule page publish date (NOT publication's date).
publishDate: "2026-02-11T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["IEEE Transactions on Robotics"]

# Publication name and optional abbreviated publication name.
publication: "Submiited to IEEE Transactions on Robotics"
publication_short: "Submiited to IEEE Trans. Robotics (T-RO)"

abstract: |

  Remote palpation enables noninvasive tissue examination in telemedicine, yet current tactile displays often lack the fidelity to convey both large-scale forces and fine spatial details. This study introduces a hybrid fingertip display comprising a rigid platform and a 4x4 soft pneumatic tactile display (4.93 mm displacement and 1.175 N per single pneumatic chamber) to render a hard lump beneath soft tissue. This study compares three rendering strategies: a Platform-Only baseline that renders the total interaction force; a Hybrid A (Position + Force Feedback) strategy that adds a dynamic, real-time soft spatial cue; and a Hybrid B (Position + Preloaded Stiffness Feedback) strategy that provides a constant, pre-calculated soft spatial cue.

  Psychophysical evaluations with 12 participants assessed lump detection and size discrimination using soft tissue phantoms. Detection accuracy increased from 50.0% (Platform-Only) to around 98% (Hybrid A and B), with elevated confidence and realism attributed to contact area modulation. Size discrimination accuracy reached 86.1% (Hybrid A) versus 63.9% (Platform-Only), underscoring the role of temporal-spatial cues in edge perception. Future efforts will enable real-time teleoperation, diverse tissue testing, and clinician validation. 

# Summary. An optional shortened abstract.
summary: In this study, we proposed a ROS 2 telepalpation system by integrating a 4x4 soft pneumatic array on a rigid platform; implemented a novel mapping algorithm where OptiTrack motion data drives the stage and K-Means clustered high-resolution tactile sensing data drives the pneumatics.

tags:
- Journal articles

featured: true

links:
# - name: Custom Link
#   url: http://example.org
url_pdf: 
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'High Resolution Tactile Sensing and Display'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: example
---

<!-- This work is driven by the results in my [previous paper](/publication/conference-paper/) on LLMs.

{{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
