---
---

{% include images.html %}

![plain image](/ssp/images/main.jpg)

# Software Security and Privacy Laboratory @ Korea UNIVERSITY

Software Security and Privacy Laboratory (SSP Lab) was established in 2023. We conduct various research and projects to enhance software security and ultimately ensure the safety of the software ecosystem. In particular, we are interested in researching software vulnerability detection, open-source software security for secure supply chains, analysis of security in the software ecosystem, and studies related to security patches. The results of our research are being published in top-tier international conferences and journals.

## RECRUITMENT

We are continuously looking for enthusiastic **PhD/master students**, **graduate/undergraduate interns**, and **postdocs** interested in working with us. Please contact Prof. Seunghoon Woo (<U>seunghoonwoo@korea.ac.kr</U>).

## RESEARCH AREAS (NOT LIMITED TO)

* **Open-source Software Security**
* **Supply Chain Security**
* **Vulnerability Detection**
* **Software Composition Analysis (SCA)**
* **Security Patch Analysis**

[See more](/ssp/research)


## LATEST NEWS


* **Aug. 2023**: **[V1SCAN](/ssp/assets/papers/SECURITY23.pdf)** has been published at **[USENIX Security 2023](https://www.usenix.org/conference/usenixsecurity23)**.
* <U>SSP lab</U> has been established.


## CONTACT

Room XXX, XXX<br>
College of Informatics<br>
Korea University<br>
Anam-dong 5-ga, Seongbuk-gu<br>
Seoul, Korea<br>
[Office] +82.2.3290.XXXX<br>
[Email] seunghoonwoo@korea.ac.kr

{% for link in site.links %}
    {% assign key = link[0] %}
    {% assign value = link[1] %}
    {% include button.html type=key text="" link=value style="bare" %}
{% endfor %}
