---
layout: default
title: Colophon
permalink: /about/this-site/
description: Info about this site
hidden: true
wide: true
---


May be out of date due to Cloudflare caching.

- Jekyll Version **{{ jekyll.version }}**
- Jekyll Environment **{{ jekyll.environment }}** 
- Built Started at **{{ site.time | date: '%Y-%m-%d %H:%M' }}**
- **{{ site.pages.size }}** Pages
- **{{ site.posts.size }}** Posts (**{{ site.categories.size }}** cats, **{{ site.tags.size }}** tags)
- **{{ site.documents.size }}** Pages in Collections
- **{{ site.static_files.size }}** Static Files

---

## Jekyll Variable
<pre style="max-height: 95vh; overflow: scroll; background-color: #000; color: #fff;">
{{ jekyll | jsonify | escape }}
</pre>

---

## Site Variable
<pre style="max-height: 95vh; overflow: scroll; background-color: #000; color: #fff;">
{% if jekyll.environment != "production" %}
{{ site | inspect }}
{% else %}
~ Hidden on production site ~
{% endif %}
</pre>

