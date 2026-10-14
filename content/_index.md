---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-10-06
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a file name within `data/authors/`)
      username: me
      text: ''
      button:
        text: Download CV
        url: uploads/cv.pdf
      headings:
        about: 'About'
        education: 'Education'
        interests: 'Interests'
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: medium
        shape: circle
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      count: 5
      filters:
        folders:
          - news
      order: desc
    design:
      view: date-title-summary
      columns: '1'
---
