---
title: ''
summary: ''
date: 2022-10-24
type: landing
sections:
  - block: resume-biography-3
    content:
      username: me
      text: ''
      button:
        text: Download Resume
        url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      name:
        size: md
      avatar:
        size: medium
        shape: circle

  - block: resume-experience
    id: experience
    content:
      username: me
    design:
      date_format: 'January 2006'
      is_education_first: false

  - block: tech-stack
    id: skills
    content:
      title: Technical Skills
      username: me
    design:
      style: grid

  - block: collection
    id: projects
    content:
      title: Featured Projects
      filters:
        folders:
          - projects
      sort_ascending: true
    design:
      view: article-grid
      fill_image: false
      columns: 3
      show_date: false
      show_read_time: false
      show_read_more: false
---
