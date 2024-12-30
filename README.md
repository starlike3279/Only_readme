# 금융 교육 & 사용자 맞춤 ETF 추천 플랫폼

<!--배지-->
![Repository Size][repository-size-shield] ![Issue Closed][issue-closed-shield]

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

* ❗️제작 동기❗️
  - 가계부채 증가, 저금리 기조, 부동산 및 주식 등 자산 시장 변동성이 커지면서, 개인이 금융지식 없이 자산을 운용하기 점점 어렵고 위험해지고 있음
  - 금융 교육을 통해 합리적 소비와 투자, 리스크 관리, 올바른 재무 목표 설정 등을 익힘으로써 개인의 재정 건전성을 높이고 사회 전반의 금융 안정성을 도모할 수 있음
  - 최근 주식, ETF 시장에 대한 관심이 높아지고 있지만, 정작 개인 투자자들 중에는 자신만의 투자 성향을 명확히 인지하지 못한 채 트렌드만 쫒아 매매하는 경우가 많음
  - 이는 불필요한 손실을 유발하거나, 장기적인 투자 목표 설정에 어려움을 겪게 만드는 원인이 됨
  - 사용자의 투자 성향을 분석하여 맞춤형 ETF를 추천해주어 이러한 문제를 해결하고 더 나아가 지속 가능한 투자 활동을 돕는 것이 본 프로젝트의 제작동기임

## 프로젝트 설명
  - 기본적으로 제공하는 퀴즈를 기반으로 지식을 쌓을 수 있음
  - 사용자가 직접 원하는 대로 퀴즈를 생성하고 수정할 수 있음 
  - 투자성향분석 설문을 바탕으로 자신의 투자성향을 파악하고 맞춤형 ETF를 추천해줌

## 개발 기간
  - 2024.11.11 ~ 2024.12.20

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

* Version Control
  - Github
  - Git
    
* Backend Technologies
  - Java
  - SpringBoot
    
* FrontEnd Technologies
  - HTML5
  - CSS3
  - React
  - Fetch API
  - Swiper Library

# [2] 팀원 & 역할분담


## 개발 팀원 & 역할 분담

- 임재혁(팀원)

  * UI

  1) 퀴즈
     
     - 퀴즈 조회
     - 인기 퀴즈
     - 사용자별 퀴즈 등록
     - 퀴즈 수정
     - 퀴즈 삭제
  
- 장준규(팀원)

  * UI
    
    - 회원가입 페이지
    - 로그인 페이지
    - 아이디, 비밀번호 찾기 페이지
    - 프로필 페이지
    - Nav 바

  1) 회원

     - 회원가입
     - 일반 로그인
     - 아이디 찾기
     - 비밀번호 찾기
     - 로그아웃
     - 로그인 갱신(30분)

  2) 프로필

     - 투자성향 MBTI 조회
     - 썸네일 이미지 등록/조회/수정
     - 자기소개 조회/수정
     - 닉네임 조회/수정
     
- 한태호(팀장)

  * UI

    - 메인 페이지
    - 전체 ETF 조회 페이지
    - ETF 상세 페이지
    - ETF 상세 비교 팝업 창
    - 투자성향분석 MBTI 팝업 창
    - 투자성향분석 결과 페이지

  1) ETF
     
     - ETF 조회, 검색
     - ETF 상세 비교
     - ETF 즐겨찾기 등록, 삭제
     - 투자성향 MBTI 설문 결과에 따른 맞춤 ETF 추천(NAV, ETF 현재가격 활용)
     - ETF 등락률 순위 조회
     - ETF 기본 정보 및 구성종목 상세 조회

  2) 투자성향 분석
 
     - 투자성향 MBTI 분석
     - 투자성향 MBTI 1일 2회 제한

# [3] 문서

## ERD
- https://www.erdcloud.com/d/jivZFQrf2wXvugu2Q

## 요구사항 정의서
- https://docs.google.com/spreadsheets/d/13flPhRkAohFWRyeVgpO6fK2K0rhyp3mD/edit?usp=sharing&ouid=114994970396661234746&rtpof=true&sd=true

## 요구사항 기획서
- https://docs.google.com/document/d/1uyWmLjlEamgZz6NCSunFm4GFJRT1n7Vc/edit?usp=sharing&ouid=114994970396661234746&rtpof=true&sd=true

## 와이어프레임
- https://www.figma.com/design/IYYwOXqcTOrugz7xzfTeiS/Fund-Find?node-id=0-1&t=IdCUjNJuED7oRxFM-1

## DFD
- https://www.figma.com/board/eFCqOQvEn6oGs17G7hX7LP/Fund-Find?node-id=0-1&t=ISUhGe4DFFLt1AXA-1


# [4] 주요 기능
이 프로젝트의 기여하신 분들을 소개합니다! 🙆‍♀️

## 회원

## 금융퀴즈

## ETF


# [5] 페이지별 기능
***유사한 프로젝트의 레포지토리** 혹은 **블로그 포스트** 등 프로젝트 구현에 영감을 준 출처에 대해 링크를 나열하세요.*

## 기능 1

## 기능 2

## 기능 3

# [6] 트러블 슈팅
- 📧 dev.ujin518@gmail.com
- 📋 [https://dev-ujin.github.io/contact](https://dev-ujin.github.io/contact)


# [7] 개선 목표

* 임재혁

  - 1 
  - 2
  - 3

* 장준규

  - 1 
  - 2
  - 3

* 한태호

  - 1 메인 페이지 디자인 및 CSS 수정 
  - 2 전체 ETF 로딩시간 단축
  - 3 코드 가독성 향상

# [8] 프로젝트 후기

## 1 임재혁

## 2 장준규

## 3 한태호




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


