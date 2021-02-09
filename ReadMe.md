![KakaoTalk_20210210_014354713](C:\Users\kwakn\Documents\카카오톡 받은 파일\KakaoTalk_20210210_014354713.jpg)

# 종백쌤과 함께하는 단기속성 내 홈페이지 만들기 프로젝트

> 설 연휴동안 SSAFY에서 배운걸 최대한 활용해서!!!!GIT HUB으로 내 포트폴리오겸 홈페이지 만들기!!!!!!! 



## 2월 8일: 들어가기 앞서 구상

나는 우선 전문적인 내 이력을 보여주는 포트폴리오 보다는 그냥, 내가 좋아하는 내 그림 끄적이고 나를 담을 수 있는 홈페이지를 만들기로 기획했다. 이름하여, 졸업을 맞이하여 척척 학사로 거듭나기..! (박사보다 무섭다는 자신만만 학사) 나는 내가 말이 많다는 걸 알고는 있었지만, 이 성격이 치명적인 단점이 될줄은 몰랐다. 하고 싶은 말은 너무 많고 구현하기는 아직 실력이 미흡해 ^~^ 아주 욕망덩어리.. 나는 욕심boy...

2/8일 월요일에 다같이 디스코드에 모여서 같이 프로젝트를 진행하는 팀원들끼리 서로의 구성안을 공유했다. 다들 발표를 들으면 들을 수록 뭔가 자기 자신들에 대해 잘 알고 확신이 있는 사람들이 많다는것이 느껴진다. 정말 부러운 부분!~! 그리고 정말 전문적이시다.. 나는 뭔가 아직 장난같은 퀄리티의 결과물들 밖에 없는데^^~ 사실 얼마전까지만 해도 이런 미흡함?에 대해서 스스로 스트레스를 많이 받았는데 이제는 걍 별로 안받는다. 24살의 나현이는 이제 안다.. 스트레스 받아봤자 나는 그런 스타일의 결과물은 못낸다는거.. 아기자기하고 정신사납고 뽀짝한 것이,, 그거시,,,바로 나의 결과물이 될 수 밖에 없는 운명..

것봐 지금도 자야되면서 서론 오지게 길게 쓰고있따 쥼맬 나는 말썽쟁이

[초기 기획안]: https://github.com/moongchi98/my_portfolio/blob/main/%EB%82%98%ED%98%84_%ED%99%88%ED%8E%98%EC%9D%B4%EC%A7%80_%EA%B8%B0%ED%9A%8D%EC%84%9C.pdf



## 2월 9일: Navbar, Section 제작

쥼맬..다들..너무 열심히 한다..나는 술이나 와랄라 먹고..들어왔는데 다들 엄청 열심히 하고 계셔서 술 좀 깨고 12시부터...헐레벌떡 조금 끄적였다.. 만든거라 하기도 뭐하고 배웠던 Navbar하면서,,뭐 내용좀 끄적였다..

> 사용한 것들!
>
> 1. Bootstrap Navbar
> 2. 외부참조로 css 파일 이용하기
> 3. google font 직접 사용해보기

- **Navbar**

  ```html
  <header class="sticky-top">
      <!-- navbar -->
      <nav class="navbar bg-white">
        <div class="container-fluid">
          <a class="navbar-brand" href="#">
            <img src="images/logo.jpg" alt="나현이의 척척 학사 거듭나기" style="width:100px; height:100px;">
          </a>
          <ul class="nav justify-content-center">
            <li class="nav-item">
              <a class="nav-link active sans classicblue fs-3" aria-current="page" href="#">나현?나현!</a>
            </li>
            <li class="nav-item">
              <a class="nav-link sans classicblue fs-3" href="#">화학공학</a>
            </li>
            <li class="nav-item">
              <a class="nav-link sans classicblue fs-3" href="#">Interest</a>
            </li>
            <li class="nav-item">
              <a class="nav-link sans classicblue fs-3" href="#">SW 개발</a>
            </li>  
          </ul>
        </div>
      </nav>
    </header>
  ```

  배웠던 거에서 크게 차이는 없다. 다만 좀 애를 먹었던거는 역시 로고 사진 사이즈 조절. 이거는 내 감대로 그냥 정방향 모양으로 사이즈를 줬다. 그리고 `sticky-top`은 가장 큰 box인 header에 class를 지정해줘야 작동한다는 정도?

  Interest탭을 뭔가 더 멋진 이름으로 하고 싶은데 아직 아이디어가 안떠오른다.

  :heavy_check_mark: 해야할일

  각각 tab에 link 달기

  

- **Section**

  1. preview 내용 작성한 부분

     ```html
     <div class="row d-flex flex-column align-items-center">
             <img src="images/대표이사.jpg" alt="나 졸업한다!" style="width: 50%;" class="mt-5">
             <h1 class="sans text-white text-center mt-3">나현이의 척척 학사 거듭나기!</h1>
             <p  class="sans text-white text-center mt-3 fs-5">화학공학 전공이지만, 노는게 제일 좋아~♪ 이제는 개발자까지 도전하는 건국대 대표 뽀로로 </p>
             <p  class="sans text-white text-center mt-3 fs-5">의미있는 경험 하나하나가 잊혀지는게 너무 아까워서, 또 나의 20대를 나답게 기록하고 싶어서 시작한 이 페이지! </p>
             <p  class="sans text-white text-center mt-3 fs-5"> 이 곳이 미래의 나현이에게는 언제나 열정을, 추억을 주는 곳이자 계속 나의 이야기를 채워나가는 곳이 되면 좋겠습니다. </p>
             <p  class="sans text-white text-center mt-3 fs-5"> 그리고, 이 누추한 곳 까지 와계신 여러분에게도 그러한 곳이면 좋겠습니다. </p>
           </div>
     ```

     :question: 궁금한 점 

     저렇게 p태그를 계속 쓰는게 아니라, 한번에 문장을 구분해서 작성하는 방법은 없는걸까?

  2. 내 머릿속 부분

     여기서 부터 깨닫게 되었다,, 이 프로젝트의 가장 큰 문제는 개발 실력이 아니라 내 그림 실력이라는 것을,,

     술 마시는 옆모습을 못그려서 20분동안 쩔쩔...

     ```html
     <div class="row coconut flex-column align-items-center">
             <h2 class="pirate text-center sans mt-3">2021년 2월 24.2살의 나는?</h2>
             <p  class="pirate text-center sans mt-2 fs-5">천방지축 얼렁뚱땅 빙글빙글 돌아가는 지금의 나는 무슨 생각 중일까..?</p>
             <div class="d-flex justify-content-center">
               <a href="https://sports.news.naver.com/wfootball/record/index.nhn">
                 <img src="images/리버풀.png" alt="리버풀" style="width:80%">
               </a>
               <a href="#">
                 <img src="images/삼성전자.png" alt="삼성" style="width: 80%;">   
               </a>
               <a href="#">
                 <img src="images/술.png" alt="술" style="width: 80%;">
               </a>
             </div>
           </div>
     ```

     음 사실 이 부분에서는 내 최대 관심분야? 지금의 나를 나타내는 키워드? 같은 걸 하고 싶은데 뭔가 마음에 안든다.. 나중에 가면 전면 수정 될 거 같다.. 아래에 글씨로 해당하는 내용을 적고 싶었는데 안이쁜것 같고 손글씨가 더 이쁜것 같기도 하다가, 나중에는 그림만 있는게 제일 이쁜거 같아서 일단은 그림만 두었다. 요즘 리버풀 축구 짱못하니까 순위좀 걸어두고 삼성로고에는 내 목표인 대주주,, 삼성 주가를 걸어놓을까 생각중이다. 술은 요즘 좋아하는 술? 아니면 술마시고 사고친 리스트 목록을 만들어서 링크로 걸어놓을까 고민중! 고민은 내일,,하고,,자야지.,

     :heavy_check_mark: 그림, 글 다 맘에 안들어 전면 수정해야해,,