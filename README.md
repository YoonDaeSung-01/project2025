# Project 2025 · 생성형 AI 기반 교수·학습 지원 시스템

강의 중 질문 생성, 강의 화면·발화 기록, 주제별 복습 자료, AI 조교 Q&A와 과제 피드백을 연결하는 팀 프로젝트입니다.

## 브랜치 안내

프론트엔드와 백엔드는 **서로 다른 브랜치**에 있습니다. 현재 보고 있는 `main`은 Vue 3 + Bootstrap-Vue 기반 화면 코드입니다.

| 구성 | 브랜치 | 주요 내용 |
|---|---|---|
| 프론트엔드 | [`main`](https://github.com/YoonDaeSung-01/project2025/tree/main) | 교수자·학습자 화면, 브라우저 음성 인식, 강의 화면 캡처 |
| **백엔드** | **[`backend`](https://github.com/YoonDaeSung-01/project2025/tree/backend)** | **FastAPI, PostgreSQL, 강의 요약·질문·과제 피드백 API** |

**[백엔드 README 보기 →](https://github.com/YoonDaeSung-01/project2025/blob/backend/README.md)**

백엔드 개발을 주도한 윤대성의 작업은 `backend` 브랜치에서 확인할 수 있습니다. 해당 README에 주요 구현 코드, 시스템 구조, API 목록, 환경 설정과 현재 재실행 시 확인할 사항을 정리했습니다.

아래는 프론트엔드의 기존 설치·실행 안내입니다. 전체 서비스 연동에는 별도의 백엔드와 DB·AI 설정이 필요합니다.

## 📦 설치 방법

1. 프로젝트 클론 또는 다운로드
2. 터미널에서 프로젝트 폴더로 이동
   ```bash
   cd project2025-main
   ```
3. 필요한 패키지 설치
   ```bash
   npm install
   ```

## 🚀 개발 서버 실행 방법

```bash
npm run serve
```

- 기본 접속 주소: http://localhost:8080

## 🛠 프로덕션 빌드 방법

```bash
npm run build
```

- `dist/` 폴더가 생성됩니다.
- 이 폴더를 웹 서버(AWS S3, Nginx, Netlify 등)에 배포하면 됩니다.

## ⚡ 주의사항

- Node.js 16 ~ 20 버전 권장
- vue-cli-service를 사용합니다.
- 추가 환경변수(.env 파일)가 필요한 경우 별도로 설정해야 합니다.

---

**문의 사항이 있다면 README 하단에 남기세요.**
