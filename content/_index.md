---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
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
        about: Basic Information
        education: Education
        interests: Research Interests
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: 'About'
      subtitle: ''
      text: |-
        Welcome to my academic homepage.
        
        This website includes my basic profile, educational background, CV, and selected publications.
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Selected Publications
      text: 'Each publication can show title, authors, a short summary, and a featured image.'
      count: 20
      filters:
        folders:
          - publications
    design:
      view: article-grid
      columns: 3
---
