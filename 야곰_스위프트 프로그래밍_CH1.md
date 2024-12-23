# 1장. 스위프트

## CHAPTER 1. 스위프트

**<객체지향 프로그래밍 패러다임>**

객체지향 프로그래밍은 컴퓨터 프로그램을 명령어의 목록으로 보는 기존의 명령형 프로그래밍 패러다임의
시각에서 벗어나 여러 개의 독립된 단위인 객체의 모임으로 파악하고자 하는 시각.
각각의 객체는 서로 메시지를 주고 받고 데이터를 처리한다

-장점: 유연하고 쉽게 변경할 수 있도록 작성할 수 있어 대규모 소프트웨어 개발에 많이 사용한다.
         소프트웨어 개발과 유지보수를 간편하게 할 수 있으며, 직관적으로 코드를 분석할 수 있다 

소프트웨어 공학의 관점에서 소프트웨어의 질 향상은 **강한 응집력과 약한 결합력**을 지향한다 
-객체지향 프로그래밍의 응집력 강화 : 클래스에 하나의 문제를 해결하기 위한 데이터와 메서드를 모아놓은 방식
-객체지향 프로그래밍의 결합력 약화 : 각 클래스는 독립적이 되도록 디자인

-클래스 : 같은 종류(또는 문제 해결을 위한)의 집단에 속하는 속성과 행위를 정의한 것. 객체 프로그램의 기본 사용자 정의 데이터 타입으로, 다른 클래스 또는 외부 요소와 독립적으로 디자인되어야 한다 

-객체 :  클래스의 인스턴스(실제로 메모리에 할당되어 동작하는 모양을 갖춘 것) 객체는 자신의 고유의 속성이 있으며 클래스에서 정의한 행위를 할 수 있다. 스위프트는 객체 보다 클래스의 인스턴스라는 표현을 사용한다 

→ 객체 == 클래스의 인스턴스 / 객체 ≠ 인스턴스
인스턴스는 구조체의 인스턴스도 있고, 열거형의 인스턴스도 있을 수 있기 때문에 객체는 인스턴스 중에도 클래스의 인스턴스만 가리키는 말로 좀 더 한정적인 의미

-메서드 또는 메시지 : 객체가 클래스에 정의된 행위를 실질적으로 하는 함수. 메서드를 통해 객체에 명령을 전달할 수 있다 

스위프트뿐만 아니라 객체지향 프로그래밍 패러다임을 차용한 언어는 필수로 명령형 프로그래밍 패러다임을 사용
→ 프로퍼티, 변수 등에 해당하는 메모리 값의 변화(상태변화)가 있기 때문

**<함수형 프로그래밍 패러다임>**

프로그램이 상태의 변화 없이 데이터 처리를 수학적 함수 계산으로 취급하고자 하는 패러다임으로, 대규모 병렬처리가 굉장히 쉽다는 장점이 있다 

객체지향 프로그래밍 패러다임이나 명령형 프로그래밍 패러다임에서는 프로그램에서 값이나 상태의 변화를 중요하게 여기지만, 함수형 프로그래밍 패러다임은 함수 자체의 응용을 중요하게 여긴다 

객체지향 프로그래밍은 절차지향 프로그래밍 패러다임이 포함되어 있다 

→ 함수가 전달받은 전달인자(Argument) 외에도 포인터, 레퍼런스 값 등 객체의 상태 값(프로퍼티 값) 또는 메모리 참조 값 등이 변경될 수 있으며 함수 내부의 처리에도 영향을 미칠 수 있다 

<aside>
💡

~p.46 | 스위프트를 다룬지 꽤 됐지만 요즘들어 정말 부족한 채로 무모하게 개발판에 뛰어들었구나싶다. 

그래서 시작한 기본 다지기 프로젝트.. 대충 알고 쓸 줄 아는 내용도 깊이 있게 알기 위해..! 습관처럼 조금씩이라도 공부하고 기록하기로 마음먹었다.. 파이팅~! 

1. 아직은 함수형 프로그래밍 패러다임에 대한 개념이 명확히 와닿진 않는다 
</aside>