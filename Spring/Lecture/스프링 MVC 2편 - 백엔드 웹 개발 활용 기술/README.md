
# 스프링 MVC 2편 - 백엔드 웹 개발 활용 기술

---

## Chapter 01. 타임리프 - 기본 기능
- 1.01 프로젝트 생성
- 1.02 타임리프 소개
- 1.03 텍스트 - text, utext
- 1.04 변수 - SpringEL
- 1.05 기본 객체들
- 1.06 유틸리티 객체와 날짜
- 1.07 URL 링크
- 1.08 리터럴
- 1.09 연산
- 1.10 속성 값 설정
- 1.11 반복
- 1.12 조건부 평가
- 1.13 주석
- 1.14 블록
- 1.15 자바스크립트 인라인
- 1.16 템플릿 조각
- 1.17 템플릿 레이아웃1
- 1.18 템플릿 레이아웃2

---

## Chapter 02. 타임리프 - 스프링 통합과 폼

- 2.1 프로젝트 설정
- 2.2 타임리프 스프링 통합
- 2.3 입력 폼 처리
- 2.4 요구사항 추가
- 2.5 체크 박스 - 단일1
- 2.6 체크 박스 - 단일2
- 2.7 체크 박스 - 멀티
- 2.8 라디오 버튼
- 2.9 셀렉트 박스

---

## Chapter 03. 메시지, 국제화

### 3.1 프로젝트 설정
### 3.2 메시지, 국제화 소개
### <a href="Chapter 03. 메시지, 국제화/3.3 스프링 메시지 소스 설정.md" target="_blank">3.3 스프링 메시지 소스 설정</a>
1) MessageSource
2) MessageSource 수동 빈 등록
3) 스프링 부트가 지원하는 메시지 소스 설정
4) (실습) 메시지 파일 만들기
### 3.4 스프링 메시지 소스 사용
### 3.5 웹 애플리케이션에 메시지 적용하기
### 3.6 웹 애플리케이션에 국제화 적용하기

---

## Chapter 04. 검증1 - Validation
- 4.01 검증 요구사항
- 4.02 프로젝트 설정 V1
- 4.03 검증 직접 처리 - 소개
- 4.04 검증 직접 처리 - 개발
- 4.05 프로젝트 준비 V2
- 4.06 BindingResult1
- 4.07 BindingResult2
- 4.08 FieldError, ObjectError
- 4.09 오류 코드와 메시지 처리1
- 4.10 오류 코드와 메시지 처리2
- 4.11 오류 코드와 메시지 처리3
- 4.12 오류 코드와 메시지 처리4
- 4.13 오류 코드와 메시지 처리5
- 4.14 오류 코드와 메시지 처리6
- 4.15 Validator 분리1
- 4.16 Validator 분리2

---

## Chapter 05. 검증2 - Bean Validation

- 5.01 Bean Validation - 소개
- 5.02 Bean Validation - 시작
- 5.03 Bean Validation - 프로젝트 준비 V3
- 5.04 Bean Validation - 스프링 적용
- 5.05 Bean Validation - 에러 코드
- 5.06 Bean Validation - 오브젝트 오류
- 5.07 Bean Validation - 수정에 적용
- 5.08 Bean Validation - 한계
- 5.09 Bean Validation - groups
- 5.10 Form 전송 객체 분리 - 프로젝트 준비 V4
- 5.11 Form 전송 객체 분리 - 소개
- 5.12 Form 전송 객체 분리 - 개발
- 5.13 Bean Validation - HTTP 메시지 컨버터

---

## Chapter 06. 로그인 처리1 - 쿠키, 세션
- 6.01 로그인 요구사항
- 6.02 프로젝트 생성
- 6.03 홈 화면
- 6.04 회원 가입
- 6.05 로그인 기능
- 6.06 로그인 처리하기 - 쿠키 사용
- 6.07 쿠키와 보안 문제
- 6.08 로그인 처리하기 - 세션 동작 방식
- 6.09 로그인 처리하기 - 세션 직접 만들기
- 6.10 로그인 처리하기 - 직접 만든 세션 적용
- 6.11 로그인 처리하기 - 서블릿 HTTP 세션1
- 6.12 로그인 처리하기 - 서블릿 HTTP 세션2
- 6.13 세션 정보와 타임아웃 설정

---

## Chapter 07. 로그인 처리2 - 필터, 인터셉터
### <a href="Chapter 07. 로그인 처리2 - 필터, 인터셉터/7.1 서블릿 필터 - 소개.md" target="_blank">7.1 서블릿 필터 - 소개</a>
1) 요구사항 : 비 로그인 사용자 차단에 관한 공통 관심사
2) 웹과 관련된 공통 관심사 해결 : 서블릿 필터, 스프링 인터셉터
3) 서블릿 필터의 흐름 : HTTP 요청 -> WAS -> 필터 -> 서블릿 -> 컨트롤러
4) 서블릿 필터의 요청 필터링 : 부적절한 요청 끊어내기
5) 서블릿 필터의 체이닝 : 여러 필터를 둘 수 있다.
6) Filter 인터페이스

### <a href="Chapter 07. 로그인 처리2 - 필터, 인터셉터/7.2 서블릿 필터 - 요청 로그.md" target="_blank">7.2 서블릿 필터 - 요청 로그</a>
작성 중

### <a href="Chapter 07. 로그인 처리2 - 필터, 인터셉터/7.3 서블릿 필터 - 인증 체크.md" target="_blank">7.3 서블릿 필터 - 인증 체크</a>
작성 중

### <a href="Chapter 07. 로그인 처리2 - 필터, 인터셉터/7.4 스프링 인터셉터 - 소개.md" target="_blank">7.4 스프링 인터셉터 - 소개</a>
작성 중

### <a href="Chapter 07. 로그인 처리2 - 필터, 인터셉터/7.5 스프링 인터셉터 - 요청 로그.md" target="_blank">7.5 스프링 인터셉터 - 요청 로그</a>
작성 중

### <a href="Chapter 07. 로그인 처리2 - 필터, 인터셉터/7.6 스프링 인터셉터 - 인증 체크.md" target="_blank">7.6 스프링 인터셉터 - 인증 체크</a>
작성 중

### <a href="Chapter 07. 로그인 처리2 - 필터, 인터셉터/7.7 ArgumentResolver 활용.md" target="_blank">7.7 ArgumentResolver 활용</a>
작성 중

---

## Chapter 08. 예외 처리와 오류 페이지
- 8.1 프로젝트 생성
- 8.2 서블릿 예외 처리 - 시작
- 8.3 서블릿 예외 처리 - 오류 화면 제공
- 8.4 서블릿 예외 처리 - 오류 페이지 작동 원리
- 8.5 서블릿 예외 처리 - 필터
- 8.6 서블릿 예외 처리 - 인터셉터
- 8.7 스프링 부트 - 오류 페이지1
- 8.8 스프링 부트 - 오류 페이지2

---

## Chapter 09. API 예외 처리
- 9.01 시작
- 9.02 스프링 부트 기본 오류 처리
- 9.03 HandlerExceptionResolver 시작
- 9.04 HandlerExceptionResolver 활용
- 9.05 스프링이 제공하는 ExceptionResolver1
- 9.06 스프링이 제공하는 ExceptionResolver2
- 9.07 @ExceptionHandler
- 9.08 @ControllerAdvice

---

## Chapter 10. 스프링 타입 컨버터

### <a href="Chapter 10. 스프링 타입 컨버터/10.01 프로젝트 생성.md" target="_blank">10.01 프로젝트 생성</a>
1) 프로젝트 생성
2) `build.gradle`에 라이브러리 추가
3) IDE 설정
4) 실행 확인

### <a href="Chapter 10. 스프링 타입 컨버터/10.02 스프링 타입 컨버터 소개.md" target="_blank">10.02 스프링 타입 컨버터 소개</a>
1) (실습) 문자열을 숫자로 변환 - 기본 방식
2) (실습) 문자열을 숫자로 변환 - 스프링
3) 스프링의 타입 변환 - 예시
4) 스프링의 타입 변환 - Converter 인터페이스

### <a href="Chapter 10. 스프링 타입 컨버터/10.03 타입 컨버터 - Converter.md" target="_blank">10.03 타입 컨버터 - Converter</a>
1) Converter 인터페이스
2) (실습) 기본 타입을 변환하는 Converter 만들어보기
3) (실습) 사용자 정의 타입으로 변환하는 Converter
4) 한 걸음 더: 타입 컨버터를 직접 등록하고 관리할 수 있다면...
5) (참고) 스프링이 제공하는 다양한 방식의 convert 방법
6) (참고) 스프링이 제공하는 컨버터 구현체들

### <a href="Chapter 10. 스프링 타입 컨버터/10.04 컨버전 서비스 - ConversionService.md" target="_blank">10.04 컨버전 서비스 - ConversionService</a>
1) ConversionService 인터페이스
2) 스프링이 사용한 객체 지향 원리 - 등록과 사용 분리
3) 스프링이 사용한 객체 지향 원리 - 인터페이스 분리 원칙(ISP)

### <a href="Chapter 10. 스프링 타입 컨버터/10.05 스프링에 Converter 적용하기.md" target="_blank">10.05 스프링에 Converter 적용하기</a>
1) WebConfig을 통해, Converter 추가 등록하기
2) 컨버터를 추가하면 추가한 컨버터가 기본 컨버터보다 높은 우선순위를 가진다.
3) (실습) IpPort 타입 변환
4) 동작 원리 - ArgumentResolver 에서 ConversionService 사용

### <a href="Chapter 10. 스프링 타입 컨버터/10.06 뷰 템플릿에 컨버터 적용하기.md" target="_blank">10.06 뷰 템플릿에 컨버터 적용하기</a>
1) Thymeleaf - 컨버터를 적용하여, 객체를 문자열로 렌더링
2) Thymeleaf - form에 컨버터 적용하여 렌더링

### <a href="Chapter 10. 스프링 타입 컨버터/10.07 포맷터 - Formatter.md" target="_blank">10.07 포맷터 - Formatter</a>
작성 중

### <a href="Chapter 10. 스프링 타입 컨버터/10.08 포맷터를 지원하는 컨버전 서비스.md" target="_blank">10.08 포맷터를 지원하는 컨버전 서비스</a>
작성 중

### <a href="Chapter 10. 스프링 타입 컨버터/10.09 포맷터 적용하기.md" target="_blank">10.09 포맷터 적용하기</a>
작성 중

### <a href="Chapter 10. 스프링 타입 컨버터/10.10 스프링이 제공하는 기본 포맷터.md" target="_blank">10.10 스프링이 제공하는 기본 포맷터</a>
작성 중

---

## Chapter 11. 파일 업로드
### <a href="Chapter 11. 파일 업로드/11.1 파일 업로드 소개.md" target="_blank">11.1 파일 업로드 소개</a>
작성 중

### <a href="Chapter 11. 파일 업로드/11.2 프로젝트 생성.md" target="_blank">11.2 프로젝트 생성</a>
작성 중

### <a href="Chapter 11. 파일 업로드/11.3 서블릿과 파일 업로드 1.md" target="_blank">11.3 서블릿과 파일 업로드 1</a>
작성 중

### <a href="Chapter 11. 파일 업로드/11.4 서블릿과 파일 업로드 2.md" target="_blank">11.4 서블릿과 파일 업로드 2</a>
작성 중

### <a href="Chapter 11. 파일 업로드/11.5 스프링과 파일 업로드.md" target="_blank">11.5 스프링과 파일 업로드</a>
작성 중

### <a href="Chapter 11. 파일 업로드/11.6 예제로 구현하는 파일 업로드, 다운로드.md" target="_blank">11.6 예제로 구현하는 파일 업로드, 다운로드</a>
작성 중

---
