---
---

{% include images.html %}

![plain image](/images/main.jpg)

# Software Security and Privacy Laboratory @ Korea UNIVERSITY

Software Security and Privacy Laboratory (SSP Lab) was established in 2023. We conduct various research and projects to enhance software security and ultimately ensure the safety of the software ecosystem. In particular, we are interested in researching software vulnerability detection, open-source software security for secure supply chains, analysis of security in the software ecosystem, and studies related to security patches. The results of our research are being published in top-tier international conferences and journals.

[See on-campus interview at Korea University (KR)](https://blog.naver.com/kumpij/223251918874)

## RECRUITMENT

We are continuously looking for enthusiastic **Ph.D./master students**, **graduate/undergraduate interns**, and **postdocs** interested in working with us. Please contact Prof. Seunghoon Woo (<U>seunghoonwoo [at] korea.ac.kr</U>).

## LATEST NEWS

* **Dec. 2023**: **CNEPS** has been accepted at **[ICSE 2024](https://conf.researchr.org/home/icse-2024)**.
* **Aug. 2023**: **[V1SCAN](/assets/papers/SECURITY23.pdf)** has been published at **[USENIX Security 2023](https://www.usenix.org/conference/usenixsecurity23)**.
* <U>SSP lab</U> has been established.

## ADVISOR

{%
  include my_feature_idx.html
  image="images/profile.jpg"
  text="**Seunghoon Woo (우승훈)**<br>(seunghoonwoo [at] korea.ac.kr)<br>Assistant professor<br>[Dept. of Computer Science and Engineering](https://cs.korea.ac.kr/)<br>[College of Informatics](https://info.korea.ac.kr/), [Korea University](https://www.korea.ac.kr/)<br>[[CV]](/assets/CV.pdf)"
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
* 2007.03 - 2010.02, Changwon Yongho High School

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

[Room] 206B, Woojung Hall of Informatics<br>
College of Informatics<br>
Korea University<br>
Anam-dong 5-ga, Seongbuk-gu<br>
Seoul, Korea<br>
[Office] +82.2.3290.3192<br>
[Email] seunghoonwoo [at] korea.ac.kr

{% for link in site.links %}
    {% assign key = link[0] %}
    {% assign value = link[1] %}
    {% include button.html type=key text="" link=value style="bare" %}
{% endfor %}
