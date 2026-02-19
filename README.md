# 🥋 Rolling (롤링) - 주짓수 라이프스타일 통합 플랫폼 Backend

![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Java](https://img.shields.io/badge/Java-17+-007396?style=for-the-badge&logo=java&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-Client-02569B?style=for-the-badge&logo=flutter&logoColor=white)

> **파편화된 주짓수 정보(오픈매트, 대회)를 하나로 모아 제공하는 B2C 커뮤니티 플랫폼입니다.**
> 복잡한 관리 기능은 걷어내고, 수련생들의 **정보 탐색**과 **외부 활동 참여**에 집중한 MVP 모델을 서비스합니다.

<br>

## 🚀 프로젝트 개요 및 개발 주안점

서버의 데이터 흐름과 클라이언트(Flutter)의 사용성을 모두 고려하여 API 및 아키텍처를 설계했습니다. 단순한 기능 구현에 급급하지 않고, 잠재적 리스크 예방과 시스템 확장성에 중점을 두었습니다.

- **데이터 무결성 및 동시성 제어**: 오픈매트 참가 신청 시 발생할 수 있는 동시성 이슈를 고려하여 정원 관리 로직을 설계했습니다.
- **예외 처리 표준화**: 클라이언트가 명확하게 인지할 수 있도록 에러 코드와 응답 규격을 통일성 있게 관리합니다.
- **자동화된 상태 관리**: 스케줄러(Scheduler)를 활용해 종료 시간을 기준으로 오픈매트의 상태(Finished)를 자동 전환하여 운영 리소스를 최소화했습니다.

<br>

## 💻 기술 스택 (Tech Stack)

### Backend
- **Framework**: Java Spring Boot 3.x
- **Database**: MySQL 8.0, Redis (Cache/Session)
- **ORM**: Spring Data JPA + QueryDSL
- **Security**: Spring Security 6.x + JWT (OAuth2)
- **Infra & Storage**: AWS S3, FCM (Firebase Cloud Messaging)
- **Docs**: Swagger / OpenAPI 3.0

### Client (참고)
- **Framework**: Flutter 3.x (Web) / Dart
- **Architecture**: MVVM + GetX 패턴 적용

<br>

<br>

## 👨‍💻 개발자 소개 (About Me)

**"기획 단계부터 데이터 구조적 결함을 파악하고, 사전에 예방하는 백엔드 개발자"**

- **Name**: 철딩 (Cheolding)
- **Email**: xogus2168@gmail.com
- **Blog**: [cheolddings.tistory.com](https://cheolddings.tistory.com/)
- **GitHub**: [github.com/cheolding119](https://github.com/cheolding119)
