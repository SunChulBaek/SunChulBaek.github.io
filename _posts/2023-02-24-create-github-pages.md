---
title: "깃허브 페이지 생성하기 (Minimal Mistakes 테마)"
categories:
  - Blog
tags:
  - GitHub
  - Pages
  - Minimal Mistakes
---

# 요약
> 테마의 starter를 사용하면 깃허브 페이지를 쉽게 생성 할 수 있습니다.

# 본문
깃허브 페이지 생성 관련된 블로그들을 찾아보니 아래와 같은 방법들이 보였습니다.
1. Jekyll 테마 repository에서 fork
2. pages repository를 생성하고나서 Jekyll 테마를 zip으로 받아서 push

하지만 [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) 테마의 경우에는
[starter](https://github.com/mmistakes/mm-github-pages-starter/generate)가 있어서, 
쉽게 테마가 적용된 repository를 생성할 수 있었습니다.

Repository name에 {본인계정}.github.io를 입력하고 Create repository from template를 클릭하면,

![starter](/assets/images/2023-02-24-create-github-pages/0.jpg)

테마가 적용된 repository가 생성되었습니다.

![created](/assets/images/2023-02-24-create-github-pages/1.jpg)

그리고 https://{본인계정}.github.io로 접속하면 아래와 같이 테마가 적용된 템플릿이 생성된 것을 확인 할 수 있습니다. 

![web](/assets/images/2023-02-24-create-github-pages/2.jpg)

제가 쓰지 않은 글 목록도 보이고, 개인 정보도 수정해야 할 것 같고, 테마 커스텀도 필요할 것 같습니다.
이런 작업들은 다음 포스팅에서 진행해보겠습니다.