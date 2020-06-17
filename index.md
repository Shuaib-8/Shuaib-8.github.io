---
layout: default
title: Shuaib | Aspiring data analyst. Enthusiastic about problem solving/challenges.
meta: some meta
---

# Welcome

Read the <a href="{{site.baseurl}}/about">about me</a> page.

<!--
Contact: [{{site.email}}](mailto:{{site.email}})
-->

# My Projects:

<ul >
    {% for project in site.categories.projects limit:10 %}
    <li>
        <a href="{{project.url}}" class="silent_list">{{project.title}}</a>
        <p>{{project.meta}}</p>
    </li>
    {% endfor %}
</ul>
