---
layout: default
title: index
---

<ul>
    {%- for post in site.posts -%}
        <li> <a href="{{post.permalink}}">{{ post.date | date: "%B %d, %Y" }} - {{ post.title }}</a> </li>
    {%- endfor -%}    
</ul>

