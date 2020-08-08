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

<br>

#### _Acknowledgements:_

- Special thanks to **[Institute for Advanced Architecture of Catalonia](https://iaac.net/)** for support in early stages of development, for providing Hololens for testing and for collaborating in applying the plugin in various in-house projects.

<div class="smallIconHolder">
<a href="https://iaac.net/"><img src="https://fablabbcn.org/img/logos/logo_partners_iaac.png"></a>
</div>

<br>

- Thanks to **Arman Najari**, **Ashkan Foroughi** for episodic help in development.

- Thanks to **Luis Fraguada** for insights on Grasshopper side of plugin and for suggestions on networking.

<br>
