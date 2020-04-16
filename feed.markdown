---
layout: default
title: Feed
permalink: /feed
---

This is a collection of some projects and articles related to the HoloFab tool.

<ul class="cleanList">
    {% assign count = site.posts.length %}
    {% assign limit = 10 %}
    {% assign start = count-limit %}
    {% for post in site.posts limit:limit offset:start %}
        <li>
            <a href="{{ post.url }}"><h3> {{ post.title }} </h3></a>
            {{ post.excerpt }}
            <p class="right note">{{ post.date | date_to_string }}</p>
        </li>
    {% endfor %}
</ul>
