### 📦 [9주차] GitHub Packages 및 의존성 보안 자동화

**1. npm 패키지 배포 및 버전 관리**
* GitHub Actions를 활용하여 `npm.pkg.github.com` 레지스트리에 `@hellokack` 스코프로 패키지를 배포함
* `package.json`의 버전을 1.0.0에서 1.0.1로 업데이트하여 지속적 배포(CD) 파이프라인의 정상 작동을 검증함
* 🔗 **배포된 패키지 확인:** 레포지토리 우측 하단의 [Packages 섹션](https://github.com/hellokack/sahahaha/packages)에서 확인 가능

**2. Docker 이미지 자동 배포 (GHCR)**
* 컨테이너 환경 구성을 위한 `Dockerfile`을 작성함
* 코드가 푸시될 때 자동으로 이미지를 빌드하고 `ghcr.io`에 배포하는 워크플로우를 구축함
* 로컬 환경에서 해당 이미지를 Pull 받아 정상 실행됨을 확인함

**3. Dependabot 및 보안 스캔 자동화**
* `.github/dependabot.yml`을 통해 npm 및 Docker 환경의 주간 의존성 검사 및 그룹화 정책을 설정함
* `npm audit` 기반의 보안 스캔 워크플로우를 구축함
* **[테스트 및 결과 증빙]**
* 취약점이 있는 패키지(`lodash@4.17.10`)를 의도적으로 주입하여, 파이프라인이 이를 감지하도록 트리거함
* 🚨 **자동 생성된 보안 이슈:** [여기를 클릭하여 자동 생성된 알림 확인하기](https://github.com/hellokack/sahahaha/issues)
* *(여기에 깃허브 Issues 탭에 경고글이 올라온 화면을 캡처해서 넣어주시면 완벽합니다)*

---
본 문서는 생성형 AI의 도움을 받아 작성되었습니다.