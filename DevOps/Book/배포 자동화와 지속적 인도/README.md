
# 배포 자동화와 지속적 인도

- 다루는 것 : 젠킨스, 도커/쿠버네티스 등

---

## Chapter 01. 지속적 인도 소개

### <a href="Chapter 01. 지속적 인도 소개/1.1 지속적 인도(CD)의 이해.md" target="_blank">1.1 지속적 인도(CD)의 이해</a>
1) 전통적 인도 프로세스
2) 지속적 인도(CD)
3) 성공 사례

### <a href="Chapter 01. 지속적 인도 소개/1.2 자동 배포 파이프라인.md" target="_blank">1.2 자동 배포 파이프라인</a>
1) 자동 배포 파이프 라인
2) 지속적 통합(CI)
3) 자동 인수 테스트
4) 구성 관리


### <a href="Chapter 01. 지속적 인도 소개/1.3 CD의 전제 조건.md" target="_blank">1.3 CD의 전제 조건</a>
1) CD 요구사항
2) 조직 구조 - 데브옵스 문화
3) 조직 구조 - 프로세스 내의 고객
4) 조직 구조 - 사업적 의사 결정과 릴리스
5) 기술 및 개발의 전제 조건

### <a href="Chapter 01. 지속적 인도 소개/1.4 CD 프로세스 구축.md" target="_blank">1.4 CD 프로세스 구축</a>
1) CD 프로세스의 도구
2) 도커 생태계 : 도커, 도커 허브, 쿠버네티스
3) 젠킨스
4) 앤서블
5) 깃허브
6) 자바/스프링 부트/그래들
7) 그 외의 도구

### <a href="Chapter 01. 지속적 인도 소개/1.5 완벽한 CD 시스템 생성하기.md" target="_blank">1.5 완벽한 CD 시스템 생성하기</a>
1) 도커 : 애플리케이션을 이미지로 패키징
2) 젠킨스 구성하기
3) 지속적 통합(CI) 파이프라인
4) 자동 인수 테스트
5) 쿠버네티스 클러스터링
6) 앤서블로 하는 구성 관리
7) 지속적 인도 파이프라인/지속적 인도 - 고급편

---

## Chapter 02. 도커 소개

### <a href="Chapter 02. 도커 소개/2.1 도커 소개.md" target="_blank">2.1 도커 소개</a>
1) 하드웨어 가상화 vs 컨테이너화
2) 도커의 필요성
3) 고양이와 가축
4) 다른 컨테이너화 기술

### <a href="Chapter 02. 도커 소개/2.2 도커 설치.md" target="_blank">2.2 도커 설치</a>
1) 도커에 필요한 환경
2) 로컬 머신에 설치하기
3) 서버에 설치하기 (미작성)

### <a href="Chapter 02. 도커 소개/2.3 도커에서 hello-world 실행하기.md" target="_blank">2.3 도커에서 hello-world 실행하기</a>
1) hello-world
2) 도커 엔진의 컴포넌트

### <a href="Chapter 02. 도커 소개/2.4 도커 애플리케이션.md" target="_blank">2.4 도커 애플리케이션</a>
1) 도커 허브에서 원하는 애플리케이션을 찾는 방법
2) 도커 허브 검색 페이지에서 찾기
3) docker search 명령어로 찾기
4) 도커 허브에서 가져온 이미지로 컨테이너 실행

### <a href="Chapter 02. 도커 소개/2.5 도커 이미지 빌드.md" target="_blank">2.5 도커 이미지 빌드</a>
1) 도커 commit을 통해 이미지 빌드하기
2) Dockerfile을 통해 이미지 빌드하기
3) 자주 사용하는 Dockerfile 명령어
4) 도커 애플리케이션 완성하기
5) 환경 변수 정의하기

### <a href="Chapter 02. 도커 소개/2.6 도커 컨테이너 상태.md" target="_blank">2.6 도커 컨테이너 상태</a>
1) `docker run -d` : 백그라운드에서 컨테이너 실행
2) `docker ps` : 실행 중인 컨테이너 확인
3) `docker ps -a` : 모든 상태의 컨테이너 확인(실행 상태, 중지상태, ...)
4) 도커 컨테이너의 상태 및 상태 전환 명령어

### <a href="Chapter 02. 도커 소개/2.7 도커 네트워킹.md" target="_blank">2.7 도커 네트워킹</a>
1) 서비스 실행 및 호스트의 포트에 바인딩
2) 작성 중...

---

