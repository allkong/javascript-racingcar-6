# 🏎 구현할 기능 목록

## 사용자 입력
- [ ] 경주할 자동차 이름 입력
  - 자동차 이름은 띄어쓰기 없이 쉼표로 구분
    - ex) pobi,woni,jun
  - 각 자동차 이름은 5자 이하로 허용
- [ ] 시도할 횟수 입력
- [ ] 사용자 입력 유효성 검사

## 무작위 값 구하기
- [ ] 0에서 9까지의 정수 중 한 개의 정수를 선택하여 무작위 값 구하기
  - [`@woowacourse/mission-utils`](https://github.com/woowacourse-projects/javascript-mission-utils) 라이브러리의 `Random.pickNumberInRange()` 활용

## 자동차 전진/멈추기
- [ ] 구한 무작위 값이 4 이상이면 전진하기
- [ ] 구한 무작위 값이 3 이하면 멈추기

## 각 차수별 실행 결과 출력
- [ ] 사용자가 입력한 횟수만큼 자동차 전진/멈추기를 진행하는 각 차수마다 출력
- [ ] 사용자가 자동차 이름을 입력한 순서대로 각 자동차 이름과 전진한 정도를 출력
- 한 번 전진을 '-'로 나타냄
- ex)
  ```
  pobi : --
  woni : ----
  jun : ---
  ```

## 우승자 출력
- [ ] 가장 전진을 많이 한 자동차를 우승자로 선정
  - 우승자는 1명 이상일 수 있음
- [ ] 단독 우승일 경우 1명의 우승자 출력
  - ex) 최종 우승자 : pobi
- [ ] 공동 우승일 경우 쉼표와 띄어쓰기로 여러 명의 공동 우승자를 구분하여 출력
  - ex) 최종 우승자 : pobi, jun

<br>

# 🚨 예외 처리
- 사용자가 잘못된 값을 입력하면 throw문으로 예외 발생시켜 애플리케이션 종료
- '[ERROR]'로 시작하는 에러 문구 출력

### 유효성 검사
- 자동차 이름
  - [ ] 자동차 이름이 6자 이상일 경우 예외 처리
  - [ ] 자동차 이름이 중복일 경우 예외 처리
  - [ ] 공백이 포함되어 있을 경우 예외 처리
  - [ ] 입력을 안했을 경우 예외 처리
- 시도할 횟수
  - [ ] 숫자가 아닐 경우 예외 처리
  - [ ] 정수가 아닐 경우 예외 처리
  - [ ] 1 미만의 숫자일 경우 예외 처리
  - [ ] 입력을 안했을 경우 예외 처리