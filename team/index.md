---
title: Members
nav:
  order: 1
  tooltip: Lab members
---

# {% include icon.html icon="fa-solid fa-users" %}Members

{%
  include my_feature.html
  image="images/me.jpg"
  text="Seunghoon Woo (우승훈)<br>(seunghoonwoo@korea.ac.kr)<br>Assistant professor<br>[Dept. of Computer Science and Engineering](https://cs.korea.ac.kr/)<br>[College of Informatics](https://info.korea.ac.kr/), [Korea University](https://www.korea.ac.kr/)"
  flip=false
%}


{% include section.html %}

{% include list.html data="members" component="portrait" filters="role: pi" %}
{% include list.html data="members" component="portrait" filters="role: ^(?!pi$)" %}

{% include section.html background="images/background.jpg" dark=true %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

{% include section.html %}

{% capture content %}

{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}

{% endcapture %}

{% include grid.html style="square" content=content %}
