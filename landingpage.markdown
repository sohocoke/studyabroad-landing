---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default

# TODO: 
# - replace placeholder content
#   - text
#   - images
# - disable unneessary elements
# - publish on github pages
# - signup input validation
# - set up domain name
# - set up firebase access control
---


<!-- Navigation -->
<nav class="navbar navbar-expand-lg navbar-dark navbar-custom fixed-top">
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
      <h1 class="masthead-heading mb-0">올인원 유학 준비</h1>
      <h2 class="masthead-subheading mb-0">해외유학 준비에 필요한 모든 문서를 한 번에 준비할 수 있다면?</h2>
      <a href="#" class="btn btn-primary btn-xl rounded-pill mt-5">Learn More</a>
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
          <h2 class="display-4">직접 해외유학을 준비하는 지원자에게 꼭 맞는 온라인 서비스</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quod aliquid, mollitia odio veniam sit iste esse assumenda amet aperiam exercitationem, ea animi blanditiis recusandae! Ratione voluptatum molestiae adipisci, beatae obcaecati.</p>
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
          <h2 class="display-4">번역, 공증, 성적 변환, 우편 문서 제출 대행 등 토탈 서비스 제공</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quod aliquid, mollitia odio veniam sit iste esse assumenda amet aperiam exercitationem, ea animi blanditiis recusandae! Ratione voluptatum molestiae adipisci, beatae obcaecati.</p>
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
          <h2 class="display-4">지원자와의 지속적인 소통을 통한 최적의 작업 결과 보장</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quod aliquid, mollitia odio veniam sit iste esse assumenda amet aperiam exercitationem, ea animi blanditiis recusandae! Ratione voluptatum molestiae adipisci, beatae obcaecati.</p>
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
          <p>2021년 상반기 출시 목표로 현재 비공개 베타 테스트 중입니다.</p>
          <p>초대를 원하시면 이메일 주소를 남겨 주십시오.</p>

          <input type="text" id="subscribe-email-address"      name="subscribe-email-address"/>
          <button id="submit">초대 요청</button>
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
    // alert("Thanks for sending a message. I'll try and get back to you as soon as possible.")
    // TODO present result.

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

  var contact_submit = function(){
    var email = document.getElementById("subscribe-email-address");
    var data = {
      "email": email.value
    };

    push_to_firebase(data);

  }

  document.getElementById("submit").addEventListener("click", contact_submit);
</script>

