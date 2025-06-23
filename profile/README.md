<div align="center">

# 🚗 MODiVE


<p align="center">
  <b>클라우드 기반 차량 데이터 분석 플랫폼으로<br/>
  운전자의 주행 습관을 MOBTI로 분석하여 개인화된 피드백을 제공하는 스마트 모빌리티 서비스</b>
</p>

[프로젝트 소개](#-프로젝트-소개) •
[주요 기능](#-주요-기능) •
[기술 스택](#-기술-스택) •
[아키텍처](#-시스템-아키텍처) •
[시작하기](#-시작하기) •
[팀 정보](#-팀-정보)

</div>

---

## 📋 프로젝트 소개

**MODiVE**는 CARLA 시뮬레이터와 AWS 클라우드를 활용하여 차량 주행 데이터를 실시간으로 수집·분석하고, 운전자에게 맞춤형 피드백을 제공하는 혁신적인 플랫폼입니다.

### 🎯 핵심 목표

- 🚙 **데이터 기반 운전 습관 분석**: CARLA 시뮬레이터를 통한 정밀한 주행 데이터 수집
- ☁️ **클라우드 네이티브 설계**: AWS 서비스를 활용한 확장 가능한 아키텍처
- 🧬 **MOBTI 분석 시스템**: MBTI처럼 운전 성향을 16가지 유형으로 분류
- 🤖 **AI 피드백**: LLM 기반 개인 맞춤형 운전 습관 개선 제안
- 🌱 **사회적 가치 창출**: 안전 운전 유도 및 탄소 중립 실천

### 📅 프로젝트 기간
> 2025.04.12 ~ 2025.06.20

---

## ✨ 주요 기능

<table>
<tr>
<td width="50%">

### 🎭 운전 MBTI (MoBTI)
운전 습관을 4가지 지표로 분석하여 16가지 성향으로 분류
- **E**co vs **H**eavy (연비/탄소배출)
- **A**ggressive vs **D**efensive (안전운전)
- **S**ensitive vs **I**nsensitive (사고예방)
- **F**ocused vs **D**istracted (주의력)

</td>
<td width="50%">

### 🤖 LLM 맞춤형 피드백
Gemini API를 활용한 지능형 운전 코칭
- 개인 관심사 기반 피드백
- 자연어 리포트 자동 생성
- 운전 습관 개선 제안

</td>
</tr>
<tr>
<td width="50%">

### 🚨 실시간 위험 감지
Apache Flink 기반 실시간 이벤트 처리
- 과속, 급가속/급제동 감지
- 차선이탈, 안전거리 경고
- 즉각적인 음성/푸시 알림

</td>
<td width="50%">

### 🌱 리워드 시스템
안전 운전 습관 형성을 위한 인센티브
- 씨앗 포인트 적립
- 미션 기반 보상
- 운전 성향 개선 보너스

</td>
</tr>
</table>

---

## 🛠 기술 스택

### Frontend
![React Native](https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)

### Backend
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

### Infrastructure & Cloud
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white)
![Apache Flink](https://img.shields.io/badge/Apache_Flink-E6526F?style=for-the-badge&logo=apache-flink&logoColor=white)

### Data & Simulation
![CARLA](https://img.shields.io/badge/CARLA-000000?style=for-the-badge&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAA4SURBVHjaYvz//z8DOYCJgUxAtkYWZIGMjIz/GRkZGcjRyEKOJrI1orsFq0ayNWI1kBhNoxYCADbZBgzxfEwiAAAAAElFTkSuQmCC)
![Kinesis](https://img.shields.io/badge/AWS_Kinesis-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)
![DynamoDB](https://img.shields.io/badge/DynamoDB-4053D6?style=for-the-badge&logo=amazon-dynamodb&logoColor=white)

---

## 🏗 시스템 아키텍처
![Image](https://github.com/user-attachments/assets/bb5fece9-0a6f-48d3-8b0d-96f334ded85c)

### 🔧 마이크로서비스 구조
![Image](https://github.com/user-attachments/assets/5678f897-9ceb-41b4-b9ba-cc3c1896440d)

| Service | Description | Tech Stack |
|---------|-------------|------------|
| 🔐 **auth-service** | 사용자 인증 및 권한 관리 | Spring Security, JWT |
| 👤 **user-service** | 사용자 정보 관리 | Spring Boot, JPA |
| 📊 **dashboard-service** | 대시보드 데이터 처리 | Spring Boot, Redis |
| 📈 **analysis-service** | 주행 데이터 분석 | Python, Pandas |
| 🎁 **reward-service** | 리워드 시스템 관리 | Spring Boot |
| 🤖 **llm-service** | AI 피드백 생성 | Python, Gemini API |
| 🤝 **agent-service** | AI 에이전트 관리 | Spring Boot |

---

## 🚀 시작하기

### Prerequisites

- Docker & Docker Compose
- AWS CLI configured
- Node.js 18+
- Java 17+
- Python 3.9+

### Repository Structure

```bash
LGCNS-Final-PJT-Team5/
├── 📁 Carla/              # CARLA 시뮬레이터 연동
├── 📁 FE/                 # 모바일 앱 (React Native)
├── 📁 admin-web/          # 관리자 웹 (React)
├── 📁 BE/                 # 백엔드 통합
├── 📁 auth-service/       # 인증 서비스
├── 📁 user-service/       # 사용자 서비스
├── 📁 dashboard-service/  # 대시보드 서비스
├── 📁 analysis-service/   # 분석 서비스
├── 📁 reward-service/     # 리워드 서비스
├── 📁 llm-service/        # LLM 서비스
├── 📁 agent-service/      # 에이전트 서비스
└── 📁 Resources/          # 프로젝트 리소스
```

## 👥 팀 정보

### LG CNS AM Inspire Camp 1기 - Team 5

| **이슬아** | **구영민** | **최진실** | **김민중** |
| :------: |  :------: | :------: | :------: |
| [<img src="https://avatars.githubusercontent.com/u/150000000?v=4" height=150 width=150> <br/> @SRASONY](https://github.com/SRASONY) | [<img src="https://avatars.githubusercontent.com/u/150000001?v=4" height=150 width=150> <br/> @rndudals](https://github.com/rndudals) | [<img src="https://avatars.githubusercontent.com/u/150000002?v=4" height=150 width=150> <br/> @jinsil296](https://github.com/jinsil296) | [<img src="https://avatars.githubusercontent.com/u/150000003?v=4" height=150 width=150> <br/> @minjooong](https://github.com/minjooong) |
| **Team Leader** | **Backend Developer** | **Frontend Developer** | **Backend Developer** |

| **신예빈** | **구도희** | **황지민** | **류동현** |
| :------: |  :------: | :------: | :------: |
| [<img src="https://avatars.githubusercontent.com/u/91859242?v=4" height=150 width=150> <br/> @ShinYEB](https://github.com/ShinYEB) | [<img src="https://avatars.githubusercontent.com/u/150000005?v=4" height=150 width=150> <br/> @peachoe](https://github.com/peachoe) | [<img src="https://avatars.githubusercontent.com/u/150000006?v=4" height=150 width=150> <br/> @jiminh00](https://github.com/jiminh00) | [<img src="https://avatars.githubusercontent.com/u/150000007?v=4" height=150 width=150> <br/> @Ryu1216](https://github.com/Ryu1216) |
| **Backend Developer** | **Backend Developer** | **Cloud Engineer** | **Frontend Developer** |
<table>
<tr>
<td align="center">

**🏢 Organization**

[LGCNS-Final-PJT-Team5](https://github.com/LGCNS-Final-PJT-Team5)


</td>
</tr>
</table>

### 🤝 Contributing

이 프로젝트는 LG CNS AM Inspire Camp 1기의 최종 프로젝트입니다.
