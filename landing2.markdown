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
headline: 해외유학 일인자들이 한 곳에 모두 모인 서비스가 있다면?
features:
  - title: 분야별로 가장 많은 우수사례를 <br/>보유한 서비스만을 엄선
    text: 지금까지는 홀로 유학을 준비하는 지원자와 학부모님들은 과연 누구의 말을 믿어야 할 지, 내가 알아본 정보가 정확한 것인지, 준비한 결과물이 학교의 요구와 내 의도에 맞게 만들어졌는지 확신을 가지기 어려웠습니다.
  - title: 번역, 성적 변환, 공증, 검수, 우편물 발송등 <br/>유학 준비 필수 서비스 제공
    text:  이제 번역, 검수, 공증, 성적 변환, 우편물 발송까지, 해외유학 준비에 필요한 각 분야의 일인자들이 해외 유학 준비에 필요한 필수 서비스를 한 곳에서, 최고의 품질로 제공해드립니다.
  - title: 유학원과는 차원이 다른 <br/>분야별 전문 서비스 제공
    text: 유학원과는 달리 어떤 사람들이 지원자를 위해 일하고 있는 지 투명하고 정직하게 공개하며, 엄선된 분야별 전문 업체의 최고의 수준을 자부합니다.
---

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
        timestamp: Date.now(),
        "source": "landing2",

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

