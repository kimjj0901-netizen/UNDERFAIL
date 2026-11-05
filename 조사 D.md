# 조사 D — 루트 조건과 엔딩 분기

> 대상: UNDERTALE  
> 조사일: 2026-11-05  
> 조사 유형: Descriptive  
> 범위: Neutral · True Pacifist · Genocide 루트의 진입·유지·이탈 조건, 엔딩 분기, 회차 간 상태

---

## 1. Charter

### 목표

Undertale의 세 가지 주요 루트가 어떤 규칙으로 판정되는지, 도중에 루트가 무효화되는 조건은 무엇인지, 엔딩과 다음 회차에 어떤 상태가 남는지 정리한다.

### 범위 / 대상 / 구체적 조사 단위

- **범위:** RPG의 진행·선택·엔딩 분기 시스템
- **대상:** Undertale의 Neutral·True Pacifist·Genocide 루트
- **구체적 조사 단위:** 지역별 처치 카운터, 주요 인물 생존과 관계 조건, 이벤트 선후관계, 엔딩 판정, SAVE·LOAD·RESET과 회차 간 상태

### 연구 유형

**Descriptive.** 기본적인 루트 구조는 A~C 조사로 파악했으므로, 이번에는 세부 조건과 분기 규칙을 구체화하는 것이 목적이다.

### 조사 질문

1. Neutral·True Pacifist·Genocide의 진입 조건은 각각 무엇인가?
2. 루트 판정은 언제, 어떤 행동을 기준으로 이루어지는가?
3. 특정 행동 하나로 루트가 깨지는 경우와, 나중에 회복할 수 있는 경우는 어떻게 다른가?
4. Genocide의 지역별 처치 조건과 진행 중단 조건은 무엇인가?
5. True Pacifist의 선행 조건과 최종전 진입 조건은 어떤 순서로 연결되는가?
6. Neutral 엔딩은 어떤 변수와 생존 상태에 따라 달라지는가?
7. 루트별 최종 보스·전투·엔딩 연출은 어떻게 달라지는가?
8. 엔딩 이후의 상태와 RESET은 다음 플레이에 어떤 영향을 주는가?

### 해석 규칙

- 게임 내에서 확인되는 규칙과 위키가 붙인 비공식 엔딩 명칭을 구분한다.
- 자료에서 확인된 사실, 구조적 해석, 미확인 사항을 서로 섞지 않는다.
- 정확한 내부 판정 변수나 소스 코드를 직접 확인하지 못한 항목은 게임 내부 구현을 확인한 것처럼 단정하지 않는다.
- Undertale Wiki는 세부 조건을 확인하는 데 사용한 2차 자료다. 개발자가 공개한 공식 규칙 문서로 취급하지 않는다.

---

## 2. Canonical sources — 출처 및 신뢰도

| 순위 | 출처 | 이번 조사에서의 역할 | 한계 |
|---|---|---|---|
| 1차 | Toby Fox가 제작한 Undertale 본편 | 실제 게임 규칙을 판단하는 원본 | 이번 조사에서 모든 루트를 직접 재실행하거나 내부 판정 코드를 확인하지 못함 |
| 2차 | [Undertale 공식 홈페이지](https://undertale.com/) 및 공식 배포 정보 | 작품과 제작 주체 확인 | 루트별 세부 판정표는 확인하지 못함 |
| 3차 | 본편을 직접 실행해 확인하는 기록 | 실제 동작을 교차검증하는 자료 | 이번 환경에서 별도 실행하지 못함 |
| 4차 | [The Undertale Wiki — Endings](https://undertale.wiki/w/Route), [Genocide Route](https://undertale.wiki/w/Genocide_Route), [Neutral Route](https://undertale.wiki/w/Neutral_Route), [True Pacifist Route](https://undertale.wiki/w/Pacifist), [True Lab](https://undertale.wiki/w/True_Lab) | 세부 조건·예외·분기 구조 정리 | 팬 위키의 2차 정리이며, 게임 내부 코드의 직접 증거는 아님 |

**조사 한계:** 아래의 세부 조건은 주로 Undertale Wiki의 공개 정리를 근거로 한다. 공식 사이트에서 세부 루트 규칙을 확인하지 못했고, 원본 게임의 내부 판정 코드를 직접 열람하지 못했다. 따라서 세부 수치와 예외는 해당 위키의 정리 기준으로 제시한다.

---

## 3. Findings ledger — 조사 결과 장부

### F1. Undertale의 세 가지 주요 루트는 서로 다른 판정 구조를 가진다.

| 루트 | 기본적인 성격 | 진입 구조 |
|---|---|---|
| Neutral | 폭력·비폭력 선택이 혼합된 기본 진행 | 특별한 루트 조건을 충족하지 못하면 도달하는 기본 루트 |
| True Pacifist | 몬스터를 처치하지 않고 관계를 회복하는 진행 | Neutral 엔딩 완료가 선행되어야 함 |
| Genocide | 지역별 처치 조건을 끝까지 충족하는 진행 | 첫 지역인 Ruins부터 처치 카운터를 소진하면서 시작 |

Neutral은 Asgore 전투와 엔딩을 거치는 기본 루트다. True Pacifist는 Neutral 엔딩을 완료한 이후 관련 퀘스트가 열린다. 반면 Genocide는 첫 번째 플레이에서도 진입할 수 있다.

근거: [Endings](https://undertale.wiki/w/Route), [Neutral Route](https://undertale.wiki/w/Neutral_Route), [Genocide Route](https://undertale.wiki/w/Genocide_Route)

### F2. True Pacifist의 핵심 조건은 공격 입력 자체가 아니라 처치·EXP 기록이다.

True Pacifist의 기본 조건은 다음과 같다.

1. Neutral 엔딩을 완료한다.
2. 게임 전체에서 몬스터를 처치해 EXP를 얻지 않는다.
3. Papyrus, Undyne, Alphys와의 관계 이벤트를 완료한다.
4. True Lab을 탐험한다.

LV는 EXP 획득과 연결되므로, EXP를 얻지 않으면 LV 1을 유지한다. 다만 이를 단순히 모든 전투에서 FIGHT를 선택하면 안 된다는 규칙으로 이해하면 틀린다.

자료에서는 적을 공격하더라도 처치하지 않거나, EXP를 주지 않는 특정 대상과 상호작용하는 경우 True Pacifist 진행을 반드시 무효화하지는 않는다고 설명한다. 예를 들어 몬스터를 쓰러뜨리지 않는 FIGHT, Ruins의 Dummy 처치, 특정 선택지에서 공격을 받지만 EXP를 얻지 않는 경우는 조건에 영향을 주지 않는 예외로 정리되어 있다.

핵심 판정 기준은 공격 버튼을 눌렀는지가 아니라 **게임이 몬스터 처치와 EXP 획득으로 기록했는지**에 가깝다. 우발적으로 몬스터를 처치했다면, 그 행동 이전의 SAVE를 불러와 되돌릴 수 있는 경우가 있다. 이미 EXP를 얻은 상태라면 초기화가 필요할 수 있다.

근거: [True Pacifist Route](https://undertale.wiki/w/Pacifist), [Endings](https://undertale.wiki/w/Route)

### F3. True Pacifist는 순서가 있는 연쇄 퀘스트다.

#### True Pacifist 진행 순서

1. **Neutral 엔딩 완료**
   - Asgore와 Omega Flowey 관련 진행을 마친다.
   - Neutral 엔딩 완료 후 SAVE를 다시 불러와 추가 조건을 수행할 수 있다.
   - 새 게임을 시작하는 Reset은 필수 조건이 아니다. 다만 EXP를 얻었다면 조건을 다시 충족하기 위해 Reset이 필요할 수 있다.

2. **Papyrus와의 관계 이벤트**
   - Papyrus와의 전투를 마친 뒤 Snowdin에 있는 그의 집을 방문한다.
   - 데이트 또는 교류 이벤트를 완료한다.

3. **Undyne을 돕는다**
   - 추격 이후 쓰러진 Undyne에게 물을 건넨다.
   - 물을 주지 않고 방을 떠나면 이후 교류 이벤트를 진행할 수 없게 될 수 있다.

4. **Undyne과의 교류 이벤트**
   - Waterfall의 Undyne 집을 방문한다.
   - Papyrus와 함께 들어가 교류 이벤트를 완료한다.

5. **Mettaton EX 전투를 비살상으로 마무리**
   - Mettaton EX 전투에서 관객 평가 점수 조건을 달성한다.
   - 위키 정리 기준 10,000점, 다리를 유지한 경우 12,000점이 요구된다.
   - 이 조건을 충족하면 전투를 평화롭게 끝낼 수 있다.

6. **Undyne의 편지**
   - Undyne에게 편지를 받아 Alphys에게 전달하는 이벤트가 열린다.
   - 편지를 버린 경우 다시 받을 수 있는 예외 경로가 존재한다.

7. **Alphys와의 교류 이벤트**
   - Undyne의 편지를 Alphys 연구실 문 아래로 전달한다.
   - Alphys와의 데이트 이벤트를 완료한다.

8. **True Lab 진입**
   - Alphys의 연구실에서 새로운 단서를 확인한다.
   - 연구실의 숨겨진 문을 통해 True Lab으로 내려간다.
   - 엘리베이터가 고장 나면서 진행을 계속해야 하는 상황이 발생한다.

9. **True Lab 조사 완료**
   - 내부에 흩어진 네 개의 열쇠를 찾아 발전기실을 연다.
   - 발전기를 작동시킨 뒤 엘리베이터로 이동한다.
   - 이후 New Home으로 이동하며 출구가 막혀 사실상 결말 진행이 고정된다.

10. **최종전과 진정한 엔딩**
    - 최종 사건을 거쳐 장벽이 무너지고 괴물들이 지상으로 나간다.
    - 에필로그에서 Toriel과 함께할지 여부에 따라 마지막 장면이 달라진다.

근거: [True Pacifist Route](https://undertale.wiki/w/Pacifist), [True Lab](https://undertale.wiki/w/True_Lab)

#### 이 연쇄 구조의 의미

친구 관계 → 편지 → 연구실의 비밀 → 진정한 결말이 하나의 연쇄 구조를 이룬다. 관계 이벤트는 독립된 수집 요소가 아니라 다음 단계의 서사를 여는 열쇠로 기능한다.

주요 예외는 다음과 같다.

- Undyne이 쓰러진 상태에서 물을 건네지 않고 떠나면 이후 교류 이벤트를 진행할 수 없게 된다.
- Mettaton EX 전투는 관객 평가 점수 조건과 연결된다.
- Undyne의 편지를 버리더라도 다시 받을 수 있는 경로가 있다.
- True Lab 진입은 True Pacifist 루트의 사실상 되돌릴 수 없는 지점이다. 진입 후에는 대부분의 지하 세계로 돌아갈 수 없고, 진행이 결말로 이어진다.

근거: [True Pacifist Route](https://undertale.wiki/w/Pacifist), [True Lab](https://undertale.wiki/w/True_Lab)

### F4. Genocide는 단순히 많이 처치하는 루트가 아니다.

Genocide에서 가장 중요한 시스템은 **지역별 처치 카운터**다. 한 지역에서 요구되는 수를 충족해야 다음 주요 보스 단계로 진행할 수 있다. 일부 특수 적은 일반 카운터와 별도로 처치 조건이 존재한다.

#### 지역별 조건

| 지역 | 일반 처치 카운터 | 별도 확인 대상 | 보스 |
|---|---:|---|---|
| Ruins | 20 | Napstablook은 카운터에 포함되지 않음 | Toriel |
| Snowdin | 16 | Snowdrake, Doggo, Dogamy와 Dogaressa, Greater Dog 등 | Papyrus |
| Waterfall | 18 | Shyren, Glad Dummy 등 | Undyne the Undying |
| Hotland / CORE | 40 | Royal Guards, Muffet | Mettaton NEO |
| New Home | 별도 카운터 없음 | 지역 카운터가 아니라 최종 진행 | Sans |

이 숫자는 지역별 일반 조우 카운터다. 특수 적과 보스 조건까지 포함한 전체 조건을 단순히 이 숫자만으로 설명할 수는 없다.

**예외와 주의사항**

- Ruins의 Napstablook은 카운터에 포함되지 않는다.
- Toriel은 Ruins의 카운터를 소진하기 전에 만날 수도 있다. 이때 전투 상태가 일반 Neutral 진행과 다르게 처리되며, 처치하면 Ruins 카운터에 반영되는 예외가 있다.
- Snowdin의 Snowdrake는 카운터를 소진하기 전에 처치해야 하는 조건이 있다.
- Lesser Dog는 필수 특수 적으로 분류되지는 않지만, 만났다면 처치해야 하는 조건으로 정리되어 있다.
- Doggo, Dogamy와 Dogaressa, Greater Dog는 일반 카운터에 포함되지 않지만 별도로 처치해야 하는 특수 조건에 해당한다.
- Waterfall에서는 Shyren과 Glad Dummy 조건이 별도로 존재하며, Undyne the Undying 전투로 이어지는 조건도 중요하다.
- Hotland/CORE에서는 Royal Guards와 Muffet을 처치해야 한다.
- Royal Guards와 Muffet, 지역 카운터가 모두 충족되면 Genocide 진행이 더 이상 일반적인 방식으로 중단되지 않는 지점에 도달한다.

따라서 Genocide는 사실상 다음과 같은 지역 반복 구조를 가진다.

**지역 진입 → 일반 조우와 특수 적 조건 확인 → 지역별 카운터 소진 → 필수 보스 조건 충족 → 다음 지역 이동**

지역 카운터를 충족하지 않은 채 보스 단계로 진행하거나 필수 특수 적을 살려 보내면 Genocide가 중단될 수 있다.

근거: [Genocide Route](https://undertale.wiki/w/Genocide_Route)

### F5. Genocide의 중단은 단순한 엔딩 변경이 아니라 세계 상태의 변화다.

Genocide 진행 중 다음과 같은 경우 루트가 중단될 수 있다.

- 지역의 필수 처치 카운터를 소진하지 못한 채 보스 단계에 도달한다.
- 필수 보스나 특수 적을 살려 보낸다.
- 지역별 필수 조건을 놓친다.

이탈하면 이후 지역은 Neutral과 유사한 상태로 진행되지만, 이미 지나온 지역의 일부 변화는 남을 수 있다. 배경 음악, NPC 배치, SAVE Point 문구, 조우 방식 등이 달라질 수 있다.

중단된 Genocide를 다시 이어가려면 중단 이전 SAVE를 불러오거나 Reset해야 한다. 이미 지나온 지역의 흔적은 단순히 Neutral로 바뀌었다고 모두 사라지는 것이 아니다.

여기서 중요한 구분은 다음과 같다.

- **Genocide 시도 실패:** 진행이 Neutral로 이탈하는 상태
- **Genocide 완수 후 세계 복원 선택:** 다음 회차에 영향을 남기는 별도 메타 상태

두 상태는 서로 다르다. 중단된 시도와 완수 후 영구 상태 변화를 같은 변수로 묶어 설명하면 부정확하다.

근거: [Genocide Route](https://undertale.wiki/w/Genocide_Route), [Endings](https://undertale.wiki/w/Route)

### F6. Neutral은 단일 엔딩이 아니라 생존 상태와 관계에 따라 세분화되는 엔딩군이다.

Neutral 엔딩의 명칭은 공식 게임 용어가 아니라 위키에서 구분을 위해 사용하는 비공식 명칭이다. 따라서 세 가지 주요 루트와 Neutral 내부의 에필로그 변형을 같은 수준의 개념으로 취급하면 안 된다.

| Neutral 엔딩 분기 | 주요 조건의 개요 | 결말의 중심 |
|---|---|---|
| Toriel Ending Tree | Toriel 생존 | Toriel이 왕위를 되찾고, 세부 조건에 따라 추가 분기 |
| Family Ending | Toriel 생존, Papyrus·Undyne과 관계 형성, 몬스터 처치 없음 | 인물들의 관계 회복과 새로운 공동체 |
| Betrayed Undyne Ending | Toriel·Papyrus·Undyne이 생존하지만 관계 형성 또는 이후 행동 조건이 어긋남 | Undyne과 플레이어 사이의 신뢰 문제 |
| Exiled Queen Ending | Toriel 생존, 일정 수 이상의 처치 또는 주요 인물 처치 | 반발과 반란으로 인한 권력 변화 |
| Undyne Ending | Toriel 사망, Undyne 생존 | Undyne 중심의 강경한 통치 |
| Mettaton Ending | Toriel·Undyne 사망, Mettaton 생존 | Mettaton 중심의 사회 |
| Papyrus Ending | Toriel·Undyne·Mettaton 사망, Papyrus 생존 | Papyrus가 지도자 역할을 맡는 결말 |
| Dog Ending | 주요 지도 인물들이 사망하고 일반 몬스터의 생존 조건이 특정 조합으로 충족됨 | 유머성 특수 결말 |
| Leaderless Ending | 주요 지도 인물들이 사망하고 일반 몬스터 일부도 처치됨 | 지하 세계의 지도력 상실 |
| Alphys Ending | Genocide 진행을 특정 지점에서 중단하거나 Hotland/CORE 조건을 완수하지 못한 경우 등 | Alphys가 남은 몬스터들을 이끄는 결말 |
| Impossible Ending | 정상적인 분기 조건과 맞지 않는 비정상적인 게임 상태 | 일반적인 정상 플레이의 표준 결말이 아님 |

#### Toriel Ending Tree의 하위 분기

- **Family Ending:** Papyrus와 Undyne을 친구로 만들고, 몬스터를 처치하지 않은 경우로 정리된다.
- **Betrayed Undyne Ending:** Papyrus와 Undyne이 살아 있지만 Undyne과의 관계가 기대한 방식으로 완성되지 않았거나, 관계를 맺은 뒤 다시 몬스터를 처치하는 등 조건이 어긋난 경우와 연결된다.
- **Exiled Queen Ending:** 일정 수 이상의 몬스터를 처치했거나 Papyrus 또는 Undyne을 처치한 경우 등과 연결된다.

#### 지도자의 생존에 따른 분기

Toriel이 사망하고 Undyne이 살아 있으면 Undyne Ending으로 이어질 수 있다. Toriel과 Undyne이 사망하고 Mettaton이 생존하면 Mettaton Ending, 주요 지도 인물이 사망하고 Papyrus가 생존하면 Papyrus Ending으로 연결되는 구조가 있다.

#### 특수 분기

- Dog Ending과 Leaderless Ending은 주요 인물과 일반 몬스터의 생존 조합에 따라 갈라지는 특수 엔딩이다.
- Leaderless Ending에는 일반 몬스터를 일부 처치했는지, 전부 처치했는지에 따라 대사 차이가 있다.
- Alphys Ending은 Genocide 조건을 진행하다가 특정 지점에서 이탈한 플레이와 연결되는 Near Genocide 계열의 결과다.
- Neutral에서 만난 적을 모두 처치한 경우에도 Genocide 지역 조건을 완성하지 못했다면 Genocide가 아니라 Neutral의 No Mercy/Leaderless 계열로 분류될 수 있다.

이 구조가 보여주는 것은 Neutral이 단순히 “나쁜 선택을 했으니 나쁜 엔딩”이라는 체계가 아니라는 점이다. 어떤 인물이 살아 있는지, 누구와 관계를 형성했는지, 얼마나 많은 몬스터가 사라졌는지에 따라 지하 세계의 권력 구조와 사회적 결과가 달라진다.

근거: [Neutral Route](https://undertale.wiki/w/Neutral_Route), [Endings](https://undertale.wiki/w/Route)

### F7. RESET은 플레이 기록을 지우는 행위이면서 동시에 서사 장치다.

True Pacifist 완료 후에는 True Reset을 사용할 수 있다. True Reset은 새로운 게임을 시작할 수 있게 하지만, Genocide 완료 후 세계 복원 선택으로 남겨진 상태는 일반적인 True Reset으로도 사라지지 않는다고 정리되어 있다.

| 상태 | 의미 | 이후 영향 |
|---|---|---|
| SAVE / LOAD | 특정 진행 지점 저장 및 복구 | 현재 플레이 진행을 되돌릴 수 있음 |
| 일반 Reset | 기본 진행을 초기화 | 일부 캐릭터의 대사 변화가 남을 수 있음 |
| True Reset | True Pacifist 이후 사용할 수 있는 재시작 | 대부분의 진행 상태를 초기화 |
| Genocide 완수 후 세계 복원 선택 | 세계를 되살리는 선택 | 이후 True Pacifist와 Genocide 엔딩에 변화가 남음 |

Genocide 완수 후 세계 복원 선택은 이후 True Pacifist와 Genocide 결말에 영구적인 차이를 남긴다. 반면 Neutral 엔딩은 같은 방식으로 바뀌지 않는다고 정리되어 있다. 콘솔 버전에서는 해당 변화가 Genocide를 완료한 플레이어 프로필에 적용되는 차이도 있다고 자료는 설명한다.

또한 Neutral 엔딩을 반복하는 경우 Flowey의 대사가 달라지는 등 반복 플레이를 캐릭터가 인식하는 메타적 표현이 존재한다.

근거: [Endings](https://undertale.wiki/w/Route), [Genocide Route](https://undertale.wiki/w/Genocide_Route), [Neutral Route](https://undertale.wiki/w/Neutral_Route)

---

## 4. Scope filter

조사 내용을 RPG 전체의 일반 원리와 비교했을 때 다음과 같이 정리해야 한다.

1. **루트와 엔딩 변형은 구분해야 한다.**  
   Neutral·True Pacifist·Genocide가 세 가지 주요 루트다. Neutral 안에서 갈라지는 Family·Undyne·Mettaton 등의 엔딩은 독립적인 메인 루트가 아니라 결과 변형으로 분류하는 것이 정확하다.

2. **처치 횟수는 단순한 누적 수치가 아니다.**  
   Genocide의 카운터는 지역별로 따로 관리되며, 일부 특수 적은 별도 조건으로 취급된다. 모든 지역을 통틀어 처치 횟수만 계산하면 정확한 루트 판정 구조를 설명할 수 없다.

3. **비폭력 루트는 단순히 전투를 피하는 루트가 아니다.**  
   True Pacifist는 전투·관계·이벤트 진행이 결합된 루트다. 공격을 했다는 사실 하나로 판정하기보다 EXP 획득과 적의 생존 여부를 함께 봐야 한다.

4. **메타 진행은 현재 플레이와 별도로 관리해야 한다.**  
   Genocide 완료 이후 남는 효과는 현재 플레이 도중의 루트 이탈과 다른 종류의 데이터다. 따라서 일반적인 엔딩 분기와 회차 간 영구 상태를 같은 변수로 묶어 설명하면 부정확하다.

---

## 5. Object filter

이제 대상인 Undertale의 실제 시스템에 맞춰 내용을 한 번 더 좁힌다.

| 검토 대상 | 수정·제한한 해석 |
|---|---|
| True Pacifist | 모든 공격을 금지하는 것이 아니라 처치와 EXP 획득을 금지하는 조건으로 설명 |
| Genocide | 단순한 몬스터 총 처치량이 아니라 지역 카운터와 특수 적·보스 조건의 조합으로 설명 |
| Neutral | 독립적인 여러 메인 루트가 아니라 생존·관계 상태에 따른 에필로그 분기로 정리 |
| Genocide 이탈 | 완수 후 영구 상태 변화와 구분 |
| RESET | SAVE/LOAD, 일반 Reset, True Reset을 서로 다른 개념으로 구분 |
| 엔딩 조건 | 공식 명칭이 아닌 위키의 분류 이름을 공식 게임 용어처럼 사용하지 않도록 제한 |

특히 **Neutral No Mercy와 Genocide는 동일한 개념이 아니다.** 플레이어가 만난 적을 모두 처치했더라도 지역별 Genocide 조건을 완성하지 않았다면 별도의 Neutral 변형으로 남을 수 있다.

근거: [Neutral Route](https://undertale.wiki/w/Neutral_Route), [Genocide Route](https://undertale.wiki/w/Genocide_Route)

---

## 6. Conclusions — 최종 분석

### 6-1. 전체 루트 판정은 세 층으로 나눌 수 있다.

**1층 — 기본 루트 판정: 현재 플레이의 행동 기록**

처치·EXP·관계 이벤트·지역별 카운터를 기록한다.

**2층 — 현재 플레이의 결말 분기: 진행 조건의 조합**

Neutral의 경우 인물 생존과 관계에 따라 에필로그가 나뉘고, True Pacifist와 Genocide는 각자의 완료 조건을 요구한다.

**3층 — 회차 간 메타 상태: 이전 엔딩의 영향**

True Reset과 Genocide 완료 후 세계 복원 상태 등은 이후 플레이의 대사와 결말에 영향을 줄 수 있다.

위 구조는 조사된 규칙을 이해하기 위해 재구성한 분석 모델이며, 게임 내부의 실제 변수 구조를 직접 확인한 것은 아니다.

### 6-2. True Pacifist의 핵심은 관계의 축적이다.

True Pacifist는 특정 보스를 처치하지 않는 방식으로 끝나지 않는다.

Papyrus와 관계를 쌓고, Undyne을 돕고, Alphys에게 편지를 전달하며, True Lab의 비밀을 발견하는 연쇄 과정이 필요하다. 전투에서 비폭력적인 태도를 유지하는 것은 그 과정의 출발점일 뿐이다.

따라서 True Pacifist는 **행동의 일관성 + 관계 형성 + 숨겨진 진실의 발견**이라는 세 가지 축으로 구성되어 있다고 해석할 수 있다.

### 6-3. Genocide의 핵심은 플레이어가 세계의 변화를 직접 관찰하게 만드는 것이다.

Genocide는 숫자를 채우는 것만으로 구성되지 않는다. 지역의 배경 음악과 NPC 배치, 조우 방식, 보스 등장 방식이 함께 달라진다.

이러한 변화는 플레이어가 별도의 설명을 듣지 않아도 세계의 상태가 달라졌음을 알아차리게 한다. 즉, 루트 판정이 UI에만 머무르지 않고 탐험 환경 전체에 반영된다.

### 6-4. Neutral은 결과의 다양성을 확보하는 역할을 한다.

Neutral은 단순히 Pacifist와 Genocide 사이에 있는 중간 단계가 아니다.

주요 인물의 생존 여부와 관계 형성에 따라 지하 세계의 지도자, 사회 분위기, 인물의 미래가 달라진다. 그러므로 모든 플레이의 결과를 완벽한 선과 악으로 나누지 않고, 중간 선택에도 의미 있는 후속 결과를 부여한다.

### 6-5. 가장 중요한 구조적 특징은 '선택 → 세계 변화 → 인물 반응 → 다음 플레이 변화'다.

Undertale에서 루트는 엔딩 직전에 결정되는 단순한 선택지가 아니다.

플레이어의 행동은 지역 단위로 기록되고, 해당 기록이 인물의 반응이나 다음 구역의 상태로 반영된다. 이후 엔딩은 그 기록을 종합해 결정된다. 일부 결과는 다음 회차에도 남는다.

이것이 D 조사에서 확인한 가장 중요한 설계 특징이다.

---

## 7. 언더페일 적용 방향 — 전부 미승인 제안

아래 내용은 Undertale의 구조를 학교 배경 게임에 응용할 수 있는 가능성이지, 현재 언더페일의 정사나 확정 기획이 아니다.

### 제안 A — 학교 구역별 판정 시스템

Genocide의 지역별 카운터 구조를 학교에 맞게 변환할 수 있다. 예를 들어 각 교실·복도·부서마다 별도의 갈등 해결 조건을 두는 방식이다. 단, 단순히 숫자를 채우는 구조보다는 각 구역의 특수 사건과 인물 관계를 결합하는 편이 자연스럽다.

### 제안 B — 우호 루트의 관계 연쇄

Papyrus·Undyne·Alphys의 관계 이벤트처럼, 특정 인물과의 관계가 다음 인물의 이벤트를 열어주는 구조를 고려할 수 있다. 한 캐릭터와의 관계가 단순한 호감도 수치가 아니라 다른 캐릭터와의 신뢰 형성에도 영향을 주는 방식이다.

### 제안 C — Neutral 엔딩의 사회적 결과

학교의 권력 구조가 학생회, 교사, 학급 대표 등의 생존·신뢰·협력 상태에 따라 달라지는 결말을 생각할 수 있다. 특히 누가 마지막에 승리했는지보다, 그 이후 학교가 어떤 상태로 남았는지가 엔딩의 핵심이 될 수 있다.

### 제안 D — 회차 간 메타 상태

한 번의 플레이에서 끝나지 않는 숨겨진 상태를 활용할 수 있다. 다만 이전 플레이의 선택이 다음 회차에 영향을 주는 이유와 범위를 서사적으로 설득력 있게 만들어야 한다.

### 제안 E — 루트 이탈의 시각적 표현

Undertale의 배경 음악·NPC·조우 변화처럼 언더페일에서도 특정 루트의 조건을 놓쳤을 때 게임 세계의 분위기가 바뀌도록 설계할 수 있다. 이는 플레이어에게 별도의 경고창을 띄우지 않고도 결과를 전달하는 방법이다.

**정사 여부:** 위 제안 A~E는 모두 미승인 제안이다. 사용자가 확정하기 전까지 언더페일의 정사나 구현 요구사항으로 취급하지 않는다.

---

## 8. Next steps / Risks

| 미확인 사항 | 현재 한계 | 다음 검증 방법 |
|---|---|---|
| 정확한 내부 판정 변수 | 게임 코드를 직접 확인하지 못함 | 원본 데이터 또는 직접 플레이 결과 대조 |
| 플랫폼 간 차이 | PC와 콘솔의 세부 차이를 전부 검증하지 못함 | 플랫폼별 조건 비교 |
| Neutral 분기 우선순위 | 위키의 조건표에 의존 | 동일 조건 조합으로 실제 엔딩 판정 확인 |
| Genocide 지역별 예외 | 일부 특수 적 조건이 복잡함 | 지역별 실제 조우 및 SAVE 상태 대조 |
| 회차 간 영구 상태 | 내부 저장 구조를 직접 조사하지 못함 | SAVE 데이터와 엔딩 이후 변화 비교 |

### 조사 진행 체크리스트

- [x] 1. Canon — 출처 우선순위 작성
- [x] 2. Charter — 목표·범위·질문 설정
- [x] 3. Type file — Descriptive 절차 확인 및 적용
- [x] 4. Findings ledger — 근거별 조사 기록
- [x] 5. Scope filter — RPG 전체 구조와 비교
- [x] 6. Object filter — Undertale의 실제 분기 구조에 맞게 해석 제한
- [x] 7. Conclusions — 결론과 근거 연결
- [ ] 원본 게임의 내부 판정 규칙 직접 검증

**조사 상태:** 문헌 기반 조사 완료. 원본 게임의 내부 판정 코드 및 모든 조건 조합의 직접 검증은 미완료다.

### 핵심 결론

Undertale의 루트 시스템은 단순한 선악 선택지가 아니다. 플레이어의 행동을 지역별·인물별·회차별로 기록하고, 그 기록을 세계의 변화와 엔딩에 연결하는 구조다.

A가 전체 이야기의 진행을, B가 공간과 탐험의 흐름을, C가 전투와 행동의 규칙을 조사했다면, D는 **그 행동이 게임 전체의 결과를 어떻게 결정하는지**를 설명하는 단계다.

---

## 참고 자료

아래 자료는 조사 과정에서 확인한 Undertale Wiki의 공개 문서다. 위키는 세부 조건을 정리하는 2차 자료이므로 공식 개발 문서와 구분한다.

1. [The Undertale Wiki — Endings / Route](https://undertale.wiki/w/Route)
2. [The Undertale Wiki — Genocide Route](https://undertale.wiki/w/Genocide_Route)
3. [The Undertale Wiki — Neutral Route](https://undertale.wiki/w/Neutral_Route)
4. [The Undertale Wiki — True Pacifist Route](https://undertale.wiki/w/Pacifist)
5. [The Undertale Wiki — True Lab](https://undertale.wiki/w/True_Lab)
6. [Undertale 공식 홈페이지](https://undertale.com/)

**자료 활용 원칙:** 위키의 페이지 명칭 및 분류를 공식 게임 내 용어로 단정하지 않는다. 원본 게임에서 직접 확인하지 못한 세부 수치는 문헌 기반 조사 결과로 취급한다.
