---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: HoloFab
permalink: /
---

![HoloFab](<{{ "/assets/images/GSS19-01.png" | prepend: site.baseurl | prepend: site.url }}>)

<br>

This is a base site for the set of **Augmented Reality** tools, that enable architects, designers and digital fabricators to tap into potential of the Mixed Reality Environment enhancing the creative process.

The tool consists of two parts:

- Grasshopper plug-in;
- AR application.

For the moment HoloFab supports **Microsoft Hololens** and **Android devices with [ARCore enabled](https://developers.google.com/ar/discover/supported-devices#android_play)**.

<br>

![HoloFab](<{{ "/assets/images/GSS19-00.jpg" | prepend: site.baseurl | prepend: site.url }}>)

<br>

---

## [Who](<{{ '/about' | prepend: site.baseurl | prepend: site.url }}>)

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

- Thanks to **Arman Najari** and **Ashkan Foroughi** for episodic help in development.

- Thanks to **Luis Fraguada** for insights on Grasshopper side of plugin and for suggestions on networking.

<br>

---

## Sources

For the moment the tool is in **beta** stage of development. Latest releases:

- [Github: Holofab for Grasshopper (for any version of Rhino 6)](https://github.com/HoloFab/HoloFab-Grasshopper/tree/master/_CurrentVersion)
- [Github: Holofab for Android](https://github.com/HoloFab/HoloFab-Unity/blob/master/_CurrentVersion/Android/)
- [Github: Holofab for Hololens: _coming soon_]() // Code in Repo is up-to-date - just the build is missing

<!-- For installation instructions go [here](<>). -->

This is an **opensource** project. You can find sources here:

- [Github: Holofab for Grasshopper](https://github.com/HoloFab/HoloFab-Grasshopper)
- [Github: Holofab for Unity](https://github.com/HoloFab/HoloFab-Unity)

<!-- For more detailed documentation go [here](<>). -->

You can also check out latest examples and updates of the projects in our **[news feed](<{{ '/feed' | prepend: site.baseurl | prepend: site.url }}>)**. Here is the latest one:

<ul class="cleanList">
    {% assign count = site.posts.length %}
    {% assign limit = 1 %}
    {% assign start = count-limit %}
    {% for post in site.posts limit:limit offset:start %}
        <li>
            <a href="{{ post.url }}"><h3> {{ post.title }} </h3></a>
            {{ post.excerpt }}
            <p class="right note">{{ post.date | date_to_string }}</p>
        </li>
    {% endfor %}
</ul>

---

## Contact

If you have faced any problems or have any suggestions please consult **[Issues and plans](<{{ '/issues' | prepend: site.baseurl | prepend: site.url }}>)** to see our plans first. Feel free to let us know which features are you missing in our tool.

For any proposals, suggestions or bugs as well as positive feedback :) found feel free to [contact us](<mailto:{{ site.email }}>).
