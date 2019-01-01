---
layout: post
title:  "상하이 Zhongan Insurance Hackathon 참가 후기"
date:   2018-08-26 18:00:00 +0900
categories: blockchain, databases
---

2018년 8월 25일 - 26일, 양일간 상하이의 Zhongan Insurance에서 주최하는 blockchain track 해커톤에 참여하였다. 현재 블록체인 기술의 발전에 비해 많은 자본이 유입되었기 때문에, 많은 사람들이 블록체인의 성공 가능성과 실생활에서의 적용 가능성에 대해 많은 의구심을 품고 있다. 하지만 이번 해커톤을 통해 오직 사업의 성공만을 위한 블록체인 연구가 아닌, 블록체인에 대하여 학문적으로 깊게 고민하며 접근하는 연구 팀이 늘고 있다는 것을 깨달았다. 실제로도 상위 학회에서 accept되는 블록체인 논문들의 수가 점점 늘어가는 상황에서, academic하게 블록체인에 대해 접근한다면 이 분야의 선구자가 되어 의미 있는 족적을 남길 수 있을 거란 자신감을 얻게 해준 좋은 경험이었다.

이번 해커톤에서 우리가 발표한 주제는  "A Layered Architecture for Querying on Blockchain" 이다. 기존 블록체인 시스템이 가지고 있는 가장 큰 문제점들은 다음과 같다.
 
* 각각의 attribute에 대한 indexing이 되어 있지 않다.
* Data analytics 수행이 불가능하다.
* data를 저장하는 값이 비싸다.

예를 들어, 누군가가 다음과 같은 보험 기록을 블록체인에 올려놓았다고 해 보겠다.

![Insurance Field Example](/files/2018-08-26/ex1.png)

현재 블록체인에서, 위 보험기록을 검색할 수 있는 유일한 방법은, 블록의 맨 앞에서부터 transaction id를 통해 일일이 블록 내의 트랜잭션을 들여다 보며 해당 attribute가 내가 찾고자 하는 것이 맞는지 확인하는 방법이다. 또한, 블록체인에서는 위의 정보가 hexadecimal encoding된 형태로 저장이 되기 때문에, 저장한 record의 attribute 정보를 알지 못하면, 원래의 정보를 확인하는 것이 불가능하다.

그래서 우리는 위에서 나열한 문제점을 다음과 같이 해결하였다.

* blockchain과 database을 통합한 2-layer synchronize architecture를 도입하여 블록체인의 특성인 immutability와, DB의 특성인 performance, analytics 를 모두 포함하는 방법을 제시
* distinct한 attribute에 대하여 dictionary encoding을 적용하여 블록체인에 저장되는 데이터의 용량을 최소화
Database를 통한 data analytics 까지 수행
* Database에 담긴 data의 위,변조가 의심된다면, 언제든지 sychronizing을 통해 블록체인에 담긴 정보를 Database로 load할 수 있도록 함

위 내용에 대한 demo 영상을 첨부한다.

[demo link](https://www.youtube.com/watch?v=EzoG1hWP9eA)

다른 팀들의 발표는 주로 Dapp과 관련된 프로젝트가 많았는데, 그 속에서 우리 팀은 블록체인과 관련하여 systematic한 접근을 했기 때문에 더 돋보이지 않았나 생각된다. 난생 처음 해외에서 진행한 해커톤에서 이토록 좋은 결과를 얻을 수 있어 기분이 좋았고, 결과를 넘어서 좋은 경험을 했다고 생각한다.
 
