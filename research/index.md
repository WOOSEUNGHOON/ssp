---
title: Research
nav:
  order: 2
  tooltip: Research Topics
---

# {% include icon.html icon="fa-solid fa-microscope" %}Research

We conduct various research on software security. Representative current research topics are as follows.

{% include section.html %}

## Open-source Software Security & Supply Chain Security & Vulnerability Detection

{%
  include my_feature.html
  image="images/oss.jpg"
  text="The reuse of open-source software (OSS) provides efficiency for developers. However, unmanaged OSS reuse may lead to the propagation of vulnerabilities. We have conducted research to devise scalable and precise vulnerability detection techniques aimed at resolving security threats caused by vulnerable OSS reuse. Our techniques can actually be used to resolve vulnerabilities in real-world popular software programs (e.g., Android, Redis, Mozjpeg, etc.). In addition, our research papers have been published in international conferences, including TIVER [ICSE '25](/assets/papers/ICSE25.pdf), [V1SCAN](/assets/papers/SECURITY23.pdf) [USENIX Security '23], [MOVERY](/assets/papers/SECURITY22.pdf) [USENIX Security '22], and [VUDDY](/assets/papers/SNP17.pdf) [S&P '17]."
  flip=false
%}

- ["소프트웨어 보안취약점, 기존 기술 대비 최대 6배 이상 탐지 가능" (KR)](https://www.korea.ac.kr/user/boardList.do?boardId=474633&command=albumView&page=1&boardSeq=493539&id=university_060108000000)
- ["이희조 고려대 교수팀 , 취약 코드 탐지 MOVERY 기술 개발" (KR)](https://n.news.naver.com/mnews/article/030/0003046842?sid=105)
- ["고려대, '재사용 코드'' 자동 탐지 기술 개발" (KR)](http://www.veritas-a.com/news/articleView.html?idxno=83064)
- ["이희조·우승훈 고려대 컴퓨터학과 교수 연구팀, 오픈소스 소프트웨어 취약점 탐지 기술 V1SCAN 개발" (KR)](https://www.dailysmart.co.kr/news/articleView.html?idxno=77884)


{% include section.html %}

## Software Composition Analysis (SCA)

{%
  include my_feature.html
  image="images/sca.jpg"
  text="Identifying what and how OSS projects are reused in the software program is the very first step towards ensuring software security. Our research can precisely identify third-party OSS components from the target software codebase, especially in C/C++ languages where identifying OSS components is challenging. The results of the research have been published in international conferences, including [CENTRIS](/assets/papers/ICSE21.pdf) [ICSE '21] and [CNEPS](/assets/papers/ICSE24.pdf) [ICSE '24]."
  flip=true
%}

- ["CENTRIS: New tool helps prevent software supply chain attacks by flagging modified open source components" (EN)](https://portswigger.net/daily-swig/centris-new-tool-helps-prevent-software-supply-chain-attacks-by-flagging-modified-open-source-components)
- ["오픈소스 커뮤니티 노리는 공급망 공격, 국내 연구팀 기술로 차단한다" (KR)](https://www.boannews.com/media/view.asp?idx=95883)
- ["고려대 이희조-우승훈 교수팀, 직접 개발한 CNEPS로 공급망 보안 강화" (KR)](https://www.boannews.com/media/view.asp?idx=129096&page=1&kind=5)




{% include section.html %}

## Security Patch Analysis

{%
  include my_feature.html
  image="images/patch.jpg"
  text="Assessing the quality of security patches provided through public vulnerability databases (e.g., NVD) is an essential task for proper vulnerability resolution. We have conducted research ranging from effective methods of collecting security patches to techniques for verifying their quality. The results of our research have been presented in international conferences and journals as papers, including [V0Finder](/assets/papers/SECURITY21.pdf) [USENIX Security '21] and [xVDB](/assets/papers/ACCESS22_xvdb.pdf) [IEEE ACCESS '22]."
  flip=false
%}

- ["고려대 이희조 교수팀, 취약점 최초 발생 지점 탐지기술 'V0Finder' 개발" (KR)](https://www.boannews.com/media/view.asp?idx=100545)
