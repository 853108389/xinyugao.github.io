---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography
    content:
      # Choose a user profile to display (a folder name within `content/authors/`) #
      username: Xinyu Gao
      text: "I am currently a Ph.D. student in the Department of Software Engineering, Nanjing University, advised by Prof. Yang Feng, Zhenyu Chen and Prof. Baowen Xu. My research focuses on reliability assurance of the AI-enabled complex software systems within the field of Software Engineering (SE). Recently, my work has explored testing, analysis, and repair for multi-sensor fusion based perception systems in autonomous driving. My work has been published in top-tier SE venues (e.g., ICSE, FSE, ASE, ISSTA)  and has received a distinguished paper award (FSE '23)."
      # Show a call-to-action button under your biography? (optional)
#      button:
#        text: Download CV
#        url: uploads/resume.pdf
    design:
#      css_class: "bg-primary-700"
      spacing:
        padding: [0, 0, 0, 0]
      biography:
        style: 'text-align: justify; font-size: 1em;'
        

#    design:
#      css_class: dark
#      background:
#        color: black
#        image:
#          # Add your image background to `assets/media/`.
#          filename: stacked-peaks.svg
#          filters:
#            brightness: 1.0
#          size: cover
#          position: center
#          parallax: false
      
#  - block: markdown
#    content:
#      title: '📚 My Research'
#      subtitle: ''
#      text: |-
#        Use this area to speak to your mission. I'm a research scientist in the Moonshot team at DeepMind. I blog about machine learning, deep learning, and moonshots.
#
#        I apply a range of qualitative and quantitative methods to comprehensively investigate the role of science and technology in the economy.
#        
#        Please reach out to collaborate 😃
#    design:
#      columns: '1'
  


  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
      count: 2
      
    design:
      view: article-grid
      columns: 2
      
  - block: collection
    content:
      title: Recent Publications
      text: ""
      sort_by: sort_weight
      sort_ascending: false
      filters:
        folders:
          - publication
        exclude_featured: false
      count: 1000
      archive:
        enable: true
    design:
      view: citation   # 这个是影响不同collection渲染逻辑的页面
      columns: 1
  
  # 只能用属性传递，用内容传递，内容会显示成代码块，没办法解析,(应该是我不会，而不是不能)
  - block: markdown
    content:
      title: 'Award and Honors'
      text: |
        {{% honors
            line1="ACM SIGSOFT Distinguished Paper Award (ESEC/FSE'23)"
            line2="National Scholarship for Postgraduate Students (2021)"
            line3="China Scholarship Council (CSC) scholarships. (2023)"
            line4="NR Scholarship Talents Scholarship by Nanjing University (2024)"
            line5="Talents Scholarship by Nanjing University (2023, 2022)"
        %}} {{% /honors %}}

#  - content:
#     text: |
#        {{% honors
#            line1="ACM SIGSOFT Distinguished Paper Award (ESEC/FSE'23)"
#            line2="National Scholarship for Postgraduate Students (2021)"
#            line3="China Scholarship Council (CSC) scholarships. (2023)"
#            line4="NR Scholarship Talents Scholarship by Nanjing University (2024)"
#            line5="Talents Scholarship by Nanjing University (2023, 2022)"
#        %}} {{% /honors %}}

#  - block: markdown
#    content:
#      title: 'Award and Honors'
#      subtitle: ''
#      text: |
#            ACM SIGSOFT Distinguished Paper Award (ESEC/FSE'23)
#            National Scholarship for Postgraduate Students (2021)
#            China Scholarship Council (CSC) scholarships. (2023)
#            NR Scholarship Talents Scholarship by Nanjing University (2024)
#            Talents Scholarship by Nanjing University (2023, 2022)

#        - ACM SIGSOFT Distinguished Paper Award (ESEC/FSE'23)
#        - National Scholarship for Postgraduate Students (2021)
#        - China Scholarship Council (CSC) scholarships. (2023)
#        - NR Scholarship Talents Scholarship by Nanjing University (2024)
#        - Talents Scholarship by Nanjing University (2023, 2022)

      
      
#  - block: collection
#    content:
#      title: Recent Publications
#      text: ""
#      filters:
#        folders:
#          - publication
#        exclude_featured: false
#    design:
#      view: card 
      
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
        
---


