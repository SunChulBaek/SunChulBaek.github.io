---
title: "깃허브 페이지에 댓글 기능 추가 (Minimal Mistakes 테마)"
last_modified_at: 2023-02-27T06:30:00+09:00
categories:
  - Blog
tags:
  - GitHub
  - Pages
  - Minimal Mistakes
  - Comments
  - 댓글
  - Disqus
  - Giscus
  - Utterances
---

# 요약
> [Giscus](https://giscus.app/ko)로 댓글 기능을 붙였습니다.

# 본문
방문해주시는 분들도 얼마 없고, 댓글을 달고 싶은 분들은 더 없겠지만!
그래도 블로그를 유지하려면 댓글 기능 정도는 있어야하지 않을까 하는 생각이 들었습니다.

검색을 해보고 후보를 우선 3가지로 추려보았습니다.
1. [Disqus](https://disqus.com/) 선정 이유 : 다른 블로그에 붙어 있는 것을 본적이 있다. (남이 쓰면 좋은줄)
2. [Giscus](https://giscus.app/ko) 선정 이유 : GitHub의 discussions를 사용
3. [Utterances](https://github.com/apps/utterances) 선정 이유 : GitHub의 issues를 사용

## Giscus 붙이기
처음 시도했을때는 실패했는데요. 글 작성하다가 최종적으로는 giscus로 댓글 기능을 붙였습니다.
처음에는 repository 명시를 하지 않아서 이슈가 발생했던 것 같습니다.
![giscus](/assets/images/2023-02-27-add-comment-github-pages/giscus.png)
장점은 대댓글 작성이 가능합니다.

## Disqus 붙이기
장점은 _config.yml에 작성할 내용은 가장 적습니다.
단점은 광고가 붙는다고 하고, 블로그 본문과 댓글이 다른 서비스로 유지가 된다는 부분이 마음에 들지 않았습니다.

## Utternaces 붙이기
![utternces](/assets/images/2023-02-27-add-comment-github-pages/utterances.png)
단점은 대댓글 작성이 안되네요.
giscus 붙일 때와 같이 repository 명시가 중요한 것 같습니다.

## 결론
댓글 기능이 붙이고 나니 이제 기능적으로는 그럴듯한 블로그가 된 것 같습니다.