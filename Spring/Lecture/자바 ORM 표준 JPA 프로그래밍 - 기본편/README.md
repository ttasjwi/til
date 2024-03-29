
# 자바 ORM 표준 JPA 프로그래밍 - 기본편

---

## Chapter 01. JPA 소개
- 1.1 SQL 중심적인 개발의 문제점
- 1.2 JPA 소개

---

## Chapter 02. JPA 시작하기
### <a href="Chapter 02. JPA 시작하기/2.1 Hello JPA - 프로젝트 생성.md" target="_blank">2.1 Hello JPA - 프로젝트 생성</a>
1) H2 데이터베이스 설치
2) maven 프로젝트 생성
3) `pom.xml`의 `dependencies`에 의존 라이브러리 추가
4) persistence.xml
5) IntelliJ Setting
6) 실행 확인

### <a href="Chapter 02. JPA 시작하기/2.2 Hello JPA - 애플리케이션 개발.md" target="_blank">2.2 Hello JPA - 애플리케이션 개발</a>
1) JPA 구동 방식 : EntityManagerFactory, EntityManager
2) 객체와 테이블을 생성하고 매핑하기
3) JPA를 통한 데이터 변경은 트랜잭션 안에서 이루어져야한다.
4) 엔티티 매니저(JPA)를 통한 비즈니스 로직 수행(등록, 수정, 삭제, 조회)
5) JPQL(Java Persistence Query Language) : 엔티티를 대상으로 한 쿼리 언어

---

## Chapter 03. 영속성 관리 - 내부 동작 방식

### <a href="Chapter 03. 영속성 관리 - 내부 동작 방식/3.1 영속성 컨텍스트 1.md" target="_blank">3.1 영속성 컨텍스트 1</a>
1) 엔티티 매니저 팩토리, 엔티티 매니저, 커넥션
2) 영속성 컨텍스트(Persistence Context)
3) 엔티티의 생명 주기

### <a href="Chapter 03. 영속성 관리 - 내부 동작 방식/3.2 영속성 컨텍스트 2.md" target="_blank">3.2 영속성 컨텍스트 2</a>
작성 중

### <a href="Chapter 03. 영속성 관리 - 내부 동작 방식/3.3 플러시.md" target="_blank">3.3 플러시</a>
작성 중

### <a href="Chapter 03. 영속성 관리 - 내부 동작 방식/3.4 준영속 상태.md" target="_blank">3.4 준영속 상태</a>
작성 중

---

## Chapter 04. 엔티티 매핑
### 4.1 객체와 테이블 매핑
### 4.2 데이터베이스 스키마 자동 생성
### 4.3 필드와 컬럼 매핑
### 4.4 기본 키 매핑
### 4.5 실전 예제 1 - 요구사항 분석과 기본 매핑

---

## Chapter 05. 연관관계 매핑 기초
### 5.1 단방향 연관관계
### 5.2 양방향 연관관계와 연관관계의 주인 1- 기본
### 5.3 양방향 연관관계와 연관관계의 주인 2 - 주의점, 정리 
### 5.4 실전 예제 2 - 연관관계 매핑 시작

---

## Chapter 06. 다양한 연관관계 매핑
### 6.1 다대일 [N:1]
### 6.2 일대다 [1:N]
### 6.3 일대일 [1:1]
### 6.4 다대다 [N:M]
### 6.5 실전 예제 3 - 다양한 연관관계 매핑

---

## Chapter 07. 고급 매핑
### 7.1 상속관계 매핑
### 7.2 Mapped Superclass - 매핑 정보 상속
### 7.3 실전 예제 4 - 상속관계 매핑

---

## Chapter 08. 프록시와 연관관계 관리
### 8.1 프록시
### 8.2 즉시 로딩과 지연 로딩
### 8.3 영속성 전이(CASCADE)와 고아 객체
### 8.4 실전 예제 5 - 연관관계 관리

## Chapter 09. 값 타입
### 9.1 기본값 타입
### 9.2 임베디드 타입
### 9.3 값 타입과 불변 객체
### 9.4 값 타입의 비교
### 9.5 값 타입 컬렉션
### 9.6 실전 예제 6 - 값 타입 매핑

---

## Chapter 10. 객체지향 쿼리 언어1 - 기본 문법
### 10.1 소개
### 10.2 기본 문법과 쿼리 API
### 10.3 프로젝션(SELECT)
### 10.4 페이징
### 10.5 조인
### 10.6 서브 쿼리
### 10.7 JPQL 타입 표현과 기타식
### 10.8 조건식(CASE 등등)
### 10.9 JPQL 함수

---

## Chapter 11. 객체지향 쿼리 언어2 - 중급 문법
### 11.1 경로 표현식
### 11.2 페치 조인 1 - 기본
### 11.3 페치 조인 2 - 한계
### 11.4 다형성 쿼리
### 11.5 엔티티 직접 사용
### 11.6 Named 쿼리
### 11.7 벌크 연산

---
