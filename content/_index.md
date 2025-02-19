---
title: "About"
layout: "default"  # 使用默认布局，或者指定其他布局

sections:
  - block: resume-biography222
    content:
      # Choose a user profile to display (a folder name within `content/authors/`) #
      username: admin2
      text: ""
      # Show a call-to-action button under your biography? (optional)
#      button:
#        text: Download CV
#        url: uploads/resume.pdf
---
{{ partial "custom-block.html" . }}
{{ partial "resume-biography222.html" . }}
