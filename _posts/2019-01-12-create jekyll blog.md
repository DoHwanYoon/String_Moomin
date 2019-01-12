---
layout: post
title: "Github Page를 기반으로 지킬(jekyll) 블로그 생성하기"
date: 2019-01-11
excerpt: "Github Page를 기반으로 지킬(jekyll) 블로그 생성방법과 테마 적용 방법 설명"
tag: [blog, markdown, github, github.io, jekyll]
comments: false
---

## Jekyll Blog란?

 Jekyll은 Blog 지향의 정적 사이트 생성기이다. 

 Github Page의 내부 엔진이기도 한데, 쉽게 말해 Jekyll을 사용하여 자신의 프로젝트 페이지 또는 블로그, 웹사이트를 무료로 Github에 호스팅 할 수 있다. 지금부터 Jekyll Blog생성 방법을 설명하려 한다.

---

## Ruby 설치

`Jekyll`은 [Ruby](https://rubyinstaller.org/downloads/)를 기반으로 만들어졌기 때문에 Jekyll Blog를 Local에서 테스트 하기 위해서는 Ruby를 설치해야 한다.

위 링크로 들어가 `Ruby+Devkit 2.5.3-1(x64)` 를 다운로드 받아 설치

![Ruby Install](/image/20190112-create-jekyll-blog/create-jekyll-blog1.PNG)

---

## 지킬(Jekyll) 설치

Ruby 설치가 완료되었다면 Windows 검색창에서 `Ruby`검색후 실행

![Search Ruby]({{site.static_url}}/image/20190112-create-jekyll-blog/create-jekyll-blog2.jpg)

콘솔창에서 아래에 나와있는 5개의 [Gem] 명령어를 통해 지킬과 실행에 필요한 패키지들을 설치

```
gem install jekyll
gem install minima
gem install bundler
gem install jekyll-feed
gem install tzinfo-data
```

---

## Local에서 블로그 실행하기

Ruby 콘솔창에서 [이전 포스팅]에서 생성한 블로그의 깃허브 저장소와 연동된 폴더로 이동

```
cd C:User\폴더경로\...\사용자이름.github.io

//인코딩 에러 발생시 아래 코드 실행
chcp 65001

//Jekyll 실행
bundle exec jekyll serve
```



브라우저를 열어 (localhost:4000)으로 접속하면 Local상에서 블로그가 실행 되는 것을 확인 할 수 있다.

![Ruby Install]({{site.static_url}}/image/20190112-create-jekyll-blog/create-jekyll-blog3.jpg)

다음 포스트에서는 Markdown을 이용하여 Jekyll로 포스트를 작성하는 방법과 포스트를 Github에 업로드 하는 방법을 알아볼것이다.

---

