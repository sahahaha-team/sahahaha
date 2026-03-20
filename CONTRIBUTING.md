# 🤝 사하구청 AI 상담사 프로젝트 기여 가이드

## 🌿 브랜치 전략 (Feature Branch)
- `main`: 배포 가능한 안정적인 코드가 모이는 보호된 브랜치
- `feat/이슈번호-작업내용`: 새로운 기능 개발 (예: `feat/#1-crawling`)
- `bug/이슈번호-버그내용`: 버그 수정 (예: `bug/#2-login-error`)

## 💬 커밋 컨벤션 (Conventional Commits)
- `feat:` 새로운 기능 추가
- `fix:` 버그 수정
- `docs:` 문서 수정
- `refactor:` 코드 구조 개선
- `test:` 테스트 코드 추가

## 👀 PR 리뷰 가이드 (Review Convention)
리뷰어는 아래 태그를 사용하여 피드백을 남깁니다.
- **[MUST]**: 반드시 수정해야 하는 치명적인 오류나 요구사항 누락
- **[SHOULD]**: 수정하는 것이 좋은 구조적 개선 제안
- **[SUGGEST]**: 사소한 제안이나 더 나은 방향 (수정 선택)
- **[QUESTION]**: 코드의 의도나 작동 방식에 대한 질문