---
layout: default
title: Home | Samuel Green
---

## About

<img class="profile-picture" src="headshot_new.jpg">

I graduated in 2017 from Harvard 
College, where I concentrated in
Computer Science and did a 
secondary in Government. I wrote a [thesis](/thesis.pdf)
on [multi-agent markets](https://en.wikipedia.org/wiki/Two-sided_market) for indivisible goods with
[Prof. David Parkes](http://www.eecs.harvard.edu/~parkes/).
I helped
[Prof. Stuart Shieber](http://eecs.harvard.edu/shieber/) lead [Computer Science 51: Abstraction and 
Design in Computation](http://cs51.io) along with [Gabbi Merz](http://gcmerz.github.io). 

#### Projects
<ul>
{% for proj in site.data.projects %}
    <li> <a href="{{proj.link}}">{{proj.name }}</a> </li>
{% endfor %}
</ul>

#### Archive
<ul>
{% for arc in site.data.archive %}
    <li> <a href="{{arc.link}}">{{arc.name }}</a> </li>
{% endfor %}
</ul>

