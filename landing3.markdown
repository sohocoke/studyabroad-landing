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
title:  유학 정보 마법사
headline: 해외유학, 가고 싶은 학교만 정하면 모든 정보를 가져다주는 서비스가 있다면?
features:
  - title: 지원자별 1:1 맞춤형 정보제공
    text: 해외유학을 준비하며, 지원하고 싶은 각 학교들의 홈페이지를 찾아본 경험이 있다면, 학교마다 다른 입시정보를 정리하는 일이 얼마나 번거로운 지 알 수 있습니다. 그래서 이 모든 정보를 오직 당신만을 위해 제공해드립니다.
  - title: 지원자가 선정한 학교의 가장 최신 입시 및 입학 정보 제공
    text:  카페나 블로그에 퍼져있는 수많은 학교와 입시 정보자료들은 과연 지금 나에게 필요한 정확한 정보일까요? 이제 내가 가고 싶은 학교와 전공, 입학 희망 시기에 맞춘 가장 최신의 가장 정확한 정보만을 받아보세요.
  - title: 지원자의 전공과 선정 학교를 모두 반영한 정보 제공
    text: 각기 다른 지원자가 희망하는 학교와 전공은 무척 다양합니다. 그에 맞추어 국가와 학교별로 각기 다른 인문계열에서부터 과학계열은 물론, 예체능계열과 의학계열까지 각 전공별 입시절차의 특수성을 모두 고려한 상세한 입시정보를 제공해드립니다.
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
          <img class="img-fluid rounded-circle" src="img/landing3/01.jpg" alt="">
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
          <img class="img-fluid rounded-circle" src="img/landing3/02.jpg" alt="">
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
