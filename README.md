# 블로그 build 과정
## 1. 블로그에 적용할 테마 선택

![image](https://user-images.githubusercontent.com/84260219/146142039-32d167e6-101c-4056-9c5f-08a9c1695acb.png)

## 2. 테마의 Github으로 이동하여 앞서 만든 repository로 fork

![2](https://user-images.githubusercontent.com/84260219/146142303-e31cbf37-9000-42d0-a2ff-d351cc8affc1.png)

## 3. fork한 repository의 이름을 yeojin-g.github.io로 변경

![tempsnip](https://user-images.githubusercontent.com/84260219/146142719-27935e4b-1a5c-4d46-b1d2-29a161de37ab.png)

## 4. _config.yml 파일에서 정보 수정
#### Blog Title과 bio, github url등의 정보를 수정한다.
    # Site
    title:              Yeojin's Blog
    bio:                "Kookmin Univ Software 21"
    description:        "Kookmin Univ Software 21"
    github-url:         yeojin-g

## 5. 프로필 이미지와 Blog 배경 이미지 변경
#### - 프로필과 배경 이미지로 사용할 이미지 파일을 assets/img 에 업로드 한다.

![tempsnip](https://user-images.githubusercontent.com/84260219/146145167-8c1b73eb-23d9-44a0-980f-0e507d7c48db.png)

#### - _config.yml 파일에서 프로필과 배경 이미지 파일 경로를 수정한다.
    logo:               'assets/img/FullMoon.jpg'
    background:         'assets/img/night.jpg'

#### < 결과 >

![image](https://user-images.githubusercontent.com/84260219/146146097-b0ca9406-2c36-4ca5-953e-f9b59481d992.png)

## 6. 댓글 기능 구현
#### - fork 해온 테마에 disqus에 관한 코드가 모두 구현되어있기 때문에 _config.yml 파일에 disqus 링크 이름만 수정한다.
#### < disqus에 저장한 disqus short name >

![image](https://user-images.githubusercontent.com/84260219/146146884-c1a72588-d56c-421d-91ad-6b90f1cd148e.png)

#### < 수정 코드 >
    # Comments
    disqus_shortname:   yeojin-g
    
## 7. favicon 추가
#### - favicon으로사용할 이미지를 사이즈에 맞게 준비하여 assets/img/favicon 에 업로드 한다.

![tempsnip](https://user-images.githubusercontent.com/84260219/146163586-113ba2af-8933-47c1-b59c-aa8f98254b8d.png)

#### -favicon icon과 기타 파일을 업로드 한다.

![tempsnip](https://user-images.githubusercontent.com/84260219/146163829-d9b58eb3-40c0-4bf2-8dca-d5c92a71ec23.png)

#### - _includes/head.html 파일의 favicon관련 코드를 수정한다.
    <!-- Favicons -->
    <link rel="apple-touch-icon" href="{{ site.url }}/assets/img/favicons/moonRabbit.jpg">
    <link rel="apple-touch-icon" sizes="72x72" href="{{ site.url }}/assets/img/favicons/moonRabbit-72x72.jpg">
    <link rel="apple-touch-icon" sizes="114x114" href="{{ site.url }}/assets/img/favicons/moonRabbit-114x114.jpg">
    <link rel="apple-touch-icon" sizes="144x144" href="{{ site.url }}/assets/img/favicons/moonRabbit-144x144.jpg">
    <link rel="shortcut icon" type="image/jpg" href="{{ site.url }}/favicon.jpg" />
    <link rel="shortcut icon" href="{{ site.url }}/favicon.ico" />**
    
