# java-ladder 기능 요구사항

## 입력
- [x] 참여할 사람 이름을 입력받는다.
  - [x] 이름은 쉼표(,)로 구분한다.
  - [x] 이름의 앞뒤 공백은 제거한다. (ex. "aa" == " aa" )
- [x] 최대 사다리 높이를 입력받는다.
  - [x] 자연수여야한다.
- [x] 실행 결과를 입력받는다.
  - [x] 결과는 쉼표(,)로 구분한다.
  - [x] 결과의 앞뒤 공백은 제거한다.
- [ ] 결과를 보고 싶은 사람을 입력받는다.
  - [ ] 참여자 목록에 있는 사람이어야 한다.
  - [ ] `all`을 입력하면 전체 참여자의 실행 결과를 출력한다.
    - [ ] 해당 경우 결과를 출력하고 프로그램을 종료한다.
  - [ ] `all`을 입력할 때까지 반복하여 입력받는다.

## 출력
- [x] 이름을 출력한다.
- [x] 사다리를 출력한다.
- [ ] 결과를 출력한다.
  - [ ] 입력 받은 `결과를 보고 싶은 사람`의 결과만 출력한다.

## 참여자들 (Players)
- [x] 참여자 이름 목록을 통해 참여자들을 생성한다.
  - [x] 이름은 중복될 수 없다.
  - [x] 이름은 두명 이상이여야한다.
- [ ] 현재 참여자들의 높이를 가지고 있다. 

## 참여자 (Player)
- [x] 이름(Name)을 가지고 있다.
- [ ] 몇 번째 라인에 서있는 지를 확인하기 위한 위치를 가지고 있다.
- [ ] `Line`의 연결 여부에 따라 위치를 변경한다.

## 이름 (Name)
- [x] 이름을 의미하는 문자열을 가지고 있다.
  - [x] 이름은 최대 5글자까지 가능하다.

## 사다리 (Ladder)
- [x] 최대 사다리 높이만큼 가로줄(Line)을 가지고 있다.

## 가로줄 (Line)
- [x] 가로줄 연결 여부는 생성자에서 정해진다.
- [x] 사다리가 연결되었는지 여부를 가지고 있다.
  - [x] 연속으로 사다리가 연결되면 안된다.

## 전체 실행 결과(Results)
- [x] 실행 결과 목록을 통해 전체 실행 결과를 생성한다.
  - [x] 실행 결과의 수는 참가자의 수와 일치해야 한다.

## 실행 결과(Result)
- [x] 결과를 의미하는 문자열을 가지고 있다.
  - [x] 결과는 최대 5글자까지 입력할 수 있다.

## 실행 결과 프롬프트
```
참여할 사람 이름을 입력하세요. (이름은 쉼표(,)로 구분하세요)
pobi,honux,crong,jk

실행 결과를 입력하세요. (결과는 쉼표(,)로 구분하세요)
꽝,5000,꽝,3000

최대 사다리 높이는 몇 개인가요?
5

사다리 결과

pobi  honux crong   jk
    |-----|     |-----|
    |     |-----|     |
    |-----|     |     |
    |     |-----|     |
    |-----|     |-----|
꽝    5000  꽝    3000

결과를 보고 싶은 사람은?
pobi

실행 결과
꽝

결과를 보고 싶은 사람은?
all

실행 결과
pobi : 꽝
honux : 3000
crong : 꽝
jk : 5000

```
<br>
<hr>

## 우아한테크코스 코드리뷰

- [온라인 코드 리뷰 과정](https://github.com/woowacourse/woowacourse-docs/blob/master/maincourse/README.md)
