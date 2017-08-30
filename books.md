---
layout: default
is_contact: false
title: Book List | Samuel Green
---

## Reading List

#### 2017 
<ul>
    {% for book in site.data.books %}
    <li>
    <a class='inline' href="{{ book.amazon }}">{{ book.title }}
    </a>
    {% if book.subtitle %}: {{book.subtitle}}.{% else %}.{%endif%}
        {{book.author}}</li>
    {% endfor %}
</ul>