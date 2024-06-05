---
pcx_content_type: example
summary: Respect Strong ETags
title: Respect Strong ETags
layout: wide
---

# Respect Strong ETags

[Create a cache rule](/cache/how-to/cache-rules/create-dashboard/) to respect strong ETags for any hostname containing `example.com`:

<div class="DocsMarkdown--example">

- **When incoming requests match**: Custom filter expression
    - Using the Expression Builder:<br>
        `Hostname contains "example.com"`
    - Using the Expression Editor:<br>
        `(http.host contains "example.com")`

- **Then**:
    - **Cache eligibility**: Eligible for cache
    - **Setting**: Respect strong ETags
        - **Use strong ETag headers**: On

</div>