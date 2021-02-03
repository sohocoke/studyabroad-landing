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
title:  검증된 유학 준비 서비스
headline: 해외유학 일인자들이 한 곳에 모두 모인 서비스가 있다면?
features:
  - title: 분야별로 가장 많은 우수사례를 보유한 서비스만을 엄선
    text: 지금까지는 홀로 유학을 준비하는 지원자와 학부모님들은 과연 누구의 말을 믿어야 할 지, 내가 알아본 정보가 정확한 것인지, 준비한 결과물이 학교의 요구와 내 의도에 맞게 만들어졌는지 확신을 가지기 어려웠습니다.
  - title: 번역, 성적 변환, 공증, 검수, 우편물 발송등 유학 준비 필수 서비스 제공
    text:  이제 번역, 검수, 공증, 성적 변환, 우편물 발송까지, 해외유학 준비에 필요한 각 분야의 일인자들이 해외 유학 준비에 필요한 필수 서비스를 한 곳에서, 최고의 품질로 제공해드립니다.
  - title: 유학원과는 차원이 다른 분야별 전문 서비스 제공
    text: 유학원과는 달리 어떤 사람들이 지원자를 위해 일하고 있는지 투명하고 정직하게 공개하며, 엄선된 분야별 전문 업체의 최고의 수준을 자부합니다.
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
