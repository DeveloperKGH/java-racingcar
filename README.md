# 자동차 경주 - 단위테스트 

---

> NEXTSTEP TDD, 클린 코드 with Java 16기, 자동차 경주 관련 미션을 구현한 저장소입니다.

# 목차

- [1단계 - 학습 테스트 실습](#1단계---학습-테스트-실습-요구사항)
- [2단계 - 문자열 덧셈 계산기](#2단계---문자열-덧셈-계산기-요구사항)
- [3단계 - 자동차 경주](#3단계---자동차-경주-요구사항)
- [4단계 - 자동차 경주(우승자)](#4단계---자동차-경주--우승자--요구사항)

## 1단계 - 학습 테스트 실습 요구사항

---
__String 클래스에 대한 학습 테스트__
- [x] split() 했을 때 1과 2로 잘 분리되는지 확인
- [x] split() 했을 때 1만을 포함하는 배열이 반환되는지 확인
- [x] substring() 했을 때 1,2 반환되는지 확인
- [x] charAt() 했을 때 abc 특정 위치의 문자가 반환되는지 확인
- [x] charAt() 했을 때 abc 특정 위치 값을 벗어나면 StringIndexOutOfBoundsException 이 발생되는지 확인

<br>

__Set Collection 에 대한 학습 테스트__
- [x] size() 했을 때 Set 의 크기인 3이 반환되는지 확인
- [x] contains() 했을 때 1, 2, 3의 값이 존재하는지를 확인
- [x] contains() 했을 때 1, 2, 3의 값은 존재하고, 4, 5의 값은 존재하지 않음을 확인

---

<br>

## 2단계 - 문자열 덧셈 계산기 요구사항

---

- [x] 빈 문자열을 입력하는 경우 0을 반환 (ex : "" = 0)
- [x] null 값을 입력하는 경우 0을 반환 (ex : null = 0)
- [x] 숫자 하나만 입력하는 경우 해당 숫자를 반환 (ex : "1" = 1)
- [x] 두개 이상의 숫자를 콤마(",") 구분자를 가진 채 입력하는 경우 각 숫자들의 합을 반환 (ex : "1,2" = 3)
- [x] 구분자는 콤마(",") 외에 콜론(":")도 사용가능 (ex : “1,2:3” = 6)
- [x] “//”와 “\n” 사이에 위치하는 문자를 커스텀 구분자로 지정할 수 있음 (ex : “//;\n1;2;3” = 6)
- [x] 음수를 입력하는 경우 RuntimeException 예외가 발생 (ex : “-1:2:3”)
- [x] 숫자 이외의 값을 입력하는 경우 RuntimeException 예외가 발생 (ex : “a:2:3”)

---

<br>

## 3단계 - 자동차 경주 요구사항

---
- [x] 차고 객체가 생성되는지 확인
- [x] 자동차 객체가 생성되는지 확인
- [x] 입력한 수만큼 자동차 객체가 생성되는지 확인
- [x] 생성한 random 값이 0 ~ 9 사이의 숫자인지 확인
- [x] 자동차 전진 이동 테스트
- [x] 자동차 전진 조건 테스트
- [x] 자동차 멈춤 조건 테스트
- [x] 레이싱 자동차 객체가 생성되는지 확인
- [x] 레이싱 객체가 생성되는지 확인
- [x] 레이스가 끝날때 남은 매치 카운트가 감소하는지 확인 
- [x] 자동차 움직임 조건 범위를 벗어나는 값을 입력하는 경우 RuntimeException 예외가 발생되는지 확인
---

<br>

## 4단계 - 자동차 경주(우승자) 요구사항

---
- [x] 자동차 객체 생성시 이름을 부여할 수 있는지 확인
- [x] 자동차 이름에 유효하지 않은 값이 입력된 경우 IllegalArgumentException 예외가 발생하는지 확인 (ex: null or "") 
- [x] 자동차 이름이 5자를 초과하는 경우 IllegalArgumentException 예외가 발생하는지 확인
- [x] 자동차 이름이 5자 이하인 경우 예외가 발생하지 않는지 확인
- [x] 입력된 이름 문자열을 쉼표(",") 를 기준으로 나누어 반환되는지 확인
- [x] 입력된 이름 문자열에 쉼표(",") 구분자가 없는경우 문자열 그대로 반환되는지 확인
- [x] 리스트 형태의 이름 문자열들을 쉼표(",") 를 기준으로 합쳐 하나의 문자열로 반환하는지 확인
- [x] 리스트의 원소가 하나인 이름 문자열을 쉼표(",") 를 기준으로 합치면 입력 문자열 그대로 반환하는지 확인
- [ ] 자동차 경주 게임을 완료한 후 우승자 이름이 하나 이상 반환되는지 확인
- [ ] 전진하는 자동차를 출력할 때 자동차 이름을 같이 출력
---
