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
              icon: brands/python
            - name: MATLAB
              icon: custom/matlab
            - name: R
              icon: brands/r
            - name: SQL
              icon: hero/circle-stack
            - name: JavaScript
              icon: brands/javascript
            - name: VBA
              icon: brands/microsoftexcel
        - name: AI & Machine Learning
          items:
            - name: PyTorch
              icon: brands/pytorch
            - name: RAG Pipelines
              icon: custom/rag-pipelines
            - name: LLM Evaluation
              icon: custom/llm-evaluation
            - name: Prompt Engineering
              icon: brands/openai
            - name: Synthetic Data Generation
              icon: hero/cpu-chip
            - name: TensorFlow
              icon: brands/tensorflow
        - name: Data & Medical Imaging
          items:
            - name: OpenCV
              icon: brands/opencv
            - name: NumPy
              icon: brands/numpy
            - name: pandas
              icon: brands/pandas
            - name: scikit-learn
              icon: brands/scikitlearn
            - name: Tableau
              icon: brands/tableau
            - name: Medical Imaging
              icon: custom/xray
        - name: Cloud & Infrastructure
          items:
            - name: AWS
              icon: brands/amazonwebservices
            - name: Git
              icon: brands/git
            - name: Linux
              icon: brands/linux
        - name: Engineering Software
          items:
            - name: Fusion 360
              icon: brands/autodesk
            - name: AutoCAD
              icon: brands/autocad
            - name: LabVIEW
              icon: brands/labview
            - name: COMSOL Multiphysics
              icon: custom/comsol
            - name: Onshape
              icon: hero/cube
            - name: SolidWorks
              icon: brands/dassaultsystemes
    design:
      style: grid

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
