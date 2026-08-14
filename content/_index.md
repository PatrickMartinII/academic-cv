---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-08-03
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: ' '
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        image: 
          filename: night_sky.jpg
          size: cover
          position: center
        text_color_light: true
        gradient_mesh:
          enable: true
      spacing: 
        padding: ['0', '0', '3rem', '0']

      # Name heading sizing to accommodate long or short names
      name:
        size: sm # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: large # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: '📚 Current Research'
      subtitle: ''
      text: |-
        Hypergraph and graph invariants can be categorified into (co)homology theories which usually capture more information and exhibit a depth that the original invariant cannot reach via the torsion subgroups which can appear. Of the invariants which have been categorified, particular interest has bee garnered in the magnitude and chromatic polynomial of a hypergraph/graph. 

        Although richer and more versatile, these categorifications typically require an immense computational cost. The aim then is to use algrbraic tools to simplify the complexes to smaller homotopy equivalent complexes in order to reduce the computations. Then these tools can be directed towards interpreting large datasets which can be represented by a hypergraph. 
    design:
      columns: '1'
#  - block: collection
#    id: papers
#    content:
#      title: Featured Publications
#      filters:
#        folders:
#          - publications
#        featured_only: true
#    design:
#      view: article-grid
#      columns: 2
  - block: collection
    id: papers
    content:
      title: Preprints and Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
---
