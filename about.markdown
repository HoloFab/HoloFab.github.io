---
layout: default
title: About
permalink: /about
---

We are an international team of architects passionate about integrating **Technology in Architecture**. All three of us passed through Institute of Advanced Architecture of Catalonia where the seeds of the project began.

<ul class="team horisontalList">
{% for person in site.data.team %}

    <li class = "teamMember horisontalListItem">
        <img src="{{ person.image }}">
        <h3>{{ person.name }}</h3>
        <p>{{ person.shortDescription }}</p>
        <a href="{{ person.link }}">contact</a>
    </li>

{% endfor %}

</ul>
