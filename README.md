# Market Live

## 프로젝트 개요
- WebRTC를 활용한 화상 중고거래 서비스

## 주요 기능
- (판매자)1 : (구매자)N 의 live-commerce 시스템
- 실시간 채팅
- multi-room 구현
- 쪽지 보내기

## 맡은 역할
- RTC server
  - multi-room 구현
  - 1:N broadcasting system
  - chatting
- Infra
  - CI/CD pipeline(jenkins)
  - ssl 인증서
  - docker

## 주요 기술
### 1. FRONTEND 
- React
  - mobile에서도 동작 가능한 반응형 웹 구현

### 2. BACKEND 
- Spring Boot : 전반적인 Rest Controller 구현
- JWT
- JPA (Hibernate)
- WebSocket : media server 통신, chatting 구현
- Redis : nosql database. room 정보 저장
- MySQL : 이용자 정보 저장
- Kurento : WebRTC 기능적 구현을 제공하는 media server

### 3. BACKEND - Infra 
- Nginx : reverse proxy 처리
- SSL : Certbot을 사용하여 무료 인증서 발급
  - rtc 사용 시 SSL 필수
- AWS EC2 ubuntu
- Docker : 프로그램 관리 및 배포 용이
- Jenkins : 배포 자동화

### 4. TEAM
- GitLab
- Jira
- Google Drive

## 동작 화면

![동작 화면](images/01_capture.jpg)

## Backend Architecture
![서버 구조](images/02_architecture.jpg)


