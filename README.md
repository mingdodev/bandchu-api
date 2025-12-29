# BandChu API Server

[![language](https://img.shields.io/badge/Language-Kotlin%202.2.21-7F52FF)](https://kotlinlang.org/docs/whatsnew2221.html)
[![framework](https://img.shields.io/badge/Framework-Spring%20Boot%203.5.7-6DB33F)](https://spring.io/projects/spring-boot)
[![orm](https://img.shields.io/badge/ORM-Exposed-7952B3)](https://github.com/JetBrains/Exposed)
[![db](https://img.shields.io/badge/Database-PostgreSQL-336791)](https://www.postgresql.org/)
[![test](https://img.shields.io/badge/Testing-Kotest-B84E0F)](https://kotest.io/)
[![build](https://img.shields.io/badge/Build-Gradle-02303A)](https://gradle.org/)

<br>

## 📄 공유 문서

- [API 명세](./docs/API_SPEC.md)
- [협업 가이드](./docs/TEAM_GUIDE.md)

<br>

## 📂 디렉토리 구조

```
   api
    ├── domain
    │   ├── member
    │   └── post
    │       ├── dto
    │       ├── controller
    │       ├── service
    │       ├── repository
    │       └── model
    ├── global
    │   ├── config
    │   ├── exception
    │   ├── response
    │   └── ...
    └── ApiApplication
```

<br>

## 📚 데이터베이스 스키마

![ERD](docs/assets/erd.png)

<br>

## ⚙️ 환경 변수 설정

```properties
# 데이터베이스 설정
DB_URL=jdbc:postgresql://localhost:5432/bandchu
DB_USERNAME=your_db_username
DB_PASSWORD=your_db_password

# Google OAuth 설정
GOOGLE_CLIENT_ID=your_google_client_id

# AWS Credential 설정
AWS_CREDENTIAL_ACCESS_KEY=your_aws_access_key
AWS_CREDENTIAL_SECRET_KEY=your_aws_secret_key
```
- **DB_URL**: PostgreSQL 데이터베이스 연결 URL
- **DB_USERNAME**: 데이터베이스 사용자 이름
- **DB_PASSWORD**: 데이터베이스 비밀번호
- **GOOGLE_CLIENT_ID**: Google OAuth 2.0 클라이언트 ID (Google Cloud Console에서 발급)
- **AWS_CREDENTIAL_ACCESS_KEY / SECRET_KEY**: AWS S3 접근을 위한 IAM 사용자 키

<!--
<br>

## 🛠️ Server Architecture
-->
