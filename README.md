# 🦁 Zoo Board Game

영어 회화 연습용 보드게임 (음성 인식 + TTS 기반)

## 🚀 배포 방법 (3단계, 약 5분 소요)

### 1단계: GitHub에 업로드

1. **github.com** 접속 → 우측 상단 **"+"** → **"New repository"** 클릭
2. Repository 이름: `zoo-board-game` (원하는 이름 가능)
3. **Public** 선택 → **"Create repository"** 클릭
4. 새 레포 페이지에서 **"uploading an existing file"** 링크 클릭
5. **이 폴더의 모든 파일을 통째로 드래그&드롭** (node_modules 제외, 폴더 구조 유지!)
6. 하단 **"Commit changes"** 버튼 클릭

> 💡 **중요**: `.github` 폴더(점으로 시작)도 꼭 함께 올려야 합니다.
> Mac에서 안 보이면: `Cmd + Shift + .` 키로 숨김 파일 표시 켜기

### 2단계: Vercel과 GitHub 연결

1. **vercel.com** 접속 → **"Sign Up"** → **"Continue with GitHub"** 클릭 (기존 GitHub 계정으로 가입)
2. 가입 완료되면 대시보드에서 **"Add New..."** → **"Project"** 클릭
3. 방금 만든 `zoo-board-game` 레포지토리 옆 **"Import"** 버튼 클릭
4. 아무 설정도 바꾸지 말고 그냥 **"Deploy"** 버튼 클릭
5. 약 1~2분 기다리면 배포 완료! 🎉

### 3단계: 학생들에게 링크 공유

배포가 끝나면 `https://zoo-board-game-xxx.vercel.app` 같은 URL이 생성됩니다.
이 링크를 학생들에게 카톡, 클래스팅, 학급 게시판 등에 공유하면 됩니다.

---

## ✅ 학생 안내 시 꼭 알려줄 것

1. **Chrome 또는 Edge 브라우저로만 접속!** (Safari, Firefox는 음성 인식 불가)
2. 첫 마이크 버튼 누를 때 권한 요청 팝업 → **"허용"** 클릭
3. 노트북/태블릿 사용 권장 (마이크 내장)

---

## 🛠️ 로컬에서 테스트하기 (선택사항)

만약 Node.js가 설치돼 있다면, 배포 전 로컬에서 테스트해볼 수 있습니다:

```bash
npm install
npm run dev
```

브라우저에서 `http://localhost:5173` 접속.

---

## 🔄 코드 수정 후 재배포

GitHub 레포지토리에서 파일을 수정하면, **Vercel이 자동으로 감지해서 1~2분 내에 재배포**합니다.
별도로 다시 deploy 버튼을 누를 필요가 없어요.

---

## 💬 문제 해결

- **배포는 됐는데 화면이 깨져요**: 브라우저 캐시 삭제 후 재접속 (`Ctrl+Shift+R` 또는 `Cmd+Shift+R`)
- **마이크가 안 잡혀요**: 주소창 왼쪽 자물쇠 🔒 아이콘 클릭 → 마이크 "허용" 확인
- **Vercel에서 빌드 실패**: GitHub 레포에 `package.json`이 제대로 올라갔는지 확인
