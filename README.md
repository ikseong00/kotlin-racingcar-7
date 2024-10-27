# kotlin-racingcar-precourse

# 자동차 경주

## 기능 목록

- [x] 자동차 이름 입력
- [x] 시도할 횟수 입력
- [x] 각 자동차들이 전진할지 멈출지 결정
- [x] 각 자동차들의 전진 여부에 따라 출력
- [x] 최종 우승자 출력

## 세부 기능 목록

### Validator

`Controller` 가 `InputView` 를 통해서 받은 입력들에 대한 유효성을 검증한다.

- [x] 입력값이 유효한 지 검증한다.

### RacingCar

`자동차 이름`, `전진 횟수`를 가지고 있다.

- [x] 전진할지 멈출지 결정한다.
- [x] `toString()` 출력 형식을 정의한다.

### RacingCarController

입력, 출력을 컨트롤하고, 게임을 진행한다.

- [x] 입력 값을 저장한다.
- [x] 시도할 횟수 만큼 게임을 플레이한다.
- [x] 각 시도마다 자동차들을 전진 혹은 정지시키고 결과를 출력한다.
- [x] 최종 우승자를 출력한다.

### InputView

`Console.readLine()`을 통해 입력을 받는다.

- [x] 자동차 이름들을 입력받는다.
- [x] 시도할 횟수를 입력받는다.

### OutputView

각각 `carList`, `winners` 리스트를 받아서 출력한다.

- [x] 각 차수별 현황을 출력한다.
- [x] 최종 우승자를 출력한다.

## 요구 사항

- 자동차 이름은 쉼표`,`를 기준으로 구분하며 이름은 5자 이하만 가능하다.
- 0~9 사이 무작위 값을 구 한 후, 값이 4 이상이면 전진한다. 아니면 정지한다.
- 잘못된 값을 입력했을 경우 `IllegalArgumentException`을 발생시킨다.
- intent depth 가 3을 넘지 않도록 구현한다.

## 개인적 목표

- [x] 코틀린 문법들을 사용해 코드를 간결하게 짜기
- [x] MVC 패턴 적용하기
- [x] 입,출력메시지를 상수, 변수화 하기
- [x] 예외 케이스 다양하게 생각하기
- [x] 테스트 코드 다양하게 작성하기

## 유효성 검증

- [x] 자동차 이름 입력 시 마지막 문자는 쉼표(,) 가 아니어야 한다.
- [x] 자동차 이름은 빈 문자열이 아니어야 한다.
- [x] 자동차 이름은 쉼표로 구분되어야 한다.
- [x] 자동차 이름은 1자 이상 5자 이하만 가능하다.
- [x] 시도 횟수는 0 혹은 양의 정수이어야 한다.
- [x] 시도 횟수는 빈 문자열이 아니어야 한다.
- [x] 시도 횟수는 Int.MAX_VALUE 이하이어야 한다.