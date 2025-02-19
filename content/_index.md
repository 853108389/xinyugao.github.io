---
sections:
  - block: markdown
    content:
      title: "📚 My Research"
      text: |
        {{% custom title="Custom Block" %}}
        This is custom content inside a shortcode.
        {{% /custom %}}
  - block: custom
    content:
      partial: "custom-block"  # # 加载 layouts/partials/custom-block.html
---