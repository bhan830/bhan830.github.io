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
      title: Skills and Qualifications
      categories:
        - name: Programming
          items:
            - name: Python
            - name: MATLAB
            - name: R
            - name: SQL
            - name: JavaScript
        - name: AI & Machine Learning
          items:
            - name: PyTorch
            - name: RAG Pipelines
            - name: LLM Evaluation
            - name: Prompt Engineering
            - name: Synthetic Data Generation
            - name: TensorFlow
        - name: Data & Medical Imaging
          items:
            - name: OpenCV
            - name: NumPy / pandas
            - name: scikit-learn
            - name: Tableau
            - name: Medical Imaging
        - name: Cloud & Infrastructure
          items:
            - name: AWS
            - name: Git
            - name: Linux
    design:
      style: list

  - block: collection
    id: projects
    content:
      title: Selected Projects
      filters:
        folders:
          - projects
    design:
      view: article-grid
      fill_image: false
      columns: 3
      show_date: false
      show_read_time: false
      show_read_more: false
---
