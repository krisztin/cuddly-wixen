---
layout: page
title: Think of the users
---

<div class="wrapper">
{%- for post in site.posts -%}
{% if post %} {% assign tags = post.tags %}{% endif %}
    <article class="blog-listing">
        <h3><a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></h3>
        <p>
        <span class="post-tags"><img src="{{ site.url }}/assets/img/tag.svg" title="tags" alt="" aria-hidden="true"> | 
        {% for tag in tags %}
        <a href="{{site.baseurl}}/tags/#{{tag|slugize}}" class="post-tag">{{tag}}</a>
            {% unless forloop.last %}&nbsp;{% endunless %}
        {% endfor %}
        </span>
        </p>
        <p>{{ post.excerpt }}</p>
    </article>
{% endfor %}
</div>
