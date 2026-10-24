# Lumloom Journal

Lumloom과 공개 프로젝트를 소개하고, 앱을 만들며 배운 것을 기록하는 정적 블로그입니다.

## 구조

- `index.html`: 블로그 홈, 최근 글, 공개 프로젝트 목록
- `posts/`: 개별 게시글
- `styles.css`: 전체 디자인과 반응형 스타일
- `404.html`: GitHub Pages 오류 페이지

## 로컬 확인

PowerShell에서 별도 가상환경 활성화 없이 실행합니다.

```powershell
cd C:\Users\lmj89\Documents\Codex\lumloom-blog
python -m http.server 4189
```

브라우저에서 `http://127.0.0.1:4189/`을 엽니다.

GitHub Pages는 `master` 브랜치의 루트 정적 파일을 배포합니다.
