## 📚 AIVLE Book Manager – 전체 프로젝트 소개
AIVLE SCHOOL 6반 17조가 개발한 도서 관리 웹 애플리케이션입니다. 이 프로젝트는 사용자가 도서를 등록하고, OpenAI DALL·E API를 통해 책 표지를 자동 생성할 수 있도록 구성된 웹 서비스입니다.
---
###📌 프로젝트 개요
| 구분 | 설명 |
| :---- | :-------------------------------------------------------------------------------------------------------------------------------- |
| 프로젝트명 | **AIVLE Book Manager** |
| 목적 | 도서 등록/수정/조회 및 AI 기반 커버 이미지 생성 |
| 주요 기능 | 도서 CRUD, DALL·E 3 기반 이미지 생성, 사용자 키 입력 방식 |
| 프론트엔드 | React + MUI (Vite 기반) |
| 백엔드 | Express.js (or Spring Boot 등) |
| AI 연동 | OpenAI DALL·E API 사용 |
---
###🧑‍🤝‍🧑 팀 구성
| 이름 | 역할 요약 |
|---|---|
| 박재현 | PM 프론트 메인페이지 구현 및 AI 표지 생성 기능 구현 및 전체 아키텍처 관리 |
| 김동희 | 백엔드 BookController구현 및 API 단위 테스트(Postman) |
| 김재홍 | 백엔드코드 통합 및 관리, BookServiceImpl, 구현 DTO, 예외처리 |
| 박소현 | 프론트엔드 도서 상세/삭제 기능 View_book.html과 Delete_Book.html 목업 기능 구현 |
| 윤용선 | 백엔드 Book개체 정의, BookService 및 BookRepository 인터페이스 정의 |
| 이유진 | 프론트엔드 View Details, Edit, Delete 버튼 기능 연동, 목록 관련 상태 관리 및 API 호출 |
| 이은수 | 프론트엔드도서 등록 페이지 (BookCreate.jsx) 구현, 도서 수정 페이지 (BookEdit.jsx) 구현, AI 표지 생성 기능 구현 |
| 정유라 | 프론트엔드 도서 목록 기능 All_books.html 목업을 React로 변환 및 기능 구현 |
---
###🛠️ 기술 스택
| 구분 | 기술 |
|---|---|
| **Frontend** | React, Vite, MUI, Axios |
| **Backend** | Spring Boot, h2-console 또는 Postman |
| **AI API** | OpenAI DALL·E 3 (v1/images/generations) |
| **기타** | RESTful API, JSON, Git, GitHub |
---
###🔐 AI 기능 (DALL·E 3 이미지 생성)
사용자가 제목과 줄거리를 입력하면, 해당 내용을 바탕으로 3D 스타일 책 표지 이미지를 생성
DALL·E 3 모델을 직접 호출 (model: "dall-e-3")
사용자가 입력한 OpenAI API 키를 직접 사용 (보안상 서버에 저장 X)
생성된 이미지 URL을 도서 데이터에 포함해 저장
---
### 🧪 실행 방법

#### 1. 프론트엔드

```bash
cd frontend
npm install
npm run dev
```

#### 2. 백엔드

```bash
cd backend
build.gradle 실행
LibraryManagementApplication 실행
```
---
### 📄 하위 README 파일

| 위치                                         | 설명                       |
| ------------------------------------------ | ------------------------ |
| [Project/README.md](https://github.com/4mini-project/4project/blob/main/README.md) | 소스 코드 및 구현 페이지 상세 안내 |
---
