# kotlin-blackjack

# Step1- KotlinDSL 
필요 도메인 
- 사람 ( Person )
  - 이름 ( Name )
  - 회사 ( Company )
  - 스킬 ( Skill )

- 회사 ( Company )
  - 이름 ( Name )

- 스킬 ( Skill )
  - 설명 ( introduce )

- 언어 ( Language )
    - 이름 ( Name )
    - 레벨 ( Level )

## 고려했던 상황 
- 언어 레벨의 경우 1~5까지만 선택할 수 있다. 
- 각 도메인들은 빈값 ("")이 들어올 경우, 예외가 발생한다.

# Step2 - BlackJack 
필요 도메인
- 플레이어 ( Player )
  - 플레이어는 이름과 카드들을 가지고있을 수 있다.
  - 플레이어는 본인이 가지고있는 카드들의 합을 구할 수 있다.
  - 플레이어는 본인이 가지고있는 카드들의 합을 토대로 블랙잭 게임을 이어갈지 결정할 수 있다.

- 카드 ( Card )
  - 카드는 숫자, 무늬 (클로버, 다이아 ...)를 가질 수 있다. 
  - 카드가 에이스인지 아닌지를 판별할 수 있다.

- 카드 덱 ( Card Deck )
  - 카드덱은 카드를 뽑을 수 있다. 

- 유저가 가지고있는 카드들 ( Cards )
  - Cards는 일급컬렉션이다.
  - 카드들의 합 계산이 가능하다. 만약, 21이 넘는다면 에이스는 1로 게산된다.

그 외
- Dto 
  - View까지 필요로 전달되는 데이터는 Dto로 구성한다.

- View
  - View는 Dto를 통해 데이터를 전달받는다.
  - View는 데이터를 토대로 화면에 출력한다.