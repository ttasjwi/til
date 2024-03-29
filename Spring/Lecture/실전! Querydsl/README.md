
# 실전! Querydsl

---

## Chapter 01. 프로젝트 환경설정
- 1.1 프로젝트 생성
- 1.2 Querydsl 설정과 검증
- 1.3 라이브러리 살펴보기
- 1.4 H2 데이터베이스 설치
- 1.5 스프링 부트 설정 - JPA, DB

---

## Chapter 02. 예제 도메인 모델
- 2.1 예제 도메인 모델과 동작확인

---

## Chapter 03. 기본 문법
- 3.01 시작 - JPQL vs Querydsl
- 3.02 기본 Q-Type 활용
- 3.03 검색 조건 쿼리
- 3.04 결과 조회
- 3.05 정렬
- 3.06 페이징
- 3.07 집합 
- 3.08 조인 - 기본 조인
- 3.09 조인 - on절
- 3.10 조인 - 페치 조인
- 3.11 서브 쿼리
- 3.12 Case 문
- 3.13 상수, 문자 더하기

---

## Chapter 04. 중급 문법
### 4.1 프로젝션과 결과 반환 - 기본
### 4.2 프로젝션과 결과 반환 - DTO 조회
### 4.3 프로젝션과 결과 반환 - @QueryProjection
### 4.4 동적 쿼리 - BooleanBuilder 사용
### 4.5 동적 쿼리 - Where 다중 파라미터 사용
### 4.6 수정, 삭제 벌크 연산


### <a href="Chapter 04. 중급 문법/4.7 SQL function 호출하기.md" target="_blank">4.7 SQL function 호출하기</a>
1) 조건 : 방언 등록
2) 함수 호출 방법
3) ANSI 표준 SQL 함수는 Querydsl에 상당부분 내장되어 있다.

---

## Chapter 05. 실무 활용 - 순수 JPA와 Querydsl
### <a href="Chapter 05. 실무 활용 - 순수 JPA와 Querydsl/5.1 순수 JPA 리포지토리와 Querydsl.md" target="_blank">5.1 순수 JPA 리포지토리와 Querydsl</a>
1) 리포지토리에 Querydsl 의존관계 등록
2) 리포지토리 계층에서 Querydsl 사용하기 - 실습 및 테스트

### <a href="Chapter 05. 실무 활용 - 순수 JPA와 Querydsl/5.2 동적 쿼리와 성능 최적화 조회 - Builder 사용.md" target="_blank">5.2 동적 쿼리와 성능 최적화 조회 - Builder 사용</a>
1) (실습) 조회 대상 DTO 생성 : MemberTeamDto
2) (실습) 조회 조건 DTO 생성 : MemberSearchCondition
3) BooleanBuilder을 구성하여 동적 쿼리 작성하기
4) 주의점 : 파라미터에 아무 것도 없을 때

### <a href="Chapter 05. 실무 활용 - 순수 JPA와 Querydsl/5.3 동적 쿼리와 성능 최적화 조회 - Where절 파라미터 사용.md" target="_blank">5.3 동적 쿼리와 성능 최적화 조회 - Where절 파라미터 사용</a>
1) (실습) BooleanExpression 메서드 분리
2) (실습) Where절에서 조건들 연결하기
3) BooleanExpression 메서드들의 재사용성
4) 여러 BooleanExpression의 조합 메서드
5) 항상 기본적으로 적용해야하는 검색 조건 공통화

### <a href="Chapter 05. 실무 활용 - 순수 JPA와 Querydsl/5.4 조회 API 컨트롤러 개발.md" target="_blank">5.4 조회 API 컨트롤러 개발</a>
1) (실습 설정) `application.yml` profile 분리
2) (실습) 샘플 회원을 java 코드로 로딩시점에 등록
3) (실습) 컨트롤러에 회원 검색 API 제공기능 추가

---

## Chapter 06. 실무 활용 - 스프링 데이터 JPA와 Querydsl
- 6.1 스프링 데이터 JPA 리포지토리로 변경
- 6.2 사용자 정의 리포지토리
- 6.3 스프링 데이터 페이징 활용1 - Querydsl 페이징 연동
- 6.4 스프링 데이터 페이징 활용2 - CountQuery 최적화
- 6.5 스프링 데이터 페이징 활용3 - 컨트롤러 개발

---

## Chapter 07. 스프링 데이터 JPA가 제공하는 Querydsl 기능
- 7.1 인터페이스 지원 - QuerydslPredicateExecutor
- 7.2 Querydsl Web 지원
- 7.3 리포지토리 지원 - QuerydslRepositorySupport
- 7.4 Querydsl 지원 클래스 직접 만들기

---
