---
title: "안드로이드 개발자가 깃허브 페이지에 글쓰기"
last_modified_at: 2023-03-03T16:00:00+09:00
categories:
  - Blog
tags:
  - GitHub
  - Pages
  - Minimal Mistakes
  - Android Studio
---

# 요약
> [Android Studio](https://developer.android.com/studio)를 사용하면 어렵지 않게 글을 쓸 수 있습니다.

# 본문
깃허브 페이지에 글을 올리려면 _posts 디렉토리에 'YEAR-MONTH-DAY-title.MARKUP' 파일을 만들어야 합니다.
저는 안드로이드 개발자이기 때문에 고민없이 [Android Studio](https://developer.android.com/studio)를 사용합니다.

## 깃허브 계정 설정
'Android Studio > Settings'로 갑니다. 'Version Control > GitHub'으로 갑니다. +버튼을 누르고 'Login With Token'을 선택 합니다.
![0](/assets/images/2023-03-03-wirte-in-github-pages/0.png)

'Add GitHub Account' 창이 나옵니다. 'Generate' 버튼을 누릅니다.
![1](/assets/images/2023-03-03-wirte-in-github-pages/1.png)

브라우저에서 GitHub 토큰 생성화면으로 넘어가고, 맨 아래의 'Generate Token' 버튼을 누릅니다.
![2](/assets/images/2023-03-03-wirte-in-github-pages/2.png)

블러 처리된 부분을 복사해주세요 (네모 두개 겹쳐진 버튼을 누르면 복사될걸요)
![3](/assets/images/2023-03-03-wirte-in-github-pages/3.png)

복사한 토큰을 Token 영역에 붙여넣기 해주세요. 그리고 'Add Account' 버튼을 누릅니다.
![4](/assets/images/2023-03-03-wirte-in-github-pages/4.png)

짜잔. 계정이 추가 되었습니다.
![5](/assets/images/2023-03-03-wirte-in-github-pages/5.png)

## 소스 
'File > New > Project from Version Control'로 갑니다.
계정, 클론할 리포지터리, 클론할 위치를 선택하여 클론 버튼을 누릅니다.
![6](/assets/images/2023-03-03-wirte-in-github-pages/6.png)

## 파일 생성
_posts 디렉토리에서 우클릭 'New > File'을 선택하여 위의 파일명 규칙에 따라 파일을 만듭니다.
![7](/assets/images/2023-03-03-wirte-in-github-pages/7.png)

## commit & push
파일내용을 블라블라 작성을 하고 상단의 초록 체크 버튼을 누릅니다.
![8](/assets/images/2023-03-03-wirte-in-github-pages/8.png)

업로드할 파일을 체크 해주고, commit message를 작성하고 commit 버튼 옆의 화살표를 눌러 commit and push를 선택합니다.
![9](/assets/images/2023-03-03-wirte-in-github-pages/9.png)

## 확인
잠시 후에 업로드 된 내용을 확인 할 수 있습니다.