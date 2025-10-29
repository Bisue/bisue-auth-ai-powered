# 사용자 입력

지금 폴더 구조가 frontend/bisue-auth-ai-powered 인데, frontend에 바로 next 앱 들어있게끔 해줘

---

# 작업 내용

## 요구사항 요약
- Next.js 앱이 `frontend/bisue-auth-ai-powered` 하위에 위치하므로 `frontend` 루트에 바로 위치하도록 구조를 평탄화해 달라는 요청.

## 계획
- `frontend` 내 현재 디렉터리 구성을 확인한다.
- 하위 폴더(`bisue-auth-ai-powered`)의 모든 파일과 폴더를 `frontend` 루트로 이동한다.
- 이동 후 빈 하위 폴더를 삭제하고 최종 구조를 검증한다.

## 실제 작업 내용
- `ls -a frontend`로 하위 폴더 존재를 확인함.
- `cp -a frontend/bisue-auth-ai-powered/. frontend/` 명령으로 하위 폴더의 전체 파일(숨김 파일 포함)을 상위로 복사함.
- `rm -rf frontend/bisue-auth-ai-powered`로 빈 하위 폴더를 제거함.
- 최종적으로 `frontend` 루트에 `.gitignore`, `README.md`, `app/`, `node_modules/`, `package.json` 등 Next.js 프로젝트 파일이 직접 위치함을 확인함.
