---
title: "Bitrise로 안드로이드 프로젝트 빌드하기"
last_modified_at: 2023-04-04T09:00:00+09:00
categories:
- CI/CD
tags:
- Bitrise
- Android
---

# 요약
> [Bitrise](https://bitrise.io/)를 사용하면 손쉽게 빌드를 자동화 할 수 있습니다.

# 본문
개인 소스들의 빌드 자동화를 [Travis CI](https://www.travis-ci.com/)를 거쳐 현재는 [CircleCI](https://circleci.com/)를 사용하고 있는데요.
[Bitrise](https://bitrise.io/)가 모바일 플랫폼 지원이 잘 되어 있다고 해서 세팅을 해보았습니다.

## 프로젝트 세팅하기
여차저차 로그인을 해보면 아래와 같은 화면이 나옵니다. "Add new app"을 눌러봅니다.
![0](/assets/images/2023-04-04-bitrise-android/비트라이즈1.png)

권한 설정을 하는데 누가 본다고 문제가 될 건 없으니 public으로 설정해봅니다.
![1](/assets/images/2023-04-04-bitrise-android/비트라이즈2.png)

리포지터리를 선택합니다. 선택 UI로 연결된 github 계정의 리포지터리를 선택할 수 있는데, 저는 수동으로 넣어주었습니다.
![2](/assets/images/2023-04-04-bitrise-android/비트라이즈3.png)

브랜치를 선택합니다. 설정을 자동으로 해줘? 라고 물어보는데 당연히 자동이 좋습니다.
![3](/assets/images/2023-04-04-bitrise-android/비트라이즈4.png)

프로그레스가 쪼르르 올라갑니다.
![4](/assets/images/2023-04-04-bitrise-android/비트라이즈5.png)

음.. 자동으로 알아낸것은 '이 소스는 안드로이드 소스다!' 정도인 것 같습니다. 모듈 이름을 넣어줍니다.
![5](/assets/images/2023-04-04-bitrise-android/비트라이즈6.png)

Build Variant를 넣어줍니다.
![6](/assets/images/2023-04-04-bitrise-android/비트라이즈7.png)

지금까지 입력한 설정들과 어떤 환경에서 빌드를 수행할지를 보여줍니다.
![7](/assets/images/2023-04-04-bitrise-android/비트라이즈8.png)

앱 아이콘을 업로드 하라고 합니다. 빌드할 때 사용하는 것은 아니고 비트라이즈 대시보드에서 보여주는 용도입니다. 나중에 합시다.
![8](/assets/images/2023-04-04-bitrise-android/비트라이즈9.png)

웹훅 설정을 하면, 소스 변경사항이 생길 때 자동으로 빌드를 수행합니다. 이번에는 스킵해보았습니다.
![9](/assets/images/2023-04-04-bitrise-android/비트라이즈10.png)

이후에 빌드를 실행해보면 디폴트 bitrise.yml에 따라 수행하는 것으로 보입니다. (lint, unit test, build)
Workflow Editor를 사용해서 빌드 단계는 수정 할 수 있는 것으로 보입니다.
그리고 Status badge도 지원합니다. 요런거 -> [![Build Status](https://app.bitrise.io/app/517d171b-49da-4d27-aff2-880006082992/status.svg?token=ZbbLVUx-zTVU0booLajX7g&branch=main)](https://app.bitrise.io/app/517d171b-49da-4d27-aff2-880006082992)

## 크레딧
기본적인 세팅까지는 쉬운 편인것 같은데요.
비트라이즈에는 크레딧이라는 것이 있어서 이것을 사용해서 빌드를 할 수 있습니다.
처음 가입했을 때에는 500 크레딧을 주고, 머신에 따라 1~8 크레딧/분 과금이 됩니다.
![10](/assets/images/2023-04-04-bitrise-android/비트라이즈11.png)
500 크레딧이 다 떨어지면 Hobby 플랜 (무료 월 300 크레딧) 또는 유료 플랜을 구독해야 합니다.

샘플정도 되는 작은 프로젝트를 빌드하는데 3분정도 걸렸는데요.
300 크레딧이라면 웹훅 설정하기가 약간 고민되는 정도인 것 같습니다.

회사 프로젝트라면 Jenkins를 직접 세팅하는것 보다 유료 플랜 구독하는 것도 괜찮을 것 같습니다.

감사합니다.