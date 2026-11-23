# 🧊 fridge-raid — 냉장고 털이 레시피봇

> 남은 재료로 오늘 뭐 먹지? 냉장고 사진이나 재료를 입력하면 AI가 만들 수 있는 레시피를 추천해 줍니다.

## ✨ 주요 기능
- 📸 **사진으로 재료 인식** — 냉장고·식재료 사진에서 재료 자동 추출
- 🍳 **레시피 추천** — 가진 재료 기준으로 부족한 재료가 적은 메뉴 우선 추천 (시간·난이도·종류·기피 재료 필터)
- 💬 **레시피봇 채팅** — 재료 대체, 인분 조절, 맛 조절 질문
- ❤️ **즐겨찾기** / 🛒 **장보기 목록**

## 🛠 기술 스택
| 영역 | 기술 |
|---|---|
| Frontend | Next.js (설계 후 설치 예정) |
| Backend | Spring Boot (설계 후 설치 예정) |
| AI | LLM API (키는 백엔드에서만 관리) |

## 📁 프로젝트 구조
```
fridge-raid/
├── .github/
│   └── pull_request_template.md   # PR 템플릿
├── docs/
│   ├── adr/                       # 설계 결정 기록 (Architecture Decision Records)
│   └── prompts/                   # AI 프롬프트 버전 관리
├── frontend/                      # Next.js 앱
├── backend/                       # Spring Boot 서버
├── .editorconfig
├── .gitignore
└── README.md
```

## 👥 팀
| 이름 | 역할 |
|---|---|
| 승주 | |
| 혜린 | |

## 🌿 브랜치 · 커밋 규칙
- `main` — 배포 가능한 상태만 유지, 직접 push 금지 (PR로만 머지)
- `feat/기능명`, `fix/버그명`, `docs/문서명` 브랜치에서 작업
- 커밋 메시지: `feat: 재료 입력 UI 추가`, `fix: …`, `docs: …`, `chore: …`

## 🔐 주의
API 키 등 비밀값은 절대 커밋하지 않습니다. `.env.example`만 커밋하고 실제 값은 각자 로컬 `.env`에 둡니다.
