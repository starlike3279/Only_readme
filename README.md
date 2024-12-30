# 금융 교육 & 사용자 맞춤 ETF 추천 플랫폼

<!--배지-->
![Repository Size][repository-size-shield] ![Issue Closed][issue-closed-shield]

<!--프로젝트 대문 이미지-->
![Project Title](img/.png)

<!--목차-->
# 목차
- [[1] 프로젝트 설명](#1-프로젝트_설명)
  - [프로젝트 설명](#프로젝트_설명)
  - [개발 기간](#개발_기간)
  - [개발 환경](#개발_환경)
  - [기술 스택](#기술_스택)
- [[2] 팀원 & 역할분담](#2-팀원_역할분담)
  - [개발 팀원](#개발_팀원)
  - [역할 분담](#역할분담)
- [[3] 문서](#3-문서)
  - [ERD](#ERD)
  - [요구사항 정의서](#요구사항_정의서)
  - [요구사항 기획서](#요구사항_기획서)
  - [와이어프레임](#와이어프레임)
  - [DFD](#DFD)
- [[4] 주요 기능](#4-주요_기능)
  - [회원](#회원)
  - [금융 퀴즈](#금융_퀴즈)
  - [ETF](#ETF)
- [[5] 페이지별 기능](#5-페이지별_기능)
  - [](#)
  - [](#)
  - [](#)
  - [](#)
  - [](#)
- [[6] 트러블 슈팅](#6-트러블_슈팅)
  - [](#)
  - [](#)
  - [](#)
  - [](#)
  - [](#)
- [[7] 개선 목표](#7-개선_목표)
  - [](#)
  - [](#)
  - [](#)
- [[8] 프로젝트 후기](#7-프로젝트_후기)
  - [](#)
  - [](#)
  - [](#)

# [1] 프로젝트 설명
*다음 내용을 고려하여 프로젝트에 대한 **전반적인 정보**를 적으세요.*

- ❗️제작 동기❗️
- 가계부채 증가, 저금리 기조, 부동산 및 주식 등 자산 시장 변동성이 커지면서, 개인이 금융지식 없이 자산을 운용하기 점점 어렵고 위험해지고 있음
- 금융 교육을 통해 합리적 소비와 투자, 리스크 관리, 올바른 재무 목표 설정 등을 익힘으로써 개인의 재정 건전성을 높이고 사회 전반의 금융 안정성을 도모할 수 있음
- 최근 주식, ETF 시장에 대한 관심이 높아지고 있지만, 정작 개인 투자자들 중에는 자신만의 투자 성향을 명확히 인지하지 못한 채 트렌드만 쫒아 매매하는 경우가 많음
- 이는 불필요한 손실을 유발하거나, 장기적인 투자 목표 설정에 어려움을 겪게 만드는 원인이 됨
- 사용자의 투자 성향을 분석하여 맞춤형 ETF를 추천해주어 이러한 문제를 해결하고 더 나아가 지속 가능한 투자 활동을 돕는 것이 본 프로젝트의 제작동기임

## 프로젝트 설명
*강조하고 싶은 **주요 기능**이나 **차별성 있는 특징**을 적으세요.*
- 기본적으로 제공하는 퀴즈를 기반으로 지식을 쌓을 수 있음
- 사용자가 직접 원하는 대로 퀴즈를 생성하고 수정할 수 있음 
- 투자성향분석 설문을 바탕으로 자신의 투자성향을 파악하고 맞춤형 ETF를 추천해줌

## 개발 기간
2024.11.11 ~ 2024.12.20

## 개발 환경
***언어, 프레임워크, 주요 라이브러리**를 **버전**과 함께 나열하세요.*

* 환경 & IDE
- 운영체제 : window 11
- Intellij
- Visual Studio Code
- Dbeaver
- Docker Desktop
- Postman

* Version
- openjdk version: 17.0.13 
- Gradle JVM: corretto-17(Amazon Corretto 17.0.13)
- SpringBoot version: 3.3.5
- spring.dependency-management plugin version: 1.1.6

* DB
- postgreSQL version -> 17.0
- DB PORT: 5433
- DB username: ff_dev
- 데이터베이스 이름 : ff_dev

## 기술 스택
- Version Control
  Github, Git
- Backend Technologies
  Java, SpringBoot
- FrontEnd Technologies
  HTML5, CSS3, React, Fetch API, Swiper 라이브러리

# [2] 팀원 & 역할분담
*만약 운영체제에 따라 프로그램을 다르게 동작시켜야한다면, 운영체제별로 동작 방법을 설명하세요*

## 개발 팀원
*프로젝트를 동작시키기 위해 필요한 소프트웨어와 라이브러리를 나열하고 어떻게 다운받을 수 있는지 설명하세요.*

- [OpenWeather API key](https://openweathermap.org/) (무료)
- npm
```bash
npm install npm@latest -g
```

## 역할분담
*어떻게 이 프로젝트의 소스코드를 다운받을 수 있는지 설명하세요.*
1. Repository 클론
```bash
git clone https://github.com/your-username/project-repository
```
2. NPM packages 설치
```bash
npm install
```

## Configuration
*코드의 어느 부분을 채우거나 수정해야하는지 설명하세요.*
- `config.js`에 Openweather API key를 입력
```bash
const API_KEY = "<Your API key>";
```



# [3] 문서
***스크린샷, 코드** 등을 통해 **사용 방법**과 **사용 예제**를 보여주세요. 사용 예제별로 h2 헤더로 나누어 설명할 수 있습니다.*

![usage](img/usage.png)

```java
// 몇 개의 API 사용 예제를 코드와 함께 보여주세요.
```

## ERD

## 요구사항 정의서

## 요구사항 기획서

## 와이어프레임

## DFD


# [4] 주요 기능
기여해주신 모든 분들께 대단히 감사드립니다.[`contributing guide`][contribution-url]를 참고해주세요.
이 프로젝트의 기여하신 분들을 소개합니다! 🙆‍♀️
*이모티콘 쓰는 것을 좋아한다면, 버그 수정에 🐞, 아이디어 제공에 💡, 새로운 기능 구현에 ✨를 사용할 수 있습니다.*
- 🐞 [dev-ujin](https://github.com/dev-ujin): 메인페이지 버그 수정

## 회원

## 금융퀴즈

## ETF


# [5] 페이지별 기능
***유사한 프로젝트의 레포지토리** 혹은 **블로그 포스트** 등 프로젝트 구현에 영감을 준 출처에 대해 링크를 나열하세요.*

- [Readme Template - Embedded Artistry](https://embeddedartistry.com/blog/2017/11/30/embedded-artistry-readme-template/)
- [How to write a kickass Readme - James.Scott](https://dev.to/scottydocs/how-to-write-a-kickass-readme-5af9)
- [Best-README-Template - othneildrew](https://github.com/othneildrew/Best-README-Template#prerequisites)
- [Img Shields](https://shields.io/)
- [Github Pages](https://pages.github.com/)

## 기능 1

## 기능 2

## 기능 3

# [6] 트러블 슈팅
- 📧 dev.ujin518@gmail.com
- 📋 [https://dev-ujin.github.io/contact](https://dev-ujin.github.io/contact)



# [7] 개선 목표
## 1
## 2
## 3

# [8] 프로젝트 후기
## 1
## 2
## 3

MIT 라이센스
라이센스에 대한 정보는 [`LICENSE`][license-url]에 있습니다.



<!--Url for Badges-->
[license-shield]: https://img.shields.io/github/license/dev-ujin/readme-template?labelColor=D8D8D8&color=04B4AE
[repository-size-shield]: https://img.shields.io/github/repo-size/dev-ujin/readme-template?labelColor=D8D8D8&color=BE81F7
[issue-closed-shield]: https://img.shields.io/github/issues-closed/dev-ujin/readme-template?labelColor=D8D8D8&color=FE9A2E

<!--Url for Buttons-->
[readme-eng-shield]: https://img.shields.io/badge/-readme%20in%20english-2E2E2E?style=for-the-badge
[view-demo-shield]: https://img.shields.io/badge/-%F0%9F%98%8E%20view%20demo-F3F781?style=for-the-badge
[view-demo-url]: https://dev-ujin.github.io
[report-bug-shield]: https://img.shields.io/badge/-%F0%9F%90%9E%20report%20bug-F5A9A9?style=for-the-badge
[report-bug-url]: https://github.com/dev-ujin/readme-template/issues
[request-feature-shield]: https://img.shields.io/badge/-%E2%9C%A8%20request%20feature-A9D0F5?style=for-the-badge
[request-feature-url]: https://github.com/dev-ujin/readme-template/issues

<!--URLS-->
[license-url]: LICENSE.md
[contribution-url]: CONTRIBUTION.md
[readme-eng-url]: ../README.md


