---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: HoloFab
permalink: /
---

![HoloFab](./assets/images/GSS19-01.jpg)

<br>

This is a base site for the set of **Augmented Reality** tools, that enable architects, designers and digital fabricators to tap into potential of the Mixed Reality Environment enhancing the creative process.

The tool consists of two parts:

-   Grasshopper plug-in;
-   AR application.

For the moment HoloFab supports **Microsoft Hololens** and **Android devices with [ARCore enabled](https://developers.google.com/ar/discover/supported-devices#android_play)**.

<br>

![HoloFab](./assets/images/GSS19-00.jpg)

<br>

<hr>

## [Who](./about)

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

<hr>

## Sources

For the moment the tool is in **beta** stage of development. Latest releases:

-   [Github: Holofab for Grasshopper](https://github.com/HoloFab/HoloFab-Grasshopper/tree/master/_CurrentVersion)
-   [Github: Holofab for Android](https://github.com/HoloFab/HoloFab-Unity/blob/master/_CurrentVersion/Android/)
-   [Github: Holofab for Hololens: _coming soon_](<>)

<!-- For installation instructions go [here](<>). -->

This is an opensource project. You can find sources here:

-   [Github: Holofab for Grasshopper](https://github.com/HoloFab/HoloFab-Grasshopper)
-   [Github: Holofab for Unity](https://github.com/HoloFab/HoloFab-Unity)

<!-- For more detailed documentation go [here](<>). -->

<!-- For examples go [here](<>). -->

<hr>

## Contact

For any proposals, suggestions or bugs found feel free to [contact us](<mailto:{{ site.email }}>).
