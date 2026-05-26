# 🥾 세lab — 강원도 도보 관광 루트 서비스

> **"이동 자체가 여행이 된다"** — 시간 단위로 최적화된 도보 루트로 강원도를 깊이 있게 경험하세요.

---

## 🗺️ 프로젝트 소개

**세lab**은 2026 관광데이터 활용 공모전 웹·앱 개발 부문 출품작입니다.

기존 관광 서비스가 **명소 중심 정보 제공**에 그치는 한계를 넘어,  
사용자의 가용 시간과 체력에 맞는 **도보 루트 기반 슬로우 관광** 경험을 제공합니다.  
스페인 산티아고 순례길처럼 — **걷는 과정 자체가 여행의 목적**이 되는 서비스입니다.

<p align="center">
  <img src="https://github.com/user-attachments/assets/bcfd001d-3d27-43d3-a0cd-e1cd8770ce84" alt="강원의 길 앱 미리보기" width="700" />
</p>


---

## 🎯 핵심 기능

| 기능 | 설명 |
|------|------|
| ⏱️ 시간 기반 루트 추천 | 가용 시간(30분 ~ 1일+)에 맞게 최적화된 도보 코스 |
| 🚶 순례형 관광 코스 | 강원도 전역을 연결하는 장거리 도보 루트 |
| 🗺️ 실시간 루트 탐색 | 관광지 간 도보 동선 + 소요 시간 안내 |
| ⭐ 사용자 리뷰/평점 | 리뷰·이용 패턴 기반 맞춤 추천 |
| 🏃 러닝/트레킹 모드 | 러닝크루 기능 및 운동 데이터 연동 |

---

## 📡 활용 데이터

한국관광공사 OpenAPI를 핵심 데이터 소스로 활용합니다.

- **국문 관광정보 서비스** — 관광지 기본 정보 및 루트 구성
- **두루누비 (걷기 여행길) 정보 서비스** — 기존 걷기 코스 기반 루트 최적화, 거리·소요 시간 데이터
- **관광지별 연관 관광지 정보** — 자연스러운 이동 경로 및 스토리형 루트 생성

---

## 🏗️ 기술 스택

### Frontend
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)

- Flutter (iOS / Android 크로스 플랫폼)

### Backend
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)

- Spring Boot — REST API 서버
- PostgreSQL — 관광지·루트·사용자 데이터 관리

### Infrastructure
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)

- AWS (EC2, RDS, S3 등)

### Architecture Overview

```
[Flutter App]
     │
     ▼
[Spring Boot API Server]  ←──→  [한국관광공사 OpenAPI]
     │
     ▼
[PostgreSQL on AWS RDS]
```

---

## 📁 리포지토리 구성

| 리포지토리 | 설명 |
|-----------|------|
| `FrontEnd` | Flutter 앱 (iOS/Android) |
| `Backend` | Spring Boot REST API 서버 |
| `infra` | AWS 인프라 구성 (IaC) |

---

## 🚀 향후 발전 방향

- 🌏 **전국 확장** — 강원도 → 전국 관광지, 도시형 산책 루트 (서울·광역시)
- 🤖 **AI 개인화 추천** — 이동 패턴 분석 기반 맞춤 루트 자동 생성
- 🛍️ **지역 상권 연계** — 카페·식당·숙소와 연결해 지역 경제 활성화
- 🌍 **글로벌 확장** — 외국인 관광객 대상 한국 도보 여행 콘텐츠

---

## 👥 팀

**세lab** — 2026 관광데이터 활용 공모전 참가팀

---

<p align="center">
  <sub>한국관광공사 OpenAPI를 활용하여 개발되었습니다.</sub>
</p>
