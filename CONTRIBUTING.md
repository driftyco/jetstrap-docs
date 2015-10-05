## 블로그글쓰기 가이드
### 문체
1. 내 앞에 앉아있는 후배 또는 학생들에게 설명해 주는 느낌으로 해봅시다. 반말이 아니라 일반적 존칭. 그러면서도 친근하게.
2. 문어체라기 보다는 존칭형의 구어체. 문어체 - 논문 스타일. 구어체 - 선생님의 강의.
3. 문어체 - "본 글은 ~ 입니다",  구어체 - "이번 글은 저희 달리웍스의 개발 문화에 대한 소개입니다"
4. ~합니다. ~하시죠.  ~일까요?  등


### 웹에서 작성하기
1. http://prose.io/#daliworks/daliworks.github.io
  - prose.io 에 github authorization 필요.
2. Just Play!

## 예제
제일 먼저 올라간 sensorjs 글을 참고하세요. ```_posts/2015-4-1-SensorJS.md```에 있습니다.

### README에 있는 내용...

Edit `/_posts/2014-3-3-Hello-World.md` to publish your first blog post. This [Markdown Cheatsheet](http://www.jekyllnow.com/Markdown-Style-Guide/) might come in handy.

> You can add additional posts in the browser on GitHub.com too! Just hit the + icon in `/_posts/` to create new content. Just make sure to include the [front-matter](http://jekyllrb.com/docs/frontmatter/) block at the top of each new blog post and make sure the post's filename is in this format: year-month-day-title.md

## 설정

### footnote 쓰기위한 설정.
 - _config.yml 에 다음과 같이 설정.

```
markdown: redcarpet
redcarpet:
  extensions: [footnotes]
```

 - see [참고글](http://stackoverflow.com/questions/19483975/jekyll-on-github-pages-any-way-to-add-footnotes-in-markdown)

## 글쓰기 환경

 - http://jekyllrb.com/docs/installation/ 에서 필요한 것 설치.
 ```
  $ sudo brew install ruby
  $ sudo gem install jekyll
  $ sudo gem install jekyll-sitemap
 ```

 - repo 꺼내고,
 ```
 $ git clone https://github.com/daliworks/daliworks.github.io
 $ cd daliworks.github.io
 $ jekyll serve --watch
 ```

 - _post 폴더내의 컨텐츠를 추가/수정 등의 작업을 하시면, http://localhost:4000/ 에서 바로 확인할 수 있습니다.

 - 완료되면, git commit and push!

 - draft 작성,
 _draft/에서 파일 만들고 ```jekyll serve --watch --draft``` 로 볼 수 있음.
