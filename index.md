---
---

{% include images.html %}

{% include carousel_image.html %}

# Software Security and Privacy Laboratory @ Korea UNIVERSITY

Software Security and Privacy Laboratory (SSP Lab) was established in 2023. We conduct various research and projects to enhance software security and ultimately ensure the safety of the software ecosystem. In particular, we are interested in researching software vulnerability detection, open-source software security for secure supply chains, analysis of security in the software ecosystem, and studies related to security patches. The results of our research are being published in top-tier international conferences and journals.

[See on-campus interview at Korea University (KR)](https://blog.naver.com/kumpij/223251918874)

## RECRUITMENT

{% include clip.html %}

We are continuously looking for enthusiastic **Ph.D./master students** and **graduate/undergraduate interns** interested in working with us. Please contact Prof. Seunghoon Woo (<U>seunghoonwoo [at] korea.ac.kr</U>) with your CV and portfolio.

## LATEST NEWS

* **Sep. 2024**: Two **new MS students** are joining our team. Welcome Youngjae and Seogyeong!
* **Jul. 2024**: Prof. Woo won the **Excellent Teaching Award (우수강좌상)** for the Theory of Computation class in Fall 2023!
* **Mar. 2024**: Our paper **BLOOMFUZZ** has been accepted at **[ESORICS 2024](https://esorics2024.org/)**. Congrats to Pyeongju!
* **Mar. 2024**: One **new Ph.D. student** is joining our team. Welcome Heedong!
* **Dec. 2023**: Our paper **[CNEPS](/assets/papers/ICSE24.pdf)** has been accepted at **[ICSE 2024](https://conf.researchr.org/home/icse-2024)**. Congrats to Yoonjong!
* **Aug. 2023**: Our paper **[V1SCAN](/assets/papers/SECURITY23.pdf)** has been published at **[USENIX Security 2023](https://www.usenix.org/conference/usenixsecurity23)**.
* <U>SSP lab</U> has been established.

## ADVISOR

{%
  include my_feature_idx.html
  image="images/profile.jpg"
  text="**Seunghoon Woo (우승훈)**<br>(seunghoonwoo [at] korea.ac.kr)<br>Assistant professor<br>[Dept. of Computer Science and Engineering](https://cs.korea.ac.kr/)<br>[College of Informatics](https://info.korea.ac.kr/), [Korea University](https://www.korea.ac.kr/)<br>[[CV]](/assets/CV(20240401).pdf) (Last updated: Apr. 2024)"
  flip=false
%}

## RESEARCH AREAS (NOT LIMITED TO)

* **Open-source Software Security**
* **Supply Chain Security**
* **Vulnerability Detection**
* **Software Composition Analysis (SCA)**
* **Software Bills of Materials (SBoM) Management**
* **Security Patch Analysis**

[See more](/research)

## EDUCATIONAL BACKGROUND

* 2016.09 - 2022.08, **Ph.D and M.S.**, Dept. of Computer Science and Engineering, Korea University (Advisor: Prof. Heejo Lee)
* 2010.03 - 2016.02, **B.S.**, Dept. of Computer Science and Engineering, Korea University

## WORKING EXPERIENCES

* 2023.09 - Present, **Assistant Professor**, Dept. of Computer Science and Engineering, Korea University
* 2022.05 - Present, **Chief Scientist**, LABRADOR LABS Inc.
* 2022.09 - 2023.08, **Research Professor**, Center for Software Security and Assurance (CSSA), Korea University
* 2016.12 - 2017.03, **Visiting Researcher**, National University of Singapore (Advisor: Prof. Min Suk Kang)
* 2015.12 - 2016.02, **Employee**, Samsung Electronics.
* 2014.06 - 2014.08, **Internship**, Samsung Electronics.

## REVIEWER

* TDSC: IEEE Transactions on Dependable and Secure Computing (2024)
* TSE: IEEE Transactions on Software Engineering (2023)
* TOSEM: ACM Transactions on Software Engineering and Methodology (2023)
* SP&E: Software Practice and Experience (2023)
* IEEE Transactions on Vehicular Technology (2022)
* Journal of Communications and Networks (2021)

## CONTACT

<i class="fa-solid fa-home"></i> 206B, Woojung Hall of Informatics<br>
College of Informatics<br>
Korea University<br>
Anam-dong 5-ga, Seongbuk-gu<br>
Seoul, Korea<br>
<i class="fa-solid fa-phone"></i> +82-2-3290-3192<br>
<i class="fa-solid fa-envelope"></i> seunghoonwoo [at] korea.ac.kr

{% for link in site.links %}
    {% assign key = link[0] %}
    {% assign value = link[1] %}
    {% include button.html type=key text="" link=value style="bare" %}
{% endfor %}
