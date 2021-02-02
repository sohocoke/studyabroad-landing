---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

# TODO: 
# - replace placeholder content
#   - text
#   - images
# - set up domain name
# - set up firebase access control

layout: default
title:  올인원 유학 준비
headline: 해외유학 준비에 필요한 모든 문서를 한 번에 준비할 수 있다면?
features:
  - title: 직접 유학을 준비하는 지원자들을 위하여
    text: 유학원의 힘을 빌리지 않고 직접 해외유학을 준비하다보면 각 단계마다 많은 어려움에 직면하게 됩니다. 그 중에서도 가장 지원자들을 힘들게 하는 일은 다양한 종류의 문서를 작성하는 일입니다.
  - title: 번역부터 제출까지 토탈 서비스
    text:  이제 간편하게 온라인으로 유학과 관련된 문서 준비를 한 번에 끝내세요. 학교별 에세이, 추천서와 이외 모든 입학에 필요한 문서 번역에서부터, 대외활동 내역 등 공증이 필요한 번역과 결과물 검수, 그리고 만들어진 문서의 제출까지 해외유학에 필요한 모든 문서에 대한 Total Support Service를 경험해보세요.
  - title: 지원자와의 지속적인 소통을 통한 최적의 작업 결과 보장
    text: 일반적인 번역 서비스와는 달리 한 번의 결과물 제공으로 끝나지 않고, 지원자가 만족할 때까지 교정과 검수를 진행하여 최고의 결과물만을 제공합니다.
---


<!-- Navigation -->
<nav class="navbar  invisible  navbar-expand-lg navbar-dark navbar-custom fixed-top">
  <div class="container">
    <a class="navbar-brand" href="#">Start Bootstrap</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarResponsive">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item">
          <a class="nav-link" href="#">Sign Up</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Log In</a>
        </li>
      </ul>
    </div>
  </div>
</nav>

<header class="masthead text-center text-white">
  <div class="masthead-content">
    <div class="container">
      <h1 class="masthead-heading mb-0">{{ page.title }}</h1>
      <h2 class="masthead-subheading mb-0">{{ page.headline }}</h2>
      <a href="#" class="btn  invisible  btn-primary btn-xl rounded-pill mt-5">Learn More</a>
    </div>
  </div>
  <div class="bg-circle-1 bg-circle"></div>
  <div class="bg-circle-2 bg-circle"></div>
  <div class="bg-circle-3 bg-circle"></div>
  <div class="bg-circle-4 bg-circle"></div>
</header>

<section>
  <div class="container">
    <div class="row align-items-center">
      <div class="col-lg-6 order-lg-2">
        <div class="p-5">
          <img class="img-fluid rounded-circle" src="img/01.jpg" alt="">
        </div>
      </div>
      <div class="col-lg-6 order-lg-1">
        <div class="p-5">
          <h2 class="display-4">{{ page.features[0].title }}</h2>
          <p>{{ page.features[0].text }}</p>
        </div>
      </div>
    </div>
  </div>
</section>

<section>
  <div class="container">
    <div class="row align-items-center">
      <div class="col-lg-6">
        <div class="p-5">
          <img class="img-fluid rounded-circle" src="img/02.jpg" alt="">
        </div>
      </div>
      <div class="col-lg-6">
        <div class="p-5">
          <h2 class="display-4">{{ page.features[1].title }}</h2>
          <p>{{ page.features[1].text }}</p>
        </div>
      </div>
    </div>
  </div>
</section>

<section>
  <div class="container">
    <div class="row align-items-center">
      <div class="col-lg-6 order-lg-2">
        <div class="p-5">
          <img class="img-fluid rounded-circle" src="img/03.jpg" alt="">
        </div>
      </div>
      <div class="col-lg-6 order-lg-1">
        <div class="p-5">
          <h2 class="display-4">{{ page.features[2].title }}</h2>
          <p>{{ page.features[2].text }}</p>
        </div>
      </div>
    </div>
  </div>
</section>

<section>
  <div class="container">
    <div class="row align-items-center">
      <div class="col-lg-6 order-lg-1">
        <div class="p-5" style="text-align: center;">
          <p>2021년 상반기 출시 목표로 준비 중입니다.</p>
          <p>비공개 베타 사용자 초대를 원하시면 이메일 주소를 남겨 주십시오.</p>

          <!-- <form id="subscribe-form" action="#subscribe-form"> -->
            <p>
              <input type="text" id="subscribe-email-address"      name="subscribe-email-address"/>
              <button id="submit">초대 요청</button>
            </p>
          <!-- </form> -->
          <p id="validation-error-message" class="invisible text-danger">이메일 주소가 올바르지 않습니다.</p>
          <p id="thank-you-message" class="invisible">감사합니다.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Firebase App (the core Firebase SDK) is always required and must be listed first -->
<script src="https://www.gstatic.com/firebasejs/8.2.4/firebase-app.js"></script>

<!-- If you enabled Analytics in your project, add the Firebase SDK for Analytics -->
<script src="https://www.gstatic.com/firebasejs/8.2.4/firebase-analytics.js"></script>

<!-- Add Firebase products that you want to use -->
<!-- <script src="https://www.gstatic.com/firebasejs/8.2.4/firebase-auth.js"></script> -->
<script src="https://www.gstatic.com/firebasejs/8.2.4/firebase-firestore.js"></script>

<script>
  // Your web app's Firebase configuration
  // For Firebase JS SDK v7.20.0 and later, measurementId is optional
  var firebaseConfig = {
    apiKey: "AIzaSyAFAC-srJh4nNjSL_eiL26aw8iIDK8LL-I",
    authDomain: "studyabroad-landing.firebaseapp.com",
    databaseURL: "https://studyabroad-landing-default-rtdb.firebaseio.com",
    projectId: "studyabroad-landing",
    storageBucket: "studyabroad-landing.appspot.com",
    messagingSenderId: "325414329709",
    appId: "1:325414329709:web:dc1811f54664e7b60e0e64",
    measurementId: "G-HHSN5WQRYB"
  };
  // Initialize Firebase
  firebase.initializeApp(firebaseConfig);
  firebase.analytics();
</script>

<script type="text/javascript">
  var push_to_firebase = function(data){
    var db = firebase.firestore();

    db.collection("signups").add({
        email: data["email"],
        timestamp: Date.now()
    })
    .then(function(docRef) {
        console.log("Message sent, ID: ", docRef.id);
        // location.reload();
    })
    .catch(function(error) {
        console.error("Message could not be sent: ", error);
    });
  }

  var validEmail = function(string) {
    const re = /^(([^<>()[\]\\.,;:\s@\"]+(\.[^<>()[\]\\.,;:\s@\"]+)*)|(\".+\"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/;
    return re.test(string);
  };

  var contact_submit = function(){
    var validationError = document.getElementById("validation-error-message");
    validationError.classList.add("invisible");

    var email = document.getElementById("subscribe-email-address");

    if (validEmail(email.value)) {
      var data = {
        "email": email.value
      };

      // prevent further input.
      var button = document.getElementById("submit");
      button.setAttribute("disabled", "");

      push_to_firebase(data);
    
      // on success, show thank-you message.
      // TODO survey.
      var thankYou = document.getElementById("thank-you-message");
      thankYou.classList.remove("invisible");
      
    } else {
      validationError.classList.remove("invisible");
    }
  }

  document.getElementById("submit").addEventListener("click", contact_submit);

  document.getElementById("subscribe-email-address").addEventListener("keyup", function(event) {
    if (event.keyCode === 13) { 
        document.getElementById("submit").click(); 
    }
  });
</script>

