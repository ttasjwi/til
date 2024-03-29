
# Real MySQL 8.0

---

## Chapter 01. 소개
### 1.1 MySQL 소개
### <a href="Chapter 01. 소개/1.2 왜 MySQL인가.md">1.2 왜 MySQL인가?</a>
1) Oracle vs MySQL
2) DBMS 선택의 우선순위
---

## Chapter 02. 설치와 설정

### 2.1 MySQL 서버 설치
1) 버전과 에디션(엔터프라이즈와 커뮤니티) 선택
2) MySQL 설치

### 2.2 MySQL 서버의 시작과 종료
1) 설정 파일 및 데이터 파일 준비
2) 시작과 종료
3) 서버 연결 테스트

### 2.3 MySQL 서버 업그레이드
1) 인플레이스 업그레이드 제약 사항
2) MySQL 8.0 업그레이드 시 고려 사항
3) MySQL 8.0 업그레이드

### 2.4 서버 설정
1) 설정 파일의 구성
2) MySQL 시스템 변수의 특징
3) 글로벌 변수와 세션 변수
4) 정적 변수와 동적 변수
5) SET PERSIST
6) my.cnf 파일

---

## Chapter 03. 사용자 및 권한
### 3.1 사용자 식별

### 3.2 사용자 계정 관리
1) 시스템 계정과 일반 계정
2) 계정 생성

### 3.3 비밀번호 관리
1) 고수준 비밀번호
2) 이중 비밀번호

### 3.4 권한(Privilege)

### 3.5 역할(Role)

---

## Chapter 04. 아키텍처
### 4.1 MySQL 엔진 아키텍처
1) MySQL의 전체 구조
2) MySQL 스레딩 구조
3) 메모리 할당 및 사용 구조
4) 플러그인 스토리지 엔진 모델
5) 컴포넌트
6) 쿼리 실행 구조
7) 복제
8) 쿼리 캐시
9) 스레드 풀
10) 트랜잭션 지원 메타데이터

### 4.2 InnoDB 스토리지 엔진 아키텍처
1) 프라이머리 키에 의한 클러스터링
2) 외래 키 지원
3) MVCC(Multi Version Concurrency Control)
4) 잠금 없는 일관된 읽기(Non-Locking Consistent Read)
5) 자동 데드락 감지
6) 자동화된 장애 복구
7) InnoDB 버퍼 풀
8) Double Write Buffer
9) 언두 로그
10) 체인지 버퍼
11) 리두 로그 및 로그 버퍼
12) 어댑티브 해시 인덱스
13) InnoDB와 MyISAM, MEMORY 스토리지 엔진 비교

### 4.3 MyISAM 스토리지 엔진 아키텍처
1) 키 캐시
2) 운영체제의 캐시 및 버퍼
3) 데이터 파일과 프라이머리 키(인덱스) 구조

### 4.4 MySQL 로그 파일
1) 에러 로그 파일
2) 제너럴 쿼리 로그 파일(제너럴 로그 파일, General log)
3) 슬로우 쿼리 로그

---

## Chapter 05. 트랜잭션과 잠금
### 5.1 트랜잭션
1) MySQL에서의 트랜잭션
2) 주의사항

### 5.2 MySQL 엔진의 잠금
1) 글로벌 락
2) 테이블 락
3) 네임드 락
4) 메타데이터 락

### 5.3 InnoDB 스토리지 엔진 잠금
1) InnoDB 스토리지 엔진의 잠금
2) 인덱스와 잠금
3) 레코드 수준의 잠금 확인 및 해제

### 5.4 MySQL의 격리 수준
1) READ UNCOMMITTED
2) READ COMMITTED
3) REPEATABLE READ
4) SERIALIZABLE

---

## Chapter 06. 데이터 압축
### 6.1 페이지 압축
### 6.2 테이블 압축
1) 압축 테이블 생성
2) KEY_BLOCK_SIZE 결정
3) 압축된 페이지의 버퍼 풀 적재 및 사용
4) 테이블 압축 관련 설정

---

## Chapter 07. 데이터 암호화
### 7.1 MySQL 서버의 데이터 암호화
1) 2단계 키 관리
2) 암호화와 성능
3) 암호화와 복제
### 7.2 keyring_file 플러그인 설치
### 7.3 테이블 암호화
1) 테이블 생성
2) 응용 프로그램 암호화와의 비교
3) 테이블스페이스 이동
### 7.4 언두 로그 및 리두 로그 암호화
### 7.5 바이너리 로그 암호화
1) 바이너리 로그 암호화 키 관리
2) 바이너리 로그 암호화 키 변경
3) mysqlbinlog 도구 활용

---

## Chapter 08. 인덱스
### 8.1 디스크 읽기 방식
1) 하드 디스크 드라이브(HDD)와 솔리드 스테이트 드라이브(SSD)
2) 랜덤 I/O와 순차 I/O
### 8.2 인덱스란?
### 8.3 B-Tree 인덱스
1) 구조 및 특성
2) B-Tree 인덱스 키 추가 및 삭제
3) B-Tree 인덱스 사용에 영향을 미치는 요소
4) B-Tree 인덱스를 통한 데이터 읽기
5) 다중 칼럼(Multi-column) 인덱스
6) B-Tree 인덱스의 정렬 및 스캔 방향
7) B-Tree 인덱스의 가용성과 효율성

### 8.4 R-Tree 인덱스
1) 구조 및 특성
2) R-Tree 인덱스의 용도

### 8.5 전문 검색 인덱스
1) 인덱스 알고리즘
2) 전문 검색 인덱스의 가용성

### 8.6 함수 기반 인덱스
1) 가상 칼럼을 이용한 인덱스
2) 함수를 이용한 인덱스

### 8.7 멀티 밸류 인덱스
### 8.8 클러스터링 인덱스
1) 클러스터링 인덱스
2) 세컨더리 인덱스에 미치는 영향
3) 클러스터링 인덱스의 장점과 단점
4) 클러스터링 테이블 사용 시 주의사항
### 8.9 유니크 인덱스
1) 유니크 인덱스와 일반 세컨더리 인덱스의 비교
2) 유니크 인덱스 사용 시 주의사항
### 8.10 외래키
1) 자식 테이블의 변경이 대기하는 경우
2) 부모 테이블의 변경 작업이 대기하는 경우

---

## Chapter 09. 옵티마이저와 힌트

### 9.1 개요
1) 쿼리 실행 절차
2) 옵티마이저의 종류

### 9.2 기본 데이터 처리
1) 풀 테이블 스캔과 풀 인덱스 스캔
2) 병렬 처리
3) ORDER BY 처리(Using filesort)
4) GROUP BY 처리
5) DISTINCT 처리
6) 내부 임시 테이블 활용

### 9.3 고급 최적화
1) 옵티마이저 스위치 옵션
2) 조인 최적화 알고리즘
### 9.4 쿼리 힌트
1) 인덱스 힌트
2) 옵티마이저 힌트

---

## Chapter 10. 실행 계획
### 10.1 통계 정보
1) 테이블 및 인덱스 통계 정보
2) 히스토그램
3) 코스트 모델(Cost Model)

### 10.2 실행 계획 확인
1) 실행 계획 출력 포맷
2) 쿼리의 실행 시간 확인

### 10.3 실행 계획 분석
1) id 칼럼
2) select_type 칼럼
3) table 칼럼
4) partitions 칼럼
5) type 칼럼
6) possible_keys 칼럼
7) key 칼럼
8) key_len 칼럼
9) ref 칼럼
10) rows 칼럼
11) filtered 칼럼
12) Extra 칼럼

---

## Chapter 11. 쿼리 작성 및 최적화

### 11.1 쿼리 작성과 연관된 시스템 변수
1) SQL 모드
2) 영문 대소문자 구분
3) My
### 11.2 매뉴얼의 SQL 문법 표기를 읽는 방법

### 11.3 MySQL 연산자와 내장 함수
1) 리터럴 표기법 문자열
2) MySQL 연산자
3) MySQL 내장 함수

### 11.4 SELECT
1) SELECT 절의 처리 순서
2) WHERE 절과 GROUP BY 절, ORDER BY 절의 인덱스 사용
3) WHERE 절의 비교 조건 사용 시 주의사항
4) DISTINCT
5) LIMIT n
6) COUNT()
7) JOIN
8) GROUP BY
9) ORDER BY
10) 서브쿼리
11) CTE(Common Table Expression)
12) 윈도우 함수(Window Function)
13) 잠금을 사용하는 SELECT

### 11.5 INSERT
1) 고급 옵션
2) LOAD DATA 명령 주의 사항
3) 성능을 위한 테이블 구조
### 11.6 UPDATE와 DELETE
1) UPDATE ... ORDER BY ... LIMIT n
2) JOIN UPDATE
3) 여러 레코드 UPDATE
4) JOIN DELETE
### 11.7 스키마 조작(DDL)
1) 온라인 DDL
2) 데이터베이스 변경
3) 테이블 스페이스 변경
4) 테이블 변경
5) 칼럼 변경
6) 인덱스 변경
7) 테이블 변경 묶음 실행
8) 프로세스 조회 및 강제 종료
9) 활성 트랜잭션 조회
### 11.8 쿼리 성능 테스트
1) 쿼리의 성능에 영향을 미치는 요소

---

## Chapter 12. 확장 검색
### 12.1 전문 검색
1) 전문 검색 인덱스의 생성과 검색
2) 전문 검색 쿼리 모드
3) 전문 검색 인덱스 디버깅

### 12.2 공간 검색
1) 용어 설명
2) SRS(Spatial Reference System)
3) 투영 좌표계와 평면 좌표계
4) 지리 좌표계

---

## Chapter 13. 파티션
### 13.1 개요
1) 파티션을 사용하는 이유
2) MySQL 파티션의 내부 처리
### 13.2 주의사항
1) 파티션의 제약 사항
2) 파티션 사용 시 주의사항
### 13.3 MySQL 파티션의 종류
1) 레인지 파티션
2) 리스트 파티션
3) 해시 파티션
4) 키 파티션
5) 리니어 해시 파티션/리니어 키 파티션
6) 파티션 테이블의 쿼리 성능

---

## Chapter 14. 스토어드 프로그램
### 14.1 스토어드 프로그램의 장단점
1) 스토어드 프로그램의 장점
2) 스토어드 프로그램의 단점
### 14.2 스토어드 프로그램의 문법
1) 예제 테스트 시 주의사항
2) 스토어드 프로시저
3) 스토어드 함수
4) 트리거
5) 이벤트
6) 스토어드 프로그램 본문(Body) 작성
### 14.3 스토어드 프로그램의 보안 옵션
1) DEFINER와 SQL SECURITY 옵션
2) DETERMINISTIC과 NOT DETERMINISTIC 옵션
### 14.4 스토어드 프로그램의 참고 및 주의사항
1) 한글 처리
2) 스토어드 프로그램과 세션 변수
3) 스토어드 프로시저와 재귀 호출
4) 중첩된 커서 사용

---

## Chapter 15. 데이터 타입
### 15.1 문자열(CHAR와 VARCHAR)
1) 저장 공간
2) 저장 공간과 스키마 변경(Online DDL)
3) 문자 집합(캐릭터 셋)
4) 콜레이션(Collation)
5) 비교 방식
6) 문자열 이스케이프 처리

### 15.2 숫자
1) 정수
2) 부동 소수점
3) DECIMAL
4) 정수 타입의 칼럼을 생성할 때의 주의사항
5) 자동 증가(AUTO_INCREMENT) 옵션 사용

### 15.3 날짜와 시간
1) 자동 업데이트

### 15.4 ENUM과 SET
1) ENUM
2) SET

### 15.5 TEXT와 BLOB

### 15.6 공간 데이터 타입
1) 공간 데이터 생성
2) 공간 데이터 조회

### 15.7 JSON 타입
1) 저장 방식
2) 부분 업데이트 성능
3) JSON 타입 콜레이션과 비교
4) JSON 칼럼 선택

### 15.8 가상 칼럼(파생 칼럼)

---

## Chapter 16. 복제
### 16.1 개요
### 16.2 복제 아키텍처
### 16.3 복제 타입
1) 바이너리 로그 파일 위치 기반 복제
2) 글로벌 트랜잭션 아이디(GTID) 기반 복제
### 16.4 복제 데이터 포맷
1) Statement 기반 바이너리 로그 포맷
2) Row 기반 바이너리 로그 포맷
3) Mixed 포맷
4) Row 포맷의 용량 최적화
### 16.5 복제 동기화 방식
1) 비동기 복제(Asynchronous replication)
2) 반동기 복제(Semi-synchronous replication)
### 16.6 복제 토폴로지
1) 싱글 레플리카 복제 구성
2) 멀티 레플리카 복제 구성
3) 체인 복제 구성
4) 듀얼 소스 복제 구성
5) 멀티 소스 복제 구성
### 16.7 복제 고급 설정
1) 지연된 복제(Delayed Replication)
2) 멀티 스레드 복제(Multi-threaded Replication)
3) 크래시 세이프 복제(Crash-safe Replication)
4) 필터링된 복제(Filtered Replication)

---

## Chapter 17. InnoDB 클러스터
### 17.01 InnoDB 클러스터 아키텍처
### 17.02 그룹 복제(Group Replication)
1) 그룹 복제 아키텍처
2) 그룹 복제 모드
3) 그룹 멤버 관리(Group Membership)
4) 그룹 복제에서의 트랜잭션 처리
5) 그룹 복제의 자동 장애 감지 및 대응
6) 그룹 복제의 분산 복구
7) 그룹 복제 요구사항
8) 그룹 복제 제약 사항

### 17.03 MySQL 셸

### 17.04 MySQL 라우터

### 17.05 InnoDB 클러스터 구축
1) InnoDB 클러스터 요구사항
2) InnoDB 클러스터 생성

### 17.06 InnoDB 클러스터 모니터링

### 17.07 InnoDB 클러스터 작업
1) 클러스터 모드 변경
2) 프라이머리 변경
3) 인스턴스 제거
4) 클러스터 해체
5) 클러스터 및 인스턴스 설정 변경

### 17.08 InnoDB 클러스터 트러블슈팅
1) 클러스터 인스턴스 장애
2) 클러스터의 정족수 손실

### 17.09 InnoDB 클러스터 버전 업그레이드
### 17.10 InnoDB 클러스터 제약 사항

---

## Chapter 18. Performance 스키마 & Sys 스키마
### 18.1 Performance 스키마란?
### 18.2 Performance 스키마 구성
1) Setup 테이블
2) Instance 테이블
3) Connection 테이블
4) Variable 테이블
5) Event 테이블
6) Summary 테이블
7) Lock 테이블
8) Replication 테이블
9) Clone 테이블
10) 기타 테이블

### 18.3 Performance 스키마 설정
1) 메모리 사용량 설정
2) 데이터 수집 및 저장 설정

### 18.4 Sys 스키마란?

### 18.5 Sys 스키마 사용을 위한 사전 설정

### 18.6 Sys 스키마 구성

### 18.7 Performance 스키마 및 Sys 스키마 활용 예제
1) 호스트 접속 이력 확인
2) 미사용 DB 계정 확인
3) MySQL 총 메모리 사용량 확인
4) 스레드별 메모리 사용량 확인
5) 미사용 인덱스 확인
6) 중복된 인덱스 확인
7) 변경이 없는 테이블 목록 확인
8) I/O 요청이 많은 테이블 목록 확인
9) 테이블별 작업량 통계 확인
10) 테이블의 Auto-Increment 칼럼 사용량 확인
11) 풀 테이블 스캔 쿼리 확인
12) 자주 실행되는 쿼리 목록 확인
13) 실행 시간이 긴 쿼리 목록 확인
14) 정렬 작업을 수행한 쿼리 목록 확인
15) 임시 테이블을 생성하는 쿼리 목록 확인
16) 트랜잭션이 활성 상태인 커넥션에서 실행한 쿼리 내역 확인
17) 쿼리 프로파일링
18) ALTER 작업 진행률 확인
19) 메타데이터 락 대기 확인
20) 데이터 락 대기 확인

