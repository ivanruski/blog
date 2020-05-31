---
layout: "essays"
title: index
---

{% assign essays = site.essays | where_exp: "item", "item.title != 'index'" %}
<dl>
    {%- for essay in essays -%}
        <dt> - <a href="{{essay.permalink}}" >{{ essay.title }}</a> </dt>
    {%- endfor -%}    
</dl>