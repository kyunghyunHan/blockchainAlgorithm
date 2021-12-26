# 👩🏻‍🎓블록체인 합의 알고리즘(blockchain consensus algorism)

![190924_consensus](https://user-images.githubusercontent.com/88940298/147365249-f83e1a95-c973-465c-97ad-014dda903ba9.png)
## 합의 알고리즘이란?

합의란 ‘서로 의견이 일치하거나 혹은 그 의견’이라는 사전적 의미를 가지고 있습니다. 즉, 합의를 한다는 것은 특정 문제 혹은 사건과 관련하여 이해 관계를 맺고 있는 사람들 간의 의견을 일치해 가는 것을 말합니다. 블록체인을 공부하다 보면 우리는 심심치 않게 ‘합의 알고리즘’이라는 개념을 자주 접하게 됩니다. 그 만큼 합의의 개념은 블록체인의 원리를 이해하는데 있어서 가장 기초적이면서 동시에 가장 중요한 역할을 담당하고 있습니다.

## 합의 알고리즘 종류
- 작업증명 (Proof of Work, PoW) 
- - 대표코인 :비트코인,라이트코인,제트캐시,모네로 등
- 지분증명 (Proof of Stake, PoS) 
- - 대표코인 :퀸텀,네오,스트라티스
- 위임 지분 증명(DPos, Delegated Proof of Stake)
- - 대표코인 :스팀,이오스,아크,라이즈

## 각 알고리즘 장단점 
### 👩🏻‍🎓작업증명(Proof of Work, PoW) 
#### 장점
- 최소 가격대 형성이 확실하게 정해져 있음
- 강력한 보안성
- 서비스 남용을 쉽게 방지

#### 단점
- 채굴 난이도가 높아지면서 연산에 필요한 고사양 장비가 많이 필요하고,과도한 전력 소모로 인한 에너지 낭비가 커짐
- 채굴 난이도가 높아지면서 개인 채굴자는 채굴을 할수 없는 수준까지 옴
- 지속적으로 해시파워를 유지해야함
- 채굴하는 업자끼리의 단합문제


### 지분증명(Proof of Stake, PoS) 
#### 장점 
- 해쉬파워가 많이 필요하지 않아 경제적이며 친환경적
- 블록 생산자의 탈중앙화로 안정성 확보
- 블록을 생성하기 위해서는 지분을 담보로 잡아야 하기 떄문에 덤핑 방지

#### 단점
- 모두 이자를 받으려고 코인을 묶어놓기 때문에 시중 코인의 유통량 감소로 이어질 수 있음
- 검증이 되지 않았기 떄문에 보안성이 강한지 확신할 수 없음
- 코인을 많이 보유한 사람이 권력을 지게되는 구조 (부익부 빈익빈)

### 👩🏻‍🎓위임지분증명 (DPos, Delegated Proof of Stake)
#### 장점
- 소규모 참여자도 이득을 볼 수 있음
- 송금속도가 빠름
#### 단점
- 상위 노드만 블록생성에 참여하기 때문에 탈중화가 맞는지 에매함
- 상위 노드만 블록생성에 참여하기 떄문에 보안이 취약함
- 코인 보유량이 적어도 상위 노드로 뽑힐 수 있음

## POW ->POS전환 이유 (이더리움)
- 첫째는 속도
작업증명 일때보다 지분증명 전환시 컨펌속도가 5배 가까이 빨라지게 됩니다.
- 두 번째는 블럭체인이 기업형 채굴가들에게 휘둘리지 않기 위해서입니다.
비트코인은 채굴 기업 몇개가 거의 모든 의사결정을 하게 됩니다.
작년 비트코인 세그윗 사태 때 비트코인캐쉬가 생겨난 거랑 소프트 포크 반대로 비트코인 분열 위기가 발생한 것도 이러한 단점 때문입니다.
작년말에 비트코인은 하드포크 시행 예정인데 분열위기로 시행 취소 됐었죠..
이렇게 가상화폐의 취지가 탈중앙화 인데 기업형 채굴자에게 오히려 휘둘리는 또 다른 중앙화가 되지 않도록 하기 위함이 두 번째 목적이 되겠습니다.
결론은 pos로 전환되면 화폐의 탈중앙화가 더 용이하고 블럭체인이 고속화 되고 이더리움을 보유할 수록 가치가 증가되니까 블럭체인이 안정화되고 이런 것을 위해서 전환 하고 있다고 생각하시면 됩니다.


## 지분증명이란
![images (2)](https://user-images.githubusercontent.com/88940298/147388067-e2440510-d898-4434-ac32-9f98b171ca24.jpeg)

Proof of Stake의 약어로 보유한 지분에 따라서 화폐를 얻게 되는 방식

- 기존 작업증명(Proof of Work)은  간략히 요약하자면 컴퓨터의 연산력을 바탕으로 합의에 도달하고 그 연산력이 빠를수록 블록에 기록할 수 있는 권한이 더 많이 부여된다는 것이 핵심!!
- Proof of Stake(지분증명)는 작업이 아닌 더 많은 지분(해당 코인)을 가지고 있을수록 그에 비례하여 블록에 기록할 권한이 더 많이 부여되는 것!!!!! 
- 코인을 가지고 있는 노드들 모두가 합의를 통해 블록에 데이터를 추가 할 수 있게 되는 것이고 코인을 많이 가진 노드는 데이터를 업데이트할 권한이 더 많이 주어지는 것이 Proof of Stake이고 PoW와 마찬가지로 블록이 생성될때 보상이 지급되는데 지분에 대한 이자의 개념으로 보상이 지급!!!!!

