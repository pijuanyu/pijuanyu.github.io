---
title: "Investigating Passive Presentation Paradigms to Approximate Active Haptic Palpation"
authors:
- admin
- Luke C. Batteas
- Thomas K. Ferris
- M. Cynthia Hipwell
- Francis Quek
- Rebecca F. Friesen
author_notes:
# - "Equal contribution"
# - "Equal contribution"
date: "2025-08-07T00:00:00Z"
doi: "https://doi.org/10.1109/TOH.2024.3523259"
type: publication

# Schedule page publish date (NOT publication's date).
publishDate: "2024-12-26"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["Journal"]

# Publication name and optional abbreviated publication name.
publication: "IEEE Transactions on Haptics (Volume: 18, Issue: 1, Jan.-March 2025)"
publication_short: "IEEE Trans. Hapt (ToH)"

abstract: |
  Active, exploratory touch supports human perception of a broad set of invisible physical surface properties. When traditionally hands-on tasks, such as medical palpation of soft tissue, are translated to virtual settings, haptic perception is throttled by technological limitations, and much of the richness of active exploration can be lost. The current research seeks to restore some of this richness with advanced methods of passively conveying haptic data alongside synchronized visual feeds. 
  
  A robotic platform presented haptic stimulation modeled after the relative motion between a hypothetical physician's hands and artificial tissue samples during palpation. Performance in discriminating the sizes of hidden “tumors” in these samples was compared across display conditions which included haptic feedback and either: 1) synchronized video of the participant's hand, recorded during active exploration; 2) synchronized video of another person's hand; 3) no accompanying video. 
  
  The addition of visual feedback did not improve task performance, which was similar whether receiving relative motion recorded from one's own hand or someone else's. While future research should explore additional strategies to improve task performance, this initial attempt to translate active haptic sensations to passive presentations indicates that visuo-haptic feedback can induce reliable haptic perceptions of motion in a stationary passive hand.

# Summary. An optional shortened abstract.
summary: We explored how passive users can perceive active palpation tasks via synchronized visual/haptic feedback from a robotic platform. While passive conditions showed slight decreases in perceptual acuity, many participants reported strong ownership/kinesthetic illusions, suggesting potential for immersive "passive immersion" in hands-on experiences.

tags:
- Journal articles
featured: true

# links:
# - name: ""
#   url: ""
url_pdf: 'uploads/Pijuan_Palpation_Paper_Draft_ToH_version.pdf'
url_code: 'https://github.com/pijuanyu/3D-platform-for-lump-detection'
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: 'https://www.youtube.com/watch?v=TbYN0pEvcNg'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Passive presentation of an active task: a passive user observes video of active hand motion while a 2D robotic platform recreates the relative motion between the hand and object.'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: [robotics/testbedv0]

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: example
---

{{< youtube id="TbYN0pEvcNg" title="Synchronized Visual-haptic Feedback" >}}