# <a href = "../../README.md" target="_blank">이펙티브 자바</a>
## Chapter 02. 객체의 생성과 파괴
### item 01. 생성자 대신 정적 팩터리 메서드를 고려하라
1) 장점1 - 이름을 가질 수 있다
2) 장점2 - 호출될 때마다 인스턴스를 새로 생성하지 않아도 된다
3) 장점3 - 반환 타입의 하위 타입 객체를 반환할 수 있는 능력이 있다
4) 장점4 - 입력 매개변수에 따라 매번 다른 클래스의 객체를 반환할 수 있다
5) 장점5 - 정적 팩터리 메서드를 작성하는 시점에는 반환할 객체의 클래스가 존재하지 않아도 된다

---

# item 01. 생성자 대신 정적 팩터리 메서드를 고려하라

---

## 1) 핵심 정리

### 1.1 장점
- <a href="1.1 장점1 - 이름을 가질 수 있다.md" target="_blank">이름을 가질 수 있다. (← 동일한 시그니처의 생성자는 단 하나만 만들 수 있다.)</a>
- <a href="1.2 장점2 - 호출될 때마다 인스턴스를 새로 생성하지 않아도 된다.md" target="_blank">호출될 때마다 인스턴스를 새로 생성하지 않아도 된다. (Boolean.valueOf)</a>
- 반환 타입의 하위 타입 객체를 반환할 수 있는 능력이 있다. (인터페이스 기반 프레임워크, 인터페이스에 정적 메소드)
- 입력 매개변수가 따라 매번 다른 클래스의 객체를 반환할 수 있다. (EnumSet)
- 정적 팩터리 메서드를 작성하는 시점에는 반환할 객체의 클래스가 존재하지 않아도 된다. (서비스 제공자 프레임워크)

### 1.2 단점
- 상속을 하려면 public이나 protected 생성하기 필요하니 정적 팩터리 메서드만 제공하면 하위 클래스를 만들 수 없
다.
- 정적 팩터리 메서드는 프로그래머가 찾기 어렵다.

---

## 2) 완벽 공략
- 열거 타입
- 플라이웨이트 패턴
- 인터페이스와 정적 메서드
- 서비스 제공자 프레임워크
- 서비스 제공자 인터페이스
- 리플렉션
- 브리지 패턴
- 의존 객체 주입 프레임워크

---
