---
layout: page
title: Profile
permalink: /profile/
---

## Info
<div class="row" style="display:flex">
  <div class="left_column" style="flex:40%">
    <img src="/files/profile/portrait.jpg" alt="portrait" width="250" />
  </div>
  <div class="right_column" style="flex:60%">
    <p style="font-size:20px">표정우(Jungwoo Pyo)</p>
    <p style="font-size:15px">
      1994.05.12<br />
      Github: <a href="https://github.com/jw-pyo">https://github.com/jw-pyo</a><br />
      Homepage: <a href="https://jw-pyo.github.io">https://jw-pyo.github.io</a><br /><br />
      Live As Greedy: local optimal을 선택하다 보면 결국 global optimal에 도달하는 greedy algorithm의 풀이 방식처럼, 현재의 위치에서 최선을 다하면 결국 원하는 목표에 도달할 수 있다는 motto를 가지며 새로운 것에 대한 배움을 즐기는 엔지니어입니다.</p>
  </div>
</div>

## Education

* 2017.03 - 2020.02 , M.S, Electrical & Computer Engineering in Seoul National University(In-memory Database Lab)
* 2013.03 - 2017.02 , B.S, Electrical & Computer Engineering in Seoul National University

## Career & Internship

* 2018.03 - 2019    , 서울대학교 블록체인 학회 Decipher 1, 2기
* 2016.07 - 2016.08 , LG전자 CTO부문 SW센터 PMO실 SDK part intern 

## Projects

* **2019, An Attention-Based Speaker Naming Method for Online Adaptation in Non-Fixed Scenarios(will be presented at *AAAI 2020 Workshop(WICRS)*)**

<p align="center" padding="5px 0 5px 0">
  <img src="/files/profile/speaker_naming.png" alt="speaker naming" width="450" height="200"/>
</p>
<p align="center" padding="0 0 5px 0">
  <img src="/files/profile/speaker_naming_architecture.png" alt="speaker naming architecture" width="450" height="200"/>
</p>
<p align="center">
  <em> ▲ Overall architecture of attention-based speaker naming method</em>
</p>

<ul><ul>
  <li>영화나 드라마에서 화자의 얼굴을 localize하고, face-voice feature embedding을 활용하여 화자의 ID를 식별하는 speaker naming task 수행</li>
  <li>speaker naming task를 수행하는 기존의 gradient-based method 방식과 달리, attention module을 이용하여 gradient update process 없이 prior knowledge와 target data 간의 similarity의 linear combination을 통한 target data의 identification을 수행하는 방법 제시</li>
  <li>기존의 방식은 모델을 훈련시키기 위해 충분한 training data와 긴 training time이 소요되는 단점이 있었으나, 본 논문에서 제시한 방법을 통해 비슷한 수준의 accuracy를 유지하면서 model training time을 크게 단축시킴(10x-100x).</li>
  <li>gradient-based method에서 사용된 것보다 적은 수의 training data(5 face-voice pairs per ID)만을 이용하여 모델 구축 가능</li>
  <li>모델이 배포된 이후에 추가적으로 얻게 되는 새로운 데이터를 attention module에 추가하여 knowledge base로 활용하는 online adaptation 가능</li>
</ul></ul>

* **2019, Multi-Domain Networks for Object Detection in Road Environment**

<p align="center" padding="5px 0 5px 0">
  <img src="/files/profile/example_mdnet.png" alt="mdnet" width="450" height="200"/>
</p>

<ul><ul>
  <li>Yolo-v3을 backbone network로 사용하여 도로의 여러 차량을 인식하는 multi-domain object detection model 구축</li>
  <li>shared weight를 공유하는 multi-branch network로 구성하고, 각 branch를 road condition(weather, time)에 dependent하게 훈련</li>
  <li><a href="https://bair.berkeley.edu/blog/2018/05/30/bdd/">BDD100k</a> dataset 활용</li>
  <li>baseline(single-branch network)에 비해 mAP 향상</li>
  <li>data preprocessing: python, core: python(Pytorch)</li>
  <li>demo link:<a href="https://youtu.be/CZ_VfzbysHA"> https://youtu.be/CZ_VfzbysHA </a></li>
  <p align="center" padding="5px 0 5px 0">
    <img src="/files/profile/mAP_mdnet.png" alt="mAP comparison between multi-domain network and single-domain network" width="450"/>
  </p>
  <p align="center">
    <em> ▲ mAP comparison between multi-domain network and single-domain network</em>
  </p>

</ul></ul>

* **2018.08.24 - 08.25, Queryable blockchain-중국 상하이 Zhongan Insurance 해커톤 준우승(2nd prize)**[(포스트)](/_posts/2018-08-26/2018-08-26-zhongan_hackathon.markdown)

<ul><ul>
  <li>demo link: <a href="https://youtu.be/EzoG1hWP9eA"> https://youtu.be/EzoG1hWP9eA </a></li>
  <li>core(blockchain): C++11, network & client: Python, JavaScript</li>
</ul></ul>

* **2017, smartcard 데이터를 이용한 출.퇴근 시간 crowd path visualization**

<ul><ul>
  <li>2016.06.17(Sat) 하루 동안의 수도권 교통카드 tagging data 활용(about 10 million rows)</li>
  <li>지하철, 버스를 이용한 승객들의 이동 방향 및 수를 시각화</li>
  <li>시간, tagging count를 필터링하여 확인 가능</li>
  <li>data processing: Python, visualization: Tableau</li>
  <li><a href="https://public.tableau.com/profile/.3518#!/vizhome/bus_v0_2/1?publish=yes">[subway demo]</a></li>
  <li><a href="https://public.tableau.com/profile/.3518#!/vizhome/bus_v0_2_onlybus/1?publish=yes">[bus demo]</a></li>
  <p align="center" padding="5px 0 5px 0">
    <img src="/files/profile/smartcard_subway.png" alt="example of visualization for smartcard:subway" width="450"/>
  </p>
  <p align="center">
    <em> ▲ example of crowd's subway trajactory visualization based on smartcard data </em>
  </p>
</ul></ul>

## Skills & Experiences

<ul>
  <li>Python(Tensorflow, Pytorch)</li>
  <li>C, C++</li>
  <li>(Blockchain)Ethereum, Quorum</li>
  <li>Solidity</li>
  <li>Apache Spark</li>
  <li>(RDBMS)PostgreSQL, MySQL</li>
  <li>(NoSQL)MongoDB</li>
  <li>Tableau</li>
</ul>

## Publications

<ul>
  <li>Jungwoo Pyo, Joohyun Lee, Youngjune Park, Tien-Cuong Bui, Sang Kyun Cha, <a href="http://arxiv.org/abs/1912.00649"><b>An Attention-Based Speaker Naming Method for Online Adaptation in Non-Fixed Scenarios</b></a>, AAAI 2020 Workshop on Interactive and Conversational Recommendation Systems(WICRS), Feb 2020, New York, USA.</li>
  <li><a href="https://medium.com/decipher-media/zero-knowledge-proof-chapter-1-introduction-to-zero-knowledge-proof-zk-snarks-6475f5e9b17b">영지식 증명(zero-knowledge proof)에 관한 글</a></li>

