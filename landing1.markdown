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
  - title: 직접 유학을 준비하는 지원자들을 위하여
    text: 유학원의 힘을 빌리지 않고 직접 해외유학을 준비하다보면 각 단계마다 많은 어려움에 직면하게 됩니다. 그 중에서도 가장 지원자들을 힘들게 하는 일은 다양한 종류의 문서를 작성하는 일입니다.
  - title: 번역부터 제출까지 토탈 서비스
    text:  이제 간편하게 온라인으로 유학과 관련된 문서 준비를 한 번에 끝내세요. 학교별 에세이, 추천서와 이외 모든 입학에 필요한 문서 번역에서부터, 대외활동 내역 등 공증이 필요한 번역과 결과물 검수, 그리고 만들어진 문서의 제출까지 해외유학에 필요한 모든 문서에 대한 Total Support Service를 경험해보세요.
  - title: 지원자와의 지속적인 소통을 통한 최적의 작업 결과 보장
    text: 일반적인 번역 서비스와는 달리 한 번의 결과물 제공으로 끝나지 않고, 지원자가 만족할 때까지 교정과 검수를 진행하여 최고의 결과물만을 제공합니다.
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

{% include_relative signup.html %}
