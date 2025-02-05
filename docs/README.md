# 미션 - 숫자 야구
### 기능 목록

#### 공통
- 컴퓨터가 출력하는 모든 안내 문구는 상수로 출력한다.
- 컴퓨터는 서로 다른 임의의 수를 고를 때 Randoms API를 활용한다
- 컴퓨터는 값을 사용자로부터 입력받을 때 Console API 의 readLine을 활용하여 값을 입력받는다

#### 환경 구성
- [x] 의존성 주입을 위한 Assembler 클래스 생성
- [x] 각 레이어별 인터페이스를 만든다
#### 게임 시작
- [x] 게임을 시작시키면 컴퓨터는 "숫자 야구 게임을 시작합니다." 라는 게임 시작 문구를 출력한다
- [x] 컴퓨터는 서로 다른 임의의 수 3개를 생성한다
- [x] 랜덤하게 고른 수들을 저장한다


#### 게임 중
- [x] 사용자에게 숫자를 입력받는 기능
    - 컴퓨터는 "숫자를 입력해주세요 : " 라는 안내 문구를 출력한다
    - 사용자는 1부터 9 까지의 수 중에서 3개를 입력한다
    - 컴퓨터는 Console API 의 readLine을 활용하여 값을 입력받는다

- [x] 사용자에게 입력받은 수와 컴퓨터가 고른 수를 비교한다
    - 입력한 수에 대한 결과를 "볼", "스트라이크", "낫싱"으로 출력한다

- [x] 3개의 숫자를 모두 맞힐 경우 게임을 종료한다
  - 모두 맞추지 못 했을 경우 맞출 때까지 반복한다

#### 게임 끝
- [x] 컴퓨터는 게임 재개 의사를 사용자에게 물어본다
  - "게임을 새로 시작하려면 1, 종료하려면 2를 입력하세요" 라는 안내 문구를 출력한다
  - 컴퓨터는 사용자로부터 1를 입력받을 시 게임을 다시 시작한다
  - 컴퓨터는 사용자로부터 2를 입력받을 시 게임을 완전히 종료한다

### 예외사항
사용자가 잘못된 값을 입력할 경우 IllegalArgumentException을 발생시킨 후 애플리케이션을 종료시킨다
