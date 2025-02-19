---
sections:
  - block: markdown  # 用shortcode
    content:
      title: "📚 My Research"
      text: |
        {{% custom title="Custom Block" %}}
        This is custom content inside a shortcode.  This is custom content inside a shortcode.  This is custom content inside a shortcode.  This is custom content inside a shortcode.  This is custom content inside a shortcode.  This is custom content inside a shortcode.  This is custom content inside a shortcode.
        {{% /custom %}}
  - block: markdown # 用小部件
    content:
      title: "📚 My Research"
      text: | 
        {{ partial "custom-block.html" . }} {{ partial "custom-block.html" . }} {{ partial "custom-block.html" . }} {{ partial "custom-block.html" . }} {{ partial "custom-block.html" . }} {{ partial "custom-block.html" . }} {{ partial "custom-block.html" . }} 
  - widget: custom-block  # 用block 这里用 widget，而不是 block
    content:
      title: "Custom Block"
      text: "This is a custom block."
---
