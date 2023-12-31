---
---

# Software Security and Privacy Laboratory

Software Security and Privacy Laboratory (SSP Lab) was established in 2023. We conduct various research and projects to enhance software security and ultimately ensure the safety of the software ecosystem. In particular, we are interested in researching software vulnerability detection, open-source software security for secure supply chains, analysis of security in the software ecosystem, and studies related to security patches. The results of our research are being published in top -tier international conferences and journals.

## NEWS

We are continuously looking for enthusiastic graduate/undergraduate students and postdocs interested in working with us.

## RESEARCH AREAS (NOT LIMITED TO)

* **Open-source Software Security**
* **Vulnerability Detection**
* **Software Composition Analysis (SCA)**
* **Security Assessment for Software Ecosystems**
* **Security Patch Analysis**


{% for link in site.links %}
    {% assign key = link[0] %}
    {% assign value = link[1] %}
    {% include button.html type=key text="" link=value style="bare" %}
{% endfor %}

<!-- {% include section.html %}

## Highlights

{% capture text %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

{%
  include button.html
  link="research"
  text="See our publications"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="research"
  title="Our Research"
  text=text
%}

{% capture text %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

{%
  include button.html
  link="projects"
  text="Browse our projects"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="projects"
  title="Our Projects"
  flip=true
  style="bare"
  text=text
%}

{% capture text %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

{%
  include button.html
  link="team"
  text="Meet our team"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="team"
  title="Our Team"
  text=text
%}
 -->


  &nbsp; | &nbsp; Built with
    <a href="https://github.com/greenelab/lab-website-template">
      Lab Website Template
    </a>