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

## 지분증명이 원리
- 블록 생성 및 검증의 역할을 하는 Validator가 되기 위해서는 자신이 보유하고 있는 암호 화폐를 보증금의 형태로 락업하는 특별한 거래(Special Transaction)를 해야 합니다.

- 그 이후에는 새로운 블록을 생성하고 검증하는 절차는 모든 Validator가 참여할 수 있도록 하는 특정 ‘합의 알고리즘(Consensus Algorithm)’에 의해 이루어집니다.

여기서 중요한 점은 바로 특정 합의 알고리즘이 하나가 아니라는 것입니다. 이에 “지분증명 자체가 합의 알고리즘 아닌가”하는 의문이 드실 수 있습니다. 맞습니다. 그러나 여기서 말하는 특정 합의 알고리즘이란 지분증명이라는 큰 틀 안에서 블록 생성 및 검증, 그리고 보상에 관한 알고리즘을 말합니다. 따라서 그 방법에 따라 지분증명은 다양한 형태가 될 수 있습니다. 가장 대표적인 형태로 ‘Chain-Based Proof-of-Stake’와 ‘BFT-Style Proof-of-Stake’가 있습니다.


Chain-Based Proof-of-Stake에서는 10초 단위의 매 슬롯마다 하나의 Validator를 의사 랜덤하게 (pseudo-randomly) 선정합니다. 선정된 Validator는 블록 한 개를 생성할 수 있는 권한을 갖게 됩니다. 그러나 생성된 블록은 반드시 이전 블록 중 하나를 가리켜야 하는데 보편적으로 길이가 가장 긴 체인의 마지막 블록을 가리키게 됩니다. 이에 결과적으로 대부분의 블록들은 단일의 체인에 모이게 됩니다. 지분증명의 가장 기본적인 형태라고 볼 수 있습니다.

BFT-Style Proof-of-Stake에서는 Validator들에게 완전히 랜덤하게(randomly) 블록을 제안(propose) 할 수 있는 권한이 주어집니다. 다만 어떤 블록이 정규 블록인지에 대한 합의는 여러 라운드에 걸쳐 이루어집니다. 매 라운드 마다 모든 Validator는 특정 블록에 ‘투표’를 할 수 있습니다. 그리고 모든 라운드가 끝나면 Validator는 어떤 블록이 체인의 부분인지 아닌지 영구적으로 합의하게 됩니다. 특이한 점이 있다면 길이가 길거나 사이즈가 큰 체인의 블록이 남는 것이 아니라 많은 합의를 받은 단 한 개의 블록만이 남을 수도 있다는 것입니다.

필자가 지분증명의 개념을 이해하는데 있어서 가장 힘들었던 부분은 바로 다양한 형태의 PoS가 존재함에도 불구하고 잘 알려지지 않았다는 점이었습니다. 작업증명의 경우 대표적인 비트코인 사례가 표본이 되었지만 지분증명은 ‘참여자의 소유 지분이 블록 생성 권한에 영향을 미친다’는 의제를 큰 틀에서 공유하고 있을 뿐 세부적인 부분에 있어서는 많은 차이가 있습니다. 따라서 앞으로 지분증명의 합의 알고리즘을 공부하는데 있어 항상 염두에 두시길 바랍니다.

### 51% 공격의 위험은 없을까
 일반적으로 블록체인 네트워크의 51%가 동시에 공격을 진행하면 해당 블록체인은 신뢰성을 잃게 됩니다. 이를 ‘51% 공격’이라고 칭하고 있습니다. 이에 지분증명 방식과 관련해서 51%의 지분을 보유한 사람이 존재한다면 쉽게 악의적인 공격이 가능하지 않냐는 가설이 생겼는데, 왜냐하면 엄청난 에너지와 기타 자원(채굴기, 넓은 평지 등)을 소모해야 하는 작업증명과 달리 지분증명은 지분만 있으면 누구나 쉽게 블록 생성 권한을 가질 수 있기 때문인데 그러나  다음과 같은 이유로 오히려 지분증명이 작업증명보다 분산화가 잘되어 있다고 말할 수 잇습니다.

- 작업증명 에서 51%의 해시파워를 가지는 비용 = 약 2,500억원
- 지분증명 에서 전 세계 자산의 51%를 보유하는 비용 = 약 25조원
이렇게 독점 권력을 갖기 위해서 지분증명 방식이 작업증명의 방식보다 약 100배 정도 비용이 더 들뿐만 아니라, 지분증명에서는 누구나 코인만 가지고 있으면 네트워크 참여가 가능하기 때문에 분산화가 더 잘되어 있다고 말합니다. 그러나 또 한편에서는 단순 수학적 계산으로 비교할 수 있는 부분이 아니라고 주장하기도 합니다. 왜냐하면 블록체인의 런칭 시기 및 화폐 발행량을 포함한 다양한 요인들로 인하여 51% 지분을 확보하는 비용이 천차만별일 수도 있기 때문입니다.

## 초기 지분 보유량이 많을 수록 유리하지 않을까
처음 지분증명 방식이 제안되었을 때 초반에 지분을 많이 확보해 두면 블록 생성 권한을 지속적으로 갖게 되는 ‘불평등’의 문제가 제기되었습니다. 이에 대한 보완책으로 내놓은 것이 보유한 코인의 ‘양’과 ‘보유 일수’를 반영하는 것이었습니다. 대표적인 예가 바로 ‘Peercoin’입니다. 예를 들어 A가 10개의 코인을 10일 동안 보유했다면 100의 가치를 갖게 하는 것입니다. (만약 해당 코인을 사용한다면 100의 가치가 소모되고 처음부터 다시 시작됩니다) 이 경우에 보유 코인이 적어도 보유 일수가 길면 블록을 생성할 수 있는 확률이 높아지기 때문에 보다 균등하게 기회가 주어집니다.

## Nothing-at-Stake 문제가 발생한다는데
Nothing-at-Stake란 말 그대로 잃을 것이 없다는 뜻입니다. 예를 들어 유효한 블록체인이 두 개 이상 존재하는 포크(fork) 상황이 발생했다고 가정해 봅시다. 작업증명 방식에서는 블록을 생성하는데 막대한 양의 컴퓨팅 파워와 전기를 소모하기 때문에 하나의 블록을 지정하여 그 다음 블록을 생성하게 됩니다. (다만 고아 블록이 될 가능성은 존재합니다) 그러나 지분증명 방식에서 Validator는 포크된 모든 블록에 지분을 투표할 확률이 높습니다. 왜냐하면 컴퓨팅 파워와 같은 기회 비용이 존재하지 않고 합의 방법에 별다른 제한이 없기 때문에 양쪽 모두에 지분을 증명해 놓아야 보상 받을 가능성을 높일 수가 있는 것입니다. 이에 Nothing-at-Stake 문제를 해결하기 위한 ‘Slash’ 제도가 도입이 됩니다. 만약 Validator가 여러 블록에 지분을 증명하거나 잘못된 블록에 지분을 증명하게 되면 해당 지분은 Slash, 즉 사라지게 됩니다. 또한 지분 증명 행위 자체에도 일정 수준의 보증금을 내게 하여 잘못된 행위를 할 경우에도 Slash 하는 등 ‘Nothing-at-Stake’를 ‘Something-at-Stake’로 만들어 해당 문제를 해결해 나가고 있습니다.

## BFT, Byzantine Fault Tolerance란
대표적인 지분증명 방식 중 하나가 BFT-Style이라고 했는데 BFT(Byzantine Fault Tolerance)가 무엇인지 알기 위해서는 Byzantine Generals’ Problem을 알아야 합니다. Byzantine Generals’ Problem란 비잔틴 제국의 여러 장군들이 하나의 적군을 공격하기 위해 출격을 하는데, 적군과의 전쟁에서 승리하기 위해서는 과반수 이상의 장군들이 같은 시각에 공격을 해야 합니다. 그러나 장군들은 오직 연락병을 통해서만 소통을 할 수 있으며 장군들 중에는 한 명 이상의 배신자가 존재하기 때문에 어떻게 출격 시각을 합의할 것인가가 중요한 문제가 됩니다.

Byzantine Generals’ Problem은 2개의 기본 가정을 전제하고 있습니다. 첫 번째 가정은 배신자를 제외한 모든 장군들은 명령이 유효하다고 검증이 되면 이를 충실히 수행합니다. 두 번째는 배신자 m명은 전체 장군 수 n명의 1/3을 넘지 않습니다. 이때 위의 문제를 해결하기 위한 방법은 다음과 같습니다. (Commander = 'C', Lieutenant = 'L')

C는 그의 명령 내용 {v}를 모든 장군들에게 보냄
- 각각의 L(i)에 대해서 C에게 받은 명령 내용을 {v(i)}라고 한다면
- 각각의 L(i) 또한 {v(i)}의 내용을 다른 모든 장군들과 공유
- L(i)는 자신이 아닌 다른 L(j)로부터 명령 내용 {v(j)}를 수령
- L(i)는 {v(1), v(2), … , v(n-1)} 중 다수의 가치를 차지하는 명령을 수행
- 이를 특정 장군의 관점, 예를 들어 L(2)의 관점에서 도식화하면 이해하기 쉽습니다.

1*IVMEKaA35NAM6sjKT_R2aA.png
[그림 11. L3가 배신자일 때]
- 1단계: C는 모든 장군들에게 명령 내용 {v}를 보냄
- 2단계: L2는 L1로부터 {v}를, L3로부터 {x}를 수령
- 3단계: L2는 {v, v, x} 중 다수의 가치를 차지하는 {v} 명령 수행
Commander가 배신자인 경우에도 마찬가지입니다.

1*FqWerJdheG1CJoMquKKieg.png

[그림 12. Commander가 배신자 일 때]
- 1단계: C는 L1, L2, L3에게 각각 {x}, {y}, {z}를 보냄
- 2단계: L1은 {x}를 L2, L3에게, L2는 {y}를 L1, L3에게, L3는 {z}를 L1, L2에게 보냄
- 3단계: L1, L2, L3는 모두 {x, y, z}의 내용에 합의를 하게 되며 최종적으로 철수
문제의 핵심은 다수의 장군들이 특정 행동(출격)을 유도하는 것이 아닌 모두가 동일한 결정을 할 수 있게 하는 것이라고 보면 됩니다.

위의 알고리즘은 Byzantine Fault에 대한 해결책을 제시해 줍니다. 만약 특정 시스템이 다양한 요소들의 결과에 영향을 받아 움직이는 시스템이라고 한다면 이런 Byzantine Fault 문제를 잘 다루는 것이 중요합니다. Byzantine Fault Tolerance란 위와 같은 문제들을 다루는 방법에 대한 것으로 BFT-Style Proof-of-Stake란 분산화 되어 있는 블록체인 네트워크에서 악의적인 노드에 의해서 발생할 수 있는 문제들을 다수의 가치(Majority Value)로 해결하고 있음을 보여줍니다. (이는 사토시 나카모토가 비트코인을 처음 만들었을 때 이에 대한 해결책으로 제시한 작업증명 방식 논의에서 언급된 것으로 지분증명 방식만의 이슈는 아니라고 할 수 있습니다)

Conclusion
오늘은 정말 긴 분량에 걸쳐서 작업증명(Proof-of-Work)과 지분증명(Proof-of-Stake)에 대해서 알아보는 시간을 가졌습니다. 사실 처음에 필자가 합의 알고리즘에 대한 글을 쓰고자 결심했을 때는 이렇게까지 많은 내용이 있을 줄은 생각하지 못했습니다. 그러나 글을 쓰다 보니 합의 알고리즘과 관련하여 알아야 할 것들이 정말 많았으며 아직까지도 부족한 부분이 많다고 느껴질 정도입니다. 그래도 최대한 쉽게 그리고 자세하게 설명하고자 노력을 했고 블록체인에 입문하시는 여러분들에게 조금이나 도움이 되었길 진심으로 바랍니다. 다음 편에서는 미리 예고해 드렸듯이 위임된 지분증명(Delegated Proof-of-Stake)에 대해서 알아보도록 하겠습니다. 최근에 가장 주목받고 있는 합의 알고리즘인 만큼 많은 관심과 기대 부탁드립니다.

