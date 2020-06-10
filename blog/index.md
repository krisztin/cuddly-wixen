---
layout: page
title: Think of the users
---

<div class="wrapper">
    <p>A collection of my UX related rants and ramblings. Mostly things that I encounter whilst surfing the web that annoy me enough to take a bunch of screenshots and write a few paragraphs. <strong>My biggest pet peeve: bad accessibility.</strong></p>
    <div class="flex-container just-even posts">
    {%- for post in site.posts -%} {% if post %} {% assign tags = post.tags %}{% endif %}
        {% include blog-articles.html %}
    {%- endfor -%}
    </div>
</div>
