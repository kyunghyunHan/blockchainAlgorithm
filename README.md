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
```
시스템상에서 다음 블록 생성자는 해당 코인을 특정양 보유하고 있는 주주들 중 선출되는 것
자신의 코인 양에 따라 이자가 발생하는 방식이기에 별도의 채굴기가 필요하지 않다.
채굴하고자 하는 코인을 지갑에 보유하면 그 보유량만큼 작업을 증명할 수 있는 지분을 갖게 되는 것
```

- 기존 작업증명(Proof of Work)은  간략히 요약하자면 컴퓨터의 연산력을 바탕으로 합의에 도달하고 그 연산력이 빠를수록 블록에 기록할 수 있는 권한이 더 많이 부여된다는 것이 핵심!!
- Proof of Stake(지분증명)는 작업이 아닌 더 많은 지분(해당 코인)을 가지고 있을수록 그에 비례하여 블록에 기록할 권한이 더 많이 부여되는 것!!!!! 
- 코인을 가지고 있는 노드들 모두가 합의를 통해 블록에 데이터를 추가 할 수 있게 되는 것이고 코인을 많이 가진 노드는 데이터를 업데이트할 권한이 더 많이 주어지는 것이 Proof of Stake이고 PoW와 마찬가지로 블록이 생성될때 보상이 지급되는데 지분에 대한 이자의 개념으로 보상이 지급!!!!!

- 간단하게 말하자면 돈 낸만큼 피자먹자  
![스크린샷 2021-12-28 오전 2 05 42](https://user-images.githubusercontent.com/88940298/147492790-0cbfa348-b632-4a9b-9930-3655ab28faf4.png)



## 지분증명이 원리
![다운로드](https://user-images.githubusercontent.com/88940298/147492898-bc1f3b8b-0e22-4c05-9bd5-004a16fd751f.png)


- 그림을 보면 B가 지분이 제일 많아 40% 확률로 권한을 획득하여 블록을 형성하고 나머지 노드들은 검증자 (validator)로써 자산들을 증명하게 되고 거래들의 수수료로 나온 보상으로 지분에 대한 이자를 지급된다.
확률상으로 봤을 때 10개의 블록이 형성되면, A는 3개 , B는 4개 , C는 3개 를 형성하게 된다.

![다운로드 (3)](https://user-images.githubusercontent.com/88940298/147492984-03349e25-11a0-4dac-9a25-7b5a0e9ca72a.png)
- 블록을 형성하면 노드들은 블록에 합의를 하기 위해 자신들의 지분을 증명하게 된다. 
- 지분이 많을수록 체인을 계속해서 유지할 것이고 블록체인에 참여를 하게 되는 노드들은 ①지분에 따라 공평하게 블록 형성 권한을 받고 블록 형성 시 발생하는 보상을 지분만큼 이자로 받는 개념이 적용되는 것이다.
- 또한, 참여한 노드들은 자신이 합의하는 블록들을 증명하고 나눠진 체인들은 ②더 많은 지분을 검증하는 블록을 보유하는 체인으로 합의가 이뤄진다.

#### 그럼 블록 형성할 노드를 어떻게 선출하지?
- 보통 지분의 크기에 따라 블록의 형성할 확률이 결정되는데 일반적인 확률상으론 가장 지분이 많은 노드만 선택되는 것을 방지해야 하며 대표적으로 아래 방식들이 있다.
##### Randomized Block Selection
- 각 노드들 중 가장 낮은 해시값과 가장 높은 지분의 조합을 가진 노드를 검증자로 선택
##### Coin Age Selection
- 토큰이 얼마나 오래 Staking 되었는지에 따라 선택. 코인을 Staking 한 일수 x 코인의 지분 크기로 선출하게 된다. 
- 계속해서 선출되는 것을 막기 위해 Staking 일수를 aging 한다. 한번 선출되면 다시 Staking 일수를 0 부터 시작한다.



##  PoS (지분증명) -기존 pow(작업증명)방식

- 채굴 난이도가 높아지면서 연산에 필요한 고사양 장비가 많이 필요하고,과도한 전력 소모로 인한 에너지 낭비가 커짐 

- 채굴 난이도가 높아지면서 개인 채굴자는 채굴을 할수 없는 수준까지 옴

- 지속적으로 해시파워를 유지해야함


## PoS (지분증명) 로 넘어오면서
- 해쉬파워가 많이 필요하지 않아 경제적이며 친환경적

- 블록 생산자의 탈중앙화로 안정성 확보

- 블록을 생성하기 위해서는 지분을 담보로 잡아야 하기 떄문에 덤핑 방지

## PoS (지분증명) 로 넘어오면서 발생하는 문제점
### 51% 공격의 위험은 없을까

일반적으로 블록체인 네트워크의 51%가 동시에 공격을 진행하면 해당 블록체인은 신뢰성을 잃게 됩니다. 이를 ‘51% 공격’이라고 칭합니다. 이에 51%의 지분을 보유한 사람이 존재한다면 쉽게 악의적인 공격이 가능하지 않냐는 가설이 생겼는데,엄청난 에너지와 기타 자원을 소모해야 하는 작업증명과 달리 지분증명은 지분만 있으면 누구나 쉽게 블록 생성 권한을 가질 수 있기 때문인데 그러나 다음과 같은 이유로 오히려 지분증명이 작업증명보다 분산화가 잘되어 있다고 말할 수 잇습니다.
- 작업증명 에서 51%의 해시파워를 가지는 비용 = 약 2,500억원
- 지분증명 에서 전 세계 자산의 51%를 보유하는 비용 = 약 25조원 
이렇게 독점 권력을 갖기 위해서 지분증명 방식이 작업증명의 방식보다 약 100배 정도 비용이 더 들뿐만 아니라, 지분증명에서는 누구나 코인만 가지고 있으면 네트워크 참여가 가능하기 때문에 분산화가 더 잘되어 있다고 말합니다. 
### 초기 지분 보유량이 많을 수록 유리하지 않을까

- 처음 지분증명 방식이 제안되었을 때 초반에 지분을 많이 확보해 두면 블록 생성 권한을 지속적으로 갖게 되는 ‘불평등’의 문제가 제기. 이에  보완책으로 내놓은 것이 보유한 코인의 ‘양’과 ‘보유 일수’를 반영하는 것이었습니다. 
- 대표적인 예가 바로 ‘Peercoin’입니다. 예시로 A가 10개의 코인을 10일 동안 보유했다면 100의 가치를 갖게 하는 것입니다. (만약 해당 코인을 사용한다면 100의 가치가 소모되고 처음부터 다시 시작됩니다) 이 경우에 보유 코인이 적어도 보유 일수가 길면 블록을 생성할 수 있는 확률이 높아지기 때문에 보다 균등하게 기회가 주어집니다
![unnamed](https://user-images.githubusercontent.com/88940298/147493311-82964f6f-ee22-40d1-b691-a36659ca5e88.png)


## Nothing-at-Stake 문제가 발생한다는데
일단 블록을 형성할 때 악의적으로 fork를 발생시켜 여러 branch가 생길 경우, Validator들은 어떤 블록이든 자신의 지분을 증명하게 될 것이다
Chain의 길이에 따라서 두가지 Attack이 발생한다.


![다운로드 (1)](https://user-images.githubusercontent.com/88940298/147493358-a7420a34-2666-4461-a8fa-2bd8cc197915.png)

지분이 많은 Validator가 악의적인 목적으로 두 체인의 블록을 모두 올바른 블록이라 검증하는 것이다.
그렇게 긴 체인이 형성된 경우 새로 참여한 Validator는 모든 체인이 올바르다고 생각할 것이다. 이 경우 새로 참여한 Validator가 지분이 많으면 악의적인 블록에도 합의를 해버리게 되므로 올바른 거래들도 모두 공격 당하는 형태가 된다.

![다운로드 (2)](https://user-images.githubusercontent.com/88940298/147493363-b4dff71f-cc0d-4918-ac1f-0fe134d56c66.png)

일단 악의적인 fork가 발생하고 나면, Validator들은 항상 두쪽 체인을 합의하려고 할 것이다. 두 체인에 대해 자신의 지분을 증명했다면 어떤 체인이 선택되든 보상받을 수 있기 때문이다. 
이렇게 악의적인 체인이 발생했을 때 양쪽에 지분 증명을 해도 잃을 것이 없다는 'Nothing at Stake' 문제가 있다는 것이다. 이 문제는 체인 유지를 함에 있어서 큰 문제이다.

#### 이럴때 해결방안
- 리워드를 통해 획득한 지분은 특정 기간 이후 사용 가능하게 하여 검증할 수 있는 네트워크 시간을 확보하고
- 만약에 노드 형성 시 악의적인 거래가 발견될 경우 형성자는 지분을 잃고 추후 블록 형성에 참여할 수 없다.
- 최근에는 전력 소비로 인한 환경문제 때문에 PoS를 채택한 블록체인 플랫폼들이 많아지고 있으며 필연적으로 보인다. 


## 이더리움 2.0(예시)      POW -> POS 전환

이더리움이 pow에서 pos로 전환하려는 이유는 크게 두 가지입니다.
```
          첫째는 이더리움 블록체인을 고속화 하기 위해서
                                          pow일때보다 pos전환시 컨펌속도가 5배 가까이 빨라지게 됩니다.
                                    두 번째는 블럭체인이 기업형 채굴가들에게 휘둘리지 않기 위해서입니다.
비트코인은 채굴 기업 몇개가 거의 모든 의사결정을 하게 됩니다.이렇게 가상화폐의 취지가 탈중앙화 인데 기업형 채굴자에게 오히려 휘둘리는 또 다른 중앙화가 되지 않도록 하기 위함

```
- 이더리움 개발팀은 이런 pow pos 전환을 용이하게 하기위해서 바로 전부 전환하지 않고 1프로를 먼저 pos로 전환 하고 점차 그 비중을 늘리는 방식을 선택했습니다
- 그 과정에서 난이도 폭탄이 터지도록 설정해서 pow로 얻을 수 있는 양이 급격히 줄도록 설계돼있어서 pow에서 pos로의 전환이 자연스럽게 이행 되게끔 계획되어 있습니다
- 또한 캐스퍼라는 이름으로 pow pos 전환 프로젝트를 진행하는데 이 캐스퍼 프로젝트가 비트코인처럼 업그레이드 하고 나면 그걸 거부하고 기존 코인을 채굴해서 쪼개지고 하는 걸 막을 수 있습니다.
- 51프로 이상이 동의하지 않는데 생성된 블록들은 캐스퍼에 의해 소멸 되도록 해버리는 거죠. 그래서 이더리움은 이제 쪼개질 위험은 없다고 판단되는 것입니다

#### 여기서 잠깐
❓캐스퍼 프로젝트란❓
- 이더리움의 합의 알고리즘인 PoW를 PoS로 전환하는 것을 목표로 하는 프로젝트

- 캐스퍼 네트워크는 캐스퍼 CBC 사양으로 구축된 최초의 라이브 베팅 증거 블록체인입니다. Casper는 오늘날 기업과 개발자의 블록체인 기술 채택을 가속화하고 미래의 사용자 요구를 충족하도록 진화하도록 설계되었습니다.

❓캐스퍼가 기존의 POS와 다른 점은?❓ 
캐스퍼(Casper) POS 작동 방식의 핵심 중 하나가 악한 행위를 하는 검증인들을 처벌하는 것입니다.  
- 검증인들은 블록을 검증 전에 자신의 이더 지분을 맡겨야 합니다 (테스트넷에서는 최소 1,500 이더 필요) 
- 검증인들은 체인의 연결 될 것이라고 믿는 블록에 원하는 만큼 베팅을 합니다. 
- 만약 자신이 베팅한 블록이 체인의 연결이 되면 검증인들은 베팅한 만큼 보상을 받게 됩니다. 
- 그러나 검증인들이 Nothing-at-stake 문제와 같이 체인을 어지럽히는 악한 행위를 하면 처벌을 받게 됩니다. 여기서 처벌이란 검증인들은 자신이 걸어 놓았던 지분을 몰수당하는 걸 의미합니다.

### 결론은 pos로 전환되면 화폐의 탈중앙화가 더 용이하고 블럭체인이 고속화 되고 이더리움을 보유할 수록 가치가 증가되니까 블록체인이 안정화되고 이런 것을  위해서 전환 하고 있다고 생각하시면 됩니다.

