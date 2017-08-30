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
    {% if book.subtitle %}
    <a class='inline' href="{{ book.amazon }}">
    {{ book.title }}</a>: {{book.subtitle}}.
    {% else %}
    <a class='inline' href="{{ book.amazon }}">
    {{ book.title }}</a>.
    {% endif %}
    <br>– {{book.author}}
    </li>
    {% endfor %}
</ul>