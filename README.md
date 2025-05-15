# 📖 Sotlak: 반복하는 자기소개는 이제그만!

## 📱 배포 
[Mufin 이용하기](https://mufin.newlecture.com)

## 📌 프로젝트 개요
"자신만의 프로필 생성 웹 애플리케이션"  

스몰토크는 사회 관계의 유지하는데 도움을 많이 줍니다
20 ~ 30대 "스몰토크" 비중이 높아졌지만 그중에서도 어떻게 대화를 시작해야 할지 또는 반복되는 자기소개에 대한 어려움을 겪고있습니다.
이러한 문제들을 해결하고자 자신만의 프로필 생성을 하여 소통의 도구가 될 수 있는 웹 애플리케이션을 개발하였습니다.

## 개요
타입 스크립트의 대한 이해도와 클린 아키텍처 적용을 위한 학습 프로젝트

## ✨ 주요 기능

### 1️⃣ 자신만의 프로필 생성하기 📝
- **키워드 별 선택하여 자신만의 프로필을 생성할 수 있습니다**  


### 2️⃣ 대화주제 추천하기 🗨️
- **타인들이 주로 대화하는 내용을 모아 사용자에게 추천합니다.**  

### 3️⃣ QR코드를 통해 다른사람 프로필 보기 🤝
- **타인이 생성한 프로필을 직접 확인할 수 있습니다.**  
  현재가와 호가창의 유동성을 시각화한 그래프로 한눈에 확인합니다.

## ❗맡은 기능

### 회원가입 및 로그인 페이지 구현
  - 로그인, 회원가입, 아이디 찾기, 비밀번호 찾기, 정보 수정, 회원 탈퇴 등 다양한 회원관리 기능  React SPA 구조를 기반으로 페이지를 구성
### 이메일 인증 기능 구현
  - Nodemailer + Gmail API로 이메일 인증 코드를 발송하고,  Redis 의 TTL을 활용해 일회성 인증 코드 유효성 관리를 구현
### 개발 환경 구축:
  - 파일 구조, ERD 설계, 공통 컴포넌트 개발 등 개발 환경을 초기에 구축


## 🗨️깨달은점
### 1️⃣ Next.js에서 렌더링 방법
 - styled-components 사용 중 className 불일치 에러를 겪으며,
Next.js는 기본적으로 SSR 방식이기 때문에 스타일도 서버에서 렌더링되도록 처리해야 한다는 점을 깨달았습니다.
이를 통해 SSR 환경에서의 스타일 처리 중요성을 명확히 이해하게 되었습니다.
### 2️⃣ 런타임 환경의 차이점
 - React 컴포넌트 방식으로 이메일을 구성했지만, 이메일 클라이언트에서는 CSS-in-JS나 클래스 기반 스타일이 적용되지 않는 문제를 겪음.
이를 통해 이메일 환경은 일반 브라우저와 다르며, 스타일은 반드시 inline 방식으로 작성해야 한다는 점을 깨달음.
### 3️⃣ Git-Flow 방식 경험
  - GitHub Flow를 처음 적용해보며, 기능 단위 브랜치 전략과 PR 기반 협업의 명확한 흐름을 경험했습니다.
이를 통해 작업 이력 관리의 중요성과 협업 시 안정성 확보 방법을 깨달았습니다.


## 🛠️ 기술 스택

### ⚡ Frameworks & Libraries
| Next.js | TypeScript | React | Styled- <br> Components |
| :---: | :---: | :---: | :---: |
| <img src="https://skillicons.dev/icons?i=nextjs" width="100" height="60" /> | <img src="https://skillicons.dev/icons?i=typescript" width="100" height="60" /> | <img src="https://skillicons.dev/icons?i=react" width="100" height="60" /> | <img src="https://skillicons.dev/icons?i=styledcomponents" width="100" height="60" /> |

### 🖥️ Development Languages
| JavaScript | 
| :---: | 
| <img src="https://skillicons.dev/icons?i=javascript" width="100" height="60" /> |

### 🗄️ Database
| Supabase | Redis |
| :---: | :---: |
| <img src="https://skillicons.dev/icons?i=supabase" width="100" height="60" /> | <img src="https://skillicons.dev/icons?i=redis" width="100" height="60" /> |

### 🏗️ Architecture
| 클린 아키텍처 (DTO, Usecase, Repository 패턴 적용) |
| :---: |

## 📂 폴더 구조
```plaintext
📦 프로젝트 루트
├── 📂 app             # Next.js 15의 App Router 구조 (페이지 & API 핸들러)
├── 📂 application     # UseCase, DTO 등 비즈니스 로직 담당
├── 📂 components      # 공통 컴포넌트
├── 📂 config          # 환경변수 및 설정 파일들
├── 📂 constants       # 프로젝트 상수 정의
├── 📂 domain          # 데이터 영역 담당 계층
├── 📂 infrastructure  # Prisma, Repository, 외부 API 담당 계층
├── 📂 public          # 정적 파일 (이미지, 아이콘 등)
├── 📂 utils           # 공통 유틸리티 함수
└── 📜 README.md       # 프로젝트 설명
```

## 🧑‍🧑‍🧒 프로젝트 구성원
| <img src="https://github.com/ggoldJeongg.png" width="80"> | <img src="https://github.com/getsoss.png" width="80"> | <img src="https://github.com/hyein07100.png" width="80"> | <img src="https://github.com/JunSeGue.png" width="80"> |
| :----------------------------------------------------: | :------------------------------------------------------: | :--------------------------------------------------------: | :------------------------------------------------------: |
|         [박금정](https://github.com/ggoldJeongg)          |         [김재연](https://github.com/getsoss)          |         [손혜인](https://github.com/hyein07100)          |         [전세계](https://github.com/JunSeGue)          |
|                          팀장 및 풀스택 개발자                          |                           팀원 및 풀스택 개발자                        |                            디자이너 및 풀스택 개발자                          |                           CTO 및 풀스택 개발자                         |


## 설치 가이드
1. 저장소 클론: `git clone https://github.com/JunSeGue/sotalk.git`
2. 의존성 설치: `npm install`
3. 실행: `npm run dev`

- ## 문의하기
질문이나 피드백은 [이메일](seogu080@naver.com)로 연락해 주세요.
