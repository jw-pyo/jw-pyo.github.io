---
layout: page
title: Profile
permalink: /profile/
---

## Education

* 2017.03 - 2020.02 , M.S, Electrical & Computer Engineering in Seoul National University(In-memory Database Lab)
* 2013.03 - 2017.02 , B.S, Electrical & Computer Engineering in Seoul National University

## Career & Internship

* 2018.03 - 2019    , 서울대학교 블록체인 학회 Decipher 1, 2기
* 2016.07 - 2016.08 , LG전자 CTO부문 SW센터 PMO실 SDK part intern 

## Projects

* 2020.02.07 - 02.12, AAAI 2020 학회 발표

* 2019, Multi-Domain Networks for Object Detection in Road Environment
    <p align="center">
      <img src="/files/profile/example_mdnet.png" alt="mdnet" width="450"/>
    </p>
    - Yolo-v3을 backbone network로 사용하여 도로의 여러 차량을 인식하는 muldi-domain object detection model 구축
    - network를 shared weight를 공유하는 multi-branch로 나누고, 각 branch를 road condition(weather, time) 별로 구분하여 train
    - [BDD100k](https://bair.berkeley.edu/blog/2018/05/30/bdd/) dataset 활용
    - baseline(single-branch network)에 비해 mAP 향상
    - data preprocessing: python, core: python(Pytorch)
    - demo link: [https://youtu.be/CZ_VfzbysHA](https://youtu.be/CZ_VfzbysHA)
    <p align="center">
      <img src="/files/profile/mAP_mdnet.png" alt="mAP comparison between multi-domain network and single-domain network" width="450"/>
    </p>
    <p align="center">
      <em> ▲ mAP comparison between multi-domain network and single-domain network</em>
    </p>

* 2018.08.24 - 08.25, Queryable blockchain-중국 상하이 Zhongan Insurance 해커톤 준우승(2nd prize)[(포스트)](/_posts/2018-08-26/2018-08-26-zhongan_hackathon.markdown)
    - demo link: [https://youtu.be/EzoG1hWP9eA](https://youtu.be/EzoG1hWP9eA)
    - core(blockchain): C++11, network & client: Python, JavaScript

* 2017, smartcard 데이터를 이용한 출.퇴근 시간 crowd path visualization(with Tableau)
    - 2016.06.17(Sat) 하루 동안의 수도권 교통카드 tagging data 활용(about 10 million rows)
    - subway, bus를 이용한 승객들의 이동 방향 및 수를 시각화
    - 시간, tagging count를 filtering하여 확인 가능
    - data processing: Python, visualization: Tableau
    - [subway demo](https://public.tableau.com/profile/.3518#!/vizhome/bus_v0_2/1?publish=yes)
    - [bus demo](https://public.tableau.com/profile/.3518#!/vizhome/bus_v0_2_onlybus/1?publish=yes)    
    <p align="center">
      <img src="/files/profile/smartcard_subway.png" alt="example of visualization for smartcard:subway" width="450"/>
    </p>
    <p align="center">
      <em> ▲ example of crowd's subway trajactory visualization based on smartcard data </em>
    </p>

## Skills & Experiences

* C, C++
* Python(Tensorflow, Pytorch)
* Solidity
* Apache Spark
* (RDBMS)PostgreSQL, MySQL
* (NoSQL)MongoDB
* (Blockchain)Ethereum, Quorum
* Tableau

## Publications

* Jungwoo Pyo, Joohyun Lee, Youngjune Park, Tien-Cuong Bui, Sang Kyun Cha, [*An Attention-Based Speaker Naming Method for Online Adaptation in Non-Fixed Scenarios*](http://arxiv.org/abs/1912.00649), AAAI Workshop on Interactive and Conversational Recommendation Systems(WICRS), Feb 2020, New York, USA.
* [영지식 증명(zero-knowledge proof)에 관한 글](https://medium.com/decipher-media/zero-knowledge-proof-chapter-1-introduction-to-zero-knowledge-proof-zk-snarks-6475f5e9b17b) 

## Presentation


## Interested in..


This is the base Jekyll theme. You can find out more info about customizing your Jekyll theme, as well as basic Jekyll usage documentation at [jekyllrb.com](https://jekyllrb.com/)

You can find the source code for Minima at GitHub:
[jekyll][jekyll-organization] /
[minima](https://github.com/jekyll/minima)

You can find the source code for Jekyll at GitHub:
[jekyll][jekyll-organization] /
[jekyll](https://github.com/jekyll/jekyll)


[jekyll-organization]: https://github.com/jekyll
