# Lumloom Journal

Lumloom과 공개 프로젝트를 소개하고, 앱을 만들며 배운 것과 하루문장 글을 기록하는 GitHub Pages 블로그입니다.

## 구조

- `index.html`: 블로그 홈과 공개 프로젝트 목록
- `posts.html`: Lumloom 프로젝트 글 목록
- `daily.html`: 하루문장 글 목록. `_daily`의 MD 파일을 날짜순으로 자동 표시
- `_daily/`: 하루문장 원문 MD 파일
- `_layouts/daily-post.html`: 하루문장 MD에 공통으로 적용되는 게시글 디자인
- `posts/`: 직접 작성한 Lumloom 프로젝트 HTML 게시글과 자동 생성된 하루문장 주소
- `styles.css`: 전체 디자인과 반응형 스타일
- `404.html`: GitHub Pages 오류 페이지

## 하루문장 글 추가하기

`_daily` 폴더에 영문 파일명의 MD 파일을 추가합니다. 본문 위에는 아래 정보를 넣습니다.

```markdown
---
title: 글 제목
title_break: 글 제목
date: 2026-10-25
category: 글감
prompt: 식물
read_time: 5분
description: 게시글 위에 표시할 짧은 소개
summary: 하루문장 목록에 표시할 짧은 소개
source: 하루문장
tags:
  - 하루문장
---

여기에 글 본문을 Markdown으로 작성합니다.
```

변경사항을 `master` 브랜치에 올리면 GitHub Pages가 게시글 HTML과 하루문장 목록을 자동으로 생성합니다. `prompt`에는 글감을 적고, `title_break`에는 필요한 경우 `<br />`을 넣어 제목 줄바꿈을 지정할 수 있습니다.

## 배포

GitHub Pages는 `master` 브랜치의 루트 파일을 Jekyll로 변환하여 배포합니다. 로컬에서 단순 웹 서버로 열면 Liquid 목록과 Markdown 변환은 처리되지 않으므로, 최종 결과는 GitHub Pages 배포 후 확인합니다.
