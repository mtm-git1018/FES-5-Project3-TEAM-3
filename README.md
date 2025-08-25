<div align="center">

# 🍷 Winepedia

와인을 좋아하는 사람들을 위한 **정보 · 리뷰 · 커뮤니티 플랫폼**
Supabase 기반의 데이터 관리와 인증을 지원하며,
검색 / 리뷰 / 취향분석 / 커뮤니티 기능을 제공합니다.
</div>


## 📑 목차
1. [🚀 프로젝트 개요](#-프로젝트-개요)
2. [🎨 프로젝트 디자인](#-프로젝트-디자인)
3. [🛠️ 기술 스택](#️-기술-스택)
4. [📂 폴더 구조](#-폴더-구조)
5. [🌱 개발 컨벤션](#-개발-컨벤션)

---

## 🚀 프로젝트 개요

- **프로젝트명** : Winepedia
- **목적** : 와인 정보 검색 및 커뮤니티 기반 리뷰/소통 플랫폼 개발
- **주요 기능** :
  - 🍇 와인 검색 및 필터링 (국가, 도수, 당도, 맛 등)
  - ✍️ 와인 상세 페이지 및 리뷰 작성
  - 💬 커뮤니티 (질문, 리뷰, 자유글 작성/검색/필터링)
  - 🧑‍💻 마이페이지 (내 리뷰, 위시리스트, 활동 내역)
  - 🔐 Supabase 기반 DB 관리 및 유저 인증
---

## 🛠️ 기술 스택

| 영역 | 기술 |
|------|------|
| **Framework** | Vite + React + TypeScript |
| **Styling** | TailwindCSS |
| **State Management** | Zustand |
| **Routing** | React Router v7+ (data mode) |
| **Lint / Format** | ESLint + Prettier |
| **Animation** | GSAP / Framer Motion |
| **Database & Auth** | Supabase |
| **Alert** | React Toastify |
| **Deployment** | Vercel |
---

## 📂 폴더 구조

```bash
public
 ├── icon
 └── image

src
 ├── @types/        # 타입 정의(global.d.ts 등)
 ├── assets/        # 정적 파일
 ├── components/    # 공통 컴포넌트
 ├── data/          # 데이터(json) or supabase 연동
 ├── pages/         # 라우트 페이지 (Home.tsx 등)
 ├── hook/         # 커스텀 훅
 ├── router/        # routes.tsx
 ├── styles/        # 공통 CSS
 ├── utils/         # 유틸 함수 (tw.ts, fetchUser.ts 등)
 └── supabase/      # supabase 관련 타입/설정

```

---

 ## 🌱 개발 컨벤션

### 🔹 Git 전략
- **브랜치 구조** : `main` → `dev` → `feature/bug`
- **Merge 규칙** : 큰 기능 단위 및 버그 수정 후 `main`으로 merge
- **배포** : 중간 단계에서 최소 1회 이상 진행


### 🔹 Branch 네이밍
- 규칙 : `[feature] ComponentName_Nickname`
  - 예시 : `[feature] Header_EJ`
- 브랜치 태그 종류 :
  - ✨ **feature** : 기능 개발
  - 🐛 **fix** : 버그 수정
  - 🔧 **chore** : 배포, 라이브러리 작업 등
  - 📄 **docs** : 문서 작업 (README 등)
  - 🎨 **style** : CSS 수정, 코드 포맷 변경
  - 💬 **comment** : 주석 추가/수정


### 🔹 PR 규칙
- Issue 단위로 PR 생성
- PR 올리기 전 반드시 dev 최신본 pull → 충돌 해결 후 merge
- 최소 1명 승인 필요


### 🔹 네이밍 규칙
- className → camelCase
- Component → PascalCase
