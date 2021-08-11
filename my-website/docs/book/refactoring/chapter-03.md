# 3장 - 코드에서 나는 악취

Code Smell is a driver for refactoring

리펙토링의 목적은 가독성과 유지 보수성을 향상 시키기 위한 것


## 3.1 기이한 이름 (Mysterious Name)

Sign and symptoms
- 코드가 무슨 동작을 하는지 이해하기 위해, Text를 이리저리 맞춰보아야 하는 경우

Treatment
- 함수 선언 바꾸기
- 변수 이름 바꾸기
- 필드 이름 바꾸기

## 3.2 중복 코드 (Duplicated Code)

Sign and symptoms
- 동일한 코드 구조가 두군데 이상 있을때
  
Treatment
- 한 클래스의 두 메서드가 똑같은 코드를 사용할 때는 함수 추출하기
- 비슷한 코드가 여러 군데 존재한다면, 문장 슬라이드로 모은 뒤 함수 추출하기
- 서브 클래스에 중복 코드가 있으면 부모 클래스로 메서드 올리기

## 3.3 긴 함수 (Long Function)

Sign and symptoms
- 함수의 코드 라인이 긴 경우 
- 일반적으로 10 라인이 넘어가면 의문을 가져보아야 한다.

Treatment
- 함수를 짧게 만드는 작업의 대부분은 함수 추출하기
- 함수 추출 시 로컬 변수가 많으면 매개 변수가 많아진다 이때는 임시 변수를 질의 함수로 바꾸기, 매개변수 객체 만들기와 객체 통째로 넘기기로 매개 변수의 수를 줄일 수 있다.
- 함수를 명령으로 바꾸기
- 조건문이나 반복문은 function 으로 분리시키기 좋은 후보다.
  - 조건문 분해하기
  - switch/case 에서 함수 추출하기
  - 반복문 쪼개기

## 3.4 긴 매개변수 목록 (Long Parameter List)

Sign and symptoms

Treatment

## 3.5 전역 데이터 (Global Data)

Sign and symptoms

Treatment

## 3.6 가변 데이터 (Mutable Data)

Sign and symptoms

Treatment

## 3.7 뒤엉킨 변경 (Divergent Change)

Sign and symptoms

Treatment

## 3.8 산탄총 수술 (Shotgun Surgery)
## 3.9 기능 편애 (Feature Envy)
## 3.10 데이터 뭉치 (Data Clump)
## 3.11 기본형 집착 (Primitive Obsession)
## 3.12 반복되는 switch문 (Repeated Switches)
## 3.13 반복문 (Loops)
## 3.14 성의 없는 요소 (Lazy Element)
## 3.15 추측성 일반화 (Speculative Generality)
## 3.16 임시 필드 (Temporary Field)
## 3.17 메시지 체인 (Message Chains)
## 3.18 중개자 (Middle Man)
## 3.19 내부자 거래 (Insider Trading)
## 3.20 거대한 클래스 (Large Class)
## 3.21 서로 다른 인터페이스의 대안 클래스들 (Alternative Classes with Different Interfaces)
## 3.22 데이터 클래스 (Data Class)
## 3.23 상속 포기 (Refused Bequest)
## 3.24 주석 (Comments)
