# ✍️ 커밋 컨벤션 가이드

자습용 React with ts study file

- 참고 도서: [React + TypeScript로 배우는 자바스크립트 프레임워크](https://www.coupang.com/vp/products/7970063912?itemId=22070450512)
- 해당 책을 기반으로 학습하며 프로젝트를 구성합니다.

---

## 📌 브랜치 전략

### 1. **메인 브랜치**

- `main`: 배포 및 안정적인 코드가 위치하는 브랜치

### 2. **개발 브랜치**

- `develop`: 기능 개발이 진행되는 메인 브랜치로, `feature` 브랜치가 병합됨

### 3. **기능 개발 브랜치**

- `feature/#이슈번호`: 새로운 기능 추가 및 개발 진행 (예: `feature/#13`, `feature/#7`)

### 4. **버그 수정 브랜치**

- `fix/`: 기존 기능에서 발생한 버그를 수정하는 브랜치 (예: `fix/#4`)

---

## 👥 협업 방식

1. **Git Flow 기반 브랜치 전략**을 준수합니다.
2. 새로운 기능 개발 시 `feature/#이슈번호` 브랜치를 생성하여 작업 후 `develop` 브랜치로 PR을 생성합니다.
3. R이 생성되면 CI/CD 파이프라인에서 코드 검사를 수행하고, 검사 통과 후 코드 리뷰를 진행합니다.
4. 코드 리뷰에서 approve를 받은 후 develop 브랜치에 병합합니다.
5. 일정 단위 개발이 완료되면 aprrove를 받고 `develop` 브랜치를 `main` 브랜치로 병합하여 배포합니다.
6. 모든 커밋 메시지는 [Conventional Commit](https://www.conventionalcommits.org/en/v1.0.0/) 형식을 따릅니다.
   - `feat: 새로운 기능 추가`
   - `fix: 버그 수정`
   - `refactor: 코드 리팩토링`
   - `docs: 문서 변경`
   - `style: 스타일 변경 (코드 포맷, 세미콜론 추가 등)`
   - `chore: 빌드 설정 및 기타 변경사항`

---
