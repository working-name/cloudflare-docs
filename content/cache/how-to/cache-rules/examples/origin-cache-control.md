---
pcx_content_type: example
summary: Origin Cache Control
title: Origin Cache Control
layout: wide
---

# Origin Cache Control

[Create a cache rule](/cache/how-to/cache-rules/create-dashboard/) to determine edge cache behavior for any hostname containing `example.com`:

<div class="DocsMarkdown--example">

- **When incoming requests match**: Custom filter expression
    - Using the Expression Builder:<br>
        `Hostname contains "example.com"`
    - Using the Expression Editor:<br>
        `(http.host contains "example.com")`

- **Then**:
    - **Cache eligibility**: Eligible for cache
    - **Setting**: Origin Cache Control
        - **Enable Origin Cache Control**: Off

</div>