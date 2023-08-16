---
title: Research
nav:
  order: 2
  tooltip: Research Topics
---

# {% include icon.html icon="fa-solid fa-microscope" %}Research

We conduct various research on software security. Representative current research topics are as follows.

{% include section.html %}

## Open-source Software Security & Vulnerability Detection

{%
  include my_feature.html
  image="images/oss.jpg"
  text="The reuse of open-source software (OSS) provides efficiency for developers. However, unmanaged OSS reuse may lead to the propagation of vulnerabilities. We have conducted research to devise scalable and precise vulnerability detection techniques aimed at resolving security threats caused by vulnerable OSS reuse. Our techniques can actually be used to resolve vulnerabilities in real-world popular software programs (e.g., Android, Redis, Mozjpeg, etc.). In addition, our research papers have been published in international conferences, including V1SCAN [USENIX Security '23], MOVERY [USENIX Security '22], and VUDDY [S&P '17]."
  flip=false
%}

{% include section.html %}

## Software Composition Analysis (SCA)

{%
  include my_feature.html
  image="images/sca.jpg"
  text="Identifying what and how OSS projects are reused in the software program is the very first step towards ensuring software security. Our research can precisely identify third-party OSS components from the target software codebase, especially in C/C++ languages where identifying OSS components is challenging. The results of the research have been published in international conferences, including CENTRIS [ICSE '21]."
  flip=true
%}

## Security Patch Analysis

{%
  include my_feature.html
  image="images/patch.jpg"
  text="Assessing the quality of security patches provided through public vulnerability databases (e.g., NVD) is an essential task for proper vulnerability resolution. We have conducted research ranging from effective methods of collecting security patches to techniques for verifying their quality. The results of our research have been presented in international conferences and journals as papers, including V0Finder [USENIX Security '21] and xVDB [IEEE ACCESS '22]."
  flip=false
%}
