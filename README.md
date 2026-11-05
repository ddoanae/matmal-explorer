# 맞말 탐험대 · GitHub Pages 배포 패키지

한국어 미니게임 2종을 담은 정적 웹사이트입니다. 별도 서버나 설치 과정 없이 HTML 파일만으로 동작합니다.

## 폴더 구조

```text
matmal-github-pages/
├── index.html            # 메인 허브 / 게임 선택
├── games/
│   ├── spelling.html     # 맞춤법 게임 (20문제, 2지선다)
│   └── choseong.html     # 초성 퀴즈 (5문제, 주관식, 이미지 스크래치)
├── .nojekyll             # GitHub Pages에서 불필요한 Jekyll 처리 방지
└── README.md             # 이 안내서
```

## GitHub Pages에 올리는 방법

1. GitHub에 로그인 후 **New repository**를 누릅니다.
2. 저장소 이름을 예: `matmal-explorer`로 설정하고, 무료 계정이면 **Public**으로 만듭니다.
3. 저장소에서 **Add file → Upload files**를 선택합니다.
4. 압축파일을 **해제한 뒤**, `index.html`, `games/` 폴더, `.nojekyll`, `README.md`를 저장소 **최상위(root)**에 업로드합니다. (ZIP 자체를 업로드하지 않기)
5. 아래의 **Commit changes**를 누릅니다.
6. **Settings → Pages → Build and deployment**에서 `Deploy from a branch`를 선택합니다.
7. Branch: `main`, Folder: `/(root)`로 설정하고 **Save**합니다.
8. 사이트 주소: `https://<GitHub-사용자명>.github.io/matmal-explorer/` (저장소 이름에 따라 달라짐)

GitHub Pages는 공개 웹사이트입니다. 비공개 팀 전용 서비스로 사용하려면 접근 제어가 가능한 별도의 호스팅이 필요합니다.

## 수정 방법

메인 페이지: `index.html` 수정. 맞춤법 문제: `games/spelling.html` 수정. 초성 문제 및 힌트: `games/choseong.html` 수정. GitHub에서 변경 내용을 커밋하면 사이트에 반영됩니다.
