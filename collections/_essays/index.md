---
layout: default
title: index
---

{% assign essays = site.essays | where_exp: "item", "item.title != 'index'" %}
<ul>
    {%- for essay in essays -%}
        <li> <a href="{{essay.permalink}}">{{ essay.date | date: "%B %d, %Y" }} - {{ essay.title }}</a> </li>
    {%- endfor -%}    
</ul>