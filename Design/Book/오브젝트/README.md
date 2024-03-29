# 오브젝트

- 조영호 님의 서적 [오브젝트](https://www.aladin.co.kr/shop/wproduct.aspx?ItemId=193681076) 정리

---

## Chapter 01. 객체, 설계

### <a href="Chapter 01. 객체, 설계/1.1 티켓 판매 애플리케이션 구현하기.md" target="_blank">1.1 티켓 판매 애플리케이션 구현하기</a>
1) 요구사항 분석
2) 구현 결과물

### <a href="Chapter 01. 객체, 설계/1.2 무엇이 문제인가.md" target="_blank">1.2 무엇이 문제인가</a>
1) 수동적인 객체 → 읽기 어려운 코드, 예상을 벗어나는 코드
2) 불필요한 의존성 → 높은 결합도 → 변경에 취약한 코드
3) 불필요한 의존성을 최소하하여 결합도를 낮춰라.

### <a href="Chapter 01. 객체, 설계/1.3 설계 개선하기.md" target="_blank">1.3 설계 개선하기</a>
1) 자율성을 높이자
2) 무엇이 개선됐는가
3) 어떻게 한 것인가
4) 캡슐화, 응집도
5) 절차지향과 객체지향
6) 책임의 이동
7) 더 개선할 수 있다 -> 트레이드 오프
8) 그래, 거짓말이다! -> 의인화, 모든 객체의 자율성

### <a href="Chapter 01. 객체, 설계/1.4 객체지향 설계.md" target="_blank">1.4 객체지향 설계</a>
1) 좋은 설계 : 기능 요구사항을 만족하면서, 변경에 유연하게 대응할 수 있는 설계
2) 훌륭한 객체지향 설계 : 협력하는 객체 사이의 의존성을 적절히 조절하는, 변경에 용이한 설계

---

## Chapter 02. 객체지향 프로그래밍

### <a href="Chapter 02. 객체지향 프로그래밍/2.1 영화 예매 시스템.md" target="_blank">2.1 영화 예매 시스템</a>
1) 요구사항 분석

### <a href="Chapter 02. 객체지향 프로그래밍/2.2 객체지향 프로그래밍을 향해.md" target="_blank">2.2 객체지향 프로그래밍을 향해</a>
1) 협력, 객체, 클래스
2) 도메인 주도 개발 : 도메인의 구조를 따르는 프로그램 구조
3) 클래스를 구현하는 법 : 캡슐화/접근제어를 통한 퍼블릭 인터페이스/구현 분리
4) 밸류 타입 : 도메인의 의미를 가진 객체 타입을 정의
5) 협력, 메시지, 메서드

### <a href="Chapter 02. 객체지향 프로그래밍/2.3 할인 요금 구하기.md" target="_blank">2.3 할인 요금 구하기</a>
1) 할인 요금 계산을 위한 협력 시작하기 : '추상화된 것'에 메시지 전송
2) 할인 정책과 할인 조건 : 추상화를 구현하는 두 가지 방법들
3) 할인 정책 구성하기 : 생성자를 통한 제약

### <a href="Chapter 02. 객체지향 프로그래밍/2.4 상속과 다형성.md" target="_blank">2.4 상속과 다형성</a>
1) 컴파일 시간 의존성과 런타임 의존성
2) 상속 : 코드의 재사용, 차이에 의한 프로그래밍
3) 상속과 인터페이스 : 부모 클래스를 자식 클래스로 대체 가능
4) 다형성 : 동일한 메시지를 수신했을 때, 객체의 타입에 따라 각각 다르게 응답할 수 있는 능력
5) 순수 인터페이스 상속을 통한 다형성 구현 : java에서의 '인터페이스'

### <a href="Chapter 02. 객체지향 프로그래밍/2.5 추상화와 다형성.md" target="_blank">2.5 추상화와 다형성</a>
1) 추상화의 장점 1: 도메인의 주요 개념, 정책을 높은 수준에서 간단하게 표현할 수 있다.
2) 추상화의 장점 2: 유연한 설계
3) 추상 클래스와 트레이드 오프
4) 코드를 재사용하는 두 가지 방법 : 상속, 합성
5) 상속을 통한 코드 재사용
6) 합성을 통한 코드 재사용

### 2장 - 마치며
- 프로그래밍 관점에서 클래스, 상속은 중요하지만 프로그래밍 관점에 치우쳐서 객체지향을 바라볼 경우 객체지향의 본질을 놓치기 쉽다.
- 객체지향은 객체를 지향하는 것이고, 객체지향 패러다임의 중심에는 객체가 위치한다. 객체지향에서 가장 중요한 것은 애플리케이션의 기능을
구현하기 위해 협력에 참여하는 객체들 사이의 상호작용이다.
- 객체지향 설계의 핵심은 적절한 협력을 식별하고, 협력에 필요한 역할을 정의한 후에 역할을 수행할 수 있는 적절한 객체에게 적절한 책임을
할당하는 것이다.

---

## Chapter 03. 역할, 책임, 협력

### Intro
- 객체지향 설계의 본질은 협력하는 객체들의 공동체를 창조하는 것
- 객체지향 설계의 핵심 : 협력을 구성하기 위해 적절한 객체를 찾고, 적절한 책임을 할당하는 과정
- 애플리케이션의 기능을 구현하기 위해 어떤 협력이 필요한 지, 협력을 위해 어떤 역할과 책임이 필요한지, 구분하지 않은 채
구현에 초점을 두면 변경하기 어렵고 유연하지 못 한 코드를 낳는 원인이 됨.

### <a href="Chapter 03. 역할, 책임, 협력/3.1 협력.md" target="_blank">3.1 협력</a>
1) 영화 예매 시스템 돌아보기 : 협력, 책임, 역할
2) 협력
3) 협력이 설계를 위한 문맥을 결정한다.

### <a href="Chapter 03. 역할, 책임, 협력/3.2 책임.md" target="_blank">3.2 책임</a>
1) 책임이란
2) 책임 할당
3) 책임 주도 설계
4) 메시지가 객체를 결정한다.
5) 행동이 상태를 결정한다.

### <a href="Chapter 03. 역할, 책임, 협력/3.3 역할.md" target="_blank">3.3 역할</a>
1) 역할과 협력
2) 유연하고 재사용 가능한 협력
3) 객체 대 역할
4) 추상화 관점에서의 역할
5) 배우와 배역

---

## Chapter 04. 설계 품질과 트레이드오프

### Intro
- 책임이 객체지향 애플리케이션 전체의 품질을 결정한다.
  - 좋은 설계는 오늘의 요구사항을 만족하면서도, 내일의 변경을 수용할 수 있는 설계다.
  - 좋은 객체지향 설계는 올바른 객체에게 올바른 책임을 할당하면서 낮은 결합도와 높은 응집도를 가진 구조를 창조하는 활동이다.
- 캡슐화를 잘 지키면 응집도를 모듈 안의 응집도를 높이고, 모듈 간 결합도를 높일 수 있다.
- 책임에 초점을 맞춘 설계를 해야한다. 필요한 책임만을 퍼블릭 인터페이스로 노출함으로서, 캡슐화를 지킬 수 있고, 유지보수하기 쉬운 안정적인
설계를 얻어낼 수 있다. 결과적으로 설계의 품질을 향상시킬 수 있다.
- 데이터 중심의 설계는 퍼블릭 인터페이스에 내부 구현을 노출시키는 결과를 낳기 때문에 결과적으로 설계가 변경에 취약해진다.

### <a href="Chapter 04. 설계 품질과 트레이드오프/4.1 데이터 중심의 영화 예매 시스템.md" target="_blank">4.1 데이터 중심의 영화 예매 시스템</a>
1) 데이터 중심 설계
2) 책임 중심 설계
3) 데이터 중심 영화 예매 시스템 구현

### <a href="Chapter 04. 설계 품질과 트레이드오프/4.2 설계 트레이드오프.md" target="_blank">4.2 설계 트레이드오프</a>
1) 캡슐화
2) 응집도
3) 결합도
4) 설계 품질 관점에서의 캡슐화, 응집도, 결합도

### <a href="Chapter 04. 설계 품질과 트레이드오프/4.3 데이터 중심의 영화 예매 시스템의 문제점.md" target="_blank">4.3 데이터 중심의 영화 예매 시스템의 문제점</a>
1) 캡슐화 위반
2) 높은 결합도
3) 낮은 응집도
4) 응집도와 단일 책임 원칙(SRP)

### <a href="Chapter 04. 설계 품질과 트레이드오프/4.6 데이터 중심 설계의 문제점.md" target="_blank">4.6 데이터 중심 설계의 문제점</a>
1) 객체의 행동보다는 상태에 초점을 맞춘다.
2) 객체를 고립시킨 채 오프레이션을 정의하도록 만든다.

---

## Chapter 05. 책임 할당하기

### Intro
- 데이터가 아닌 책임에 초점을 맞춘 설계를 하자
- 문제는 어떤 객체에게 어떤 책임을 할당할 지 결정하기가 쉽지 않다.
- 동일한 문제를 해결할 수 있는 다양한 책임 할당 방법이 존재하며, 어떤 방법이 최선인지는 상황과 문맥에 따라 달라진다.
  - 올바른 책임을 할당하기 위해서는 다양한 관점에서 설계를 평가할 수 있어야 한다.
- GRASP 패턴은 책임 할당의 어려움을 해결하기 위한 답을 제시해준다.
  - GRASP 패턴을 통해 응집도, 결합도, 캡슐화 같은 다양한 기준에 따라 책임을 할당하고 결과를 트레이드 오프할 수 있는 기준을 배우게 될 것이다.

### <a href="Chapter 05. 책임 할당하기/5.1 책임 주도 설계를 향해.md" target="_blank">5.1 책임 주도 설계를 향해</a>
1) 데이터보다 행동을 먼저 결정하라
2) 협력이라는 문맥 안에서 책임을 결정하라
3) 책임 주도 설계

### <a href="Chapter 05. 책임 할당하기/5.2 책임 할당을 위한 GRASP 패턴.md" target="_blank">5.2 책임 할당을 위한 GRASP 패턴</a>
1) GRASP 패턴 : 객체에게 책임을 할당할 때 지침으로 삼을 수 있는 원칙들의 집합을 패턴화
2) 도메인 개념에서 출발하기
3) 정보 전문가 패턴 : 책임을 수행할 정보를 가장 잘 알고 있는 객체에게 책임을 할당하라
4) 높은 응집도와 낮은 결합도

### <a href="Chapter 05. 책임 할당하기/5.3 구현을 통한 검증.md" target="_blank">5.3 구현을 통한 검증</a>
작성 예정


### <a href="Chapter 05. 책임 할당하기/5.4 책임 주도 설계의 대안.md" target="_blank">5.4 책임 주도 설계의 대안</a>
1) 리팩터링 : 책임 주도 설계의 대안
2) 메서드 분리 : 작고 목적이 명확한 메서드들로 분리하여, 응집도를 높이자
3) 메서드 이동 : 객체를 자율적으로 만들자

---

## Chapter 06. 메시지와 인터페이스

### Intro
- 클래스는 개발자가 직접 만지고, 실험하고, 고쳐볼 수 있는 실제적이면서도 구체적인 도구에 불과하다.
- 객체지향 애플리케이션의 가장 중요한 재료는 클래스가 아니라 객체들이 주고 받는 메시지이다.
  - 훌륭한 객체지향 코드를 얻기 위해서는 객체, 더 정확히 말하면 협력 안에서 객체가 수행하는 책임에 초점을 맞춰야 한다.
  - 책임은 객체가 수신할 수 있는 메시지의 기반이 된다.
  - 애플리케이션은 클래스로 구성되지만 메시지를 통해 정의된다.
  - 메시지들이 퍼블릭 인터페이스를 구성한다.
- 훌륭한 퍼블릭 인터페이스를 얻기 위해서는 책임 주도 설계 방법을 따르는 것만으로는 부족하다.
- 유연하고 재사용한 퍼블릭 인터페이스를 만드는데 도움이 되는 설계 원칙과 기법을 익히고 적용해야 한다.

### <a href="Chapter 06. 메시지와 인터페이스/6.1 협력과 메시지.md" target="_blank">6.1 협력과 메시지</a>
1) 클라이언트-서버 모델
2) 메시지와 메시지 전송
3) 메시지와 메서드
4) 퍼블릭 인터페이스와 오퍼레이션
5) 시그니처

---

## Chapter 07. 객체 분해

### <a href="Chapter 07. 객체 분해/7.1 프로시저 추상화와 데이터 추상화.md" target="_blank">7.1 프로시저 추상화와 데이터 추상화</a>
1) 추상화와 분해
2) 프로시저 추상화와 데이터 추상화
3) 객체지향 시스템 분해

---

## Chapter 08. 의존성 관리하기

---

## Chapter 09. 유연한 설계

---

## Chapter 10. 상속과 코드 재사용

---

## Chapter 11. 합성과 유연한 설계

---

## Chapter 12. 다형성

---

## Chapter 13. 서브클래싱과 서브타이핑

---

## Chapter 14. 일관성 있는 협력


---

## Chapter 15. 디자인 패턴과 프레임워크

---

## Appendix A. 계약에 의한 설계

---

## Appendix B. 타입 계층의 구현

---

## Appendix C. 동적인 협력, 정적인 코드

---
