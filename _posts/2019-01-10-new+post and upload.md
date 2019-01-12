---
layout: post
title: "마크다운(markdown)을 사용하여 지킬(jekyll)로 포스트 작성하기"
date: 2019-01-12
excerpt: "마크다운(markdown)언어의 간략한 사용 방법과 지킬(Jekyll)포스트 작성방법, 그리고 github에 업로드 하는 방법"
tag: [blog, markdown, github, github.io, jekyll, post]
comments: false
---

# 마크다운(markdown) 이란?

Jekyll은 마크다운 문법을 통해 작성된다.

마크다운이라는것은 최소한의 텍스트 convention을 통하여 문서의 틀을 잡는 것인데, 몇가지 간단한 규칙이 있고 해당 규칙에 따라 웹에 표시될 때 효과를 갖는 것을 이야기 한다.

일반 Text파일과 .md의 확장자 파일로 작성하면 된다.

필자는 [Typora](https://www.typora.io/)라는 마크다운 에디터를 사용한다.

---

### "#" 의 갯수는 Heading(제목, 소제목)으로 표시되고 이는 Bold 효과와 크기로 제어된다.

> # 마크다운
>
> ## 마크다운
>
> ### 마크다운
>
> #### 마크다운

```
### "#"의 갯수는 Heading(제목,소제목)으로 표시되고 이는 Bold 효과와 크기로 제어된다.
> # 마크다운
  ## 마크다운
  ### 마크다운
  #### 마크다운
```

### "*" 와 "1." 로 시작되는 부분은 목록 시작점이다.

> * DoHwan_Yoon
> * String_Moomin
>
> 1. DoHwan_Yoon
> 2. String_Moomin

```
### "*" 와 "1." 로 시작되는 부분은 목록 시작점이다.
> * DoHwan_Yoon
    String_Moomin
  
  1. DoHwan_Yoon
     String_Moomin
```

### 링크(Link) 는 [링크 이름] (실제 링크) 로 사용할 수 있다.

> [String_Moomin의 Blog](https://dohwanyoon.github.io/String_Moomin/)

```
### 링크(Link)는 [링크 이름](실제링크)로 사용할 수 있다.
> [String_Moomin의 Blog](https://dohwanyoon.github.io/String_Moomin/)
```

### Bold 효과와 기울임 효과는 ** Bold **, * 기울임 * 으로 사용한다.

> **Bold**
>
> *기울임*
>
> ***Bold + 기울임***

```
### Bold 효과와 기울임 효과는 **Bold**, *기울임*으로 사용한다.
> **Bold**
  *기울임*
  ***Bold + 기울임***
```

---

### Convention

컨벤션이란 파일명 또는 프로젝트 폴더 트리 구성을 약속된 convention에 따라 작성하면 자동으로 설정 되는 부분을 의미한다.

- Post 작성 시 정보를 최상단에 기입한다.

  ```
  ---
  layout: post
  title: "마크다운(markdown)을 사용하여 지킬(jekyll)로 포스트 작성하기"
  date: 2019-01-10
  category: Github
  tags: [blog, markdown, jekyll, github, github.io]
  ---
  ```

- layout 부분의 post는 대부분 post로 둔다. 수정 할 일은 잘 없을것이라 생각한다.
- title은 포스트의 제목이다.
- category는 동적으로 관리되며, 기존에 있는 카테고리를 기입하면 해당 카테고리 안에 포스트가 자동으로 추가되고, 새로운 카테고리를 입력하면 자동으로 새로운 카테고리가 생성된다.
- tag는 [Instagram](https://www.instagram.com)의 그것과 비슷하다고 생각하면 좋을 것 같다. 검색엔진의 노출에 유리하다.
- 파일명은 yyyy-mm-dd-title.md 이며, _post 폴더에 위치한다.

---

### Post Upload

포스트 작성을 완료했다면 업로드를 해보자.

업로드는 jekyll을 설치할 때 사용했던 git 명령어로 github.io로 넣어준다고 생각하면 된다.

```
git add *
git commit -m "post"
git push
```

위 명령어를 입력했다면 페이지 적용까지 최소 30초에서 최대 3분정도가 소요될 수 있다.
