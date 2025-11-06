# Labify 🧪
> 연구실 폐기물, 스마트하게 관리하고 간편하게 수거하세요!

Labify는 연구실, 실험실 등에서 발생하는 복잡한 폐기물 처리 과정을 디지털화하여, 폐기물 등록부터 수거 요청, 처리까지의 전 과정을 효율적으로 관리하는 서비스입니다.

<br>

## ✨ 주요 기능
**1. AI 기반 폐기물 분류:** 사용자가 폐기물 이미지를 업로드하면, 외부 AI 서버와 연동하여 폐기물의 종류를 자동으로 인식하고 분류합니다.

**2. QR 코드 기반 추적 시스템:** 등록된 모든 폐기물(DisposalItem)에 고유 QR 코드를 부여합니다. 수거 업체는 QR 스캔만으로 간편하게 수거를 완료하고, 모든 과정은 로그로 기록되어 정확한 추적이 가능합니다.

**3. 체계적인 수거 프로세스:** 실험실 관리자는 앱을 통해 간편하게 수거를 요청(PickupRequest)하고, 수거 업체는 요청 내역을 바탕으로 작업을 배정(Pickup)하고 처리 현황을 실시간으로 업데이트할 수 있습니다.

**4. 역할 기반 사용자 관리:** 실험실 관리자(LAB_MANAGER), 시설 관리자(FACILITY_MANAGER), 수거 업체 직원(PICKUP_MANAGER) 등 다양한 사용자 역할을 구분하여 각 역할에 맞는 권한과 기능을 제공합니다.

**5. 편리한 조회 기능:** '내 실험실 목록', '내가 요청한 수거 내역', '오늘/내일의 수거 일정', '전체 처리 이력' 등 필요한 정보를 API를 통해 쉽게 조회할 수 있습니다.

<br>

## ⚙️ 시스템 아키텍처

```
+--------------+     HTTP     +-----------------------------+     HTTP      +-----------------------+
|              | <----------> |                             | <-----------> |                       |
|  iOS Client  |              |  Spring Boot (Main Server)  |               |  FastAPI (AI Server)  |
|              | <----------> |                             | <-----------> |                       |
+--------------+              +-----------------------------+               +-----------------------+
                                          |
                                          | JDBC
                                          |
                                   +--------------+
                                   |              |
                                   |   MySQL DB   |
                                   |              |
                                   +--------------+
```
                                   
## 🛠️ 기술 스택

| 분야 | 기술 스택 |
|:----:|:-----------|
| **Backend** | ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white) ![Spring Data JPA](https://img.shields.io/badge/Spring%20Data%20JPA-6DB33F?style=for-the-badge&logo=spring&logoColor=white) ![Spring Security](https://img.shields.io/badge/Spring%20Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white) ![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white) |
| **Frontend** | ![SwiftUI](https://img.shields.io/badge/SwiftUI-FA7343?style=for-the-badge&logo=swift&logoColor=white) |
| **AI Server** | ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) |


<br>

## 👥 팀원

| <img src="https://github.com/ownue.png" width="100" height="100"> | <img src="https://github.com/spacefoul.png" width="130" height="130"> | <img src="https://github.com/nayun0724.png" width="130" height="130"> | <img src="https://github.com/romdyfo.png" width="130" height="130"> | <img src="https://github.com/user-attachments/assets/47a3e6ac-39a3-41c8-bfa0-75f7b62be8ee" width="130" height="130"> |
|:---:|:---:|:---:|:---:|:---:|
| **이은우** | **강예현** | **권나윤** | **김지희** | **임혜린** |
| 팀장 / 백엔드 개발 | 프론트엔드 개발 | AI 개발 | 백엔드 개발 | 디자이너 |
| <a href="https://github.com/ownue"><img src="http://img.shields.io/badge/ownue-green?style=social&logo=github"/></a> | <a href="https://github.com/spacefoul"><img src="http://img.shields.io/badge/spacefoul-green?style=social&logo=github"/></a> | <a href="https://github.com/nayun0724"><img src="http://img.shields.io/badge/nayun0724-green?style=social&logo=github"/></a> | <a href="https://github.com/romdyfo"><img src="http://img.shields.io/badge/romdyfo-green?style=social&logo=github"/></a> | [Portfolio](#) |
