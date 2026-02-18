---
layout: splash
title: "openKcloud Platform"
excerpt: "An Open AI Semiconductor-based Cloud Service Platform for Hyperscale AI Services." 


header:
  overlay_image: /assets/images/hero.png
  overlay_filter: 0.45

  actions:
    - label: "Latest release v0.10.0"
      url: "https://github.com/openkcloud/openkcloud/releases/tag/v0.1.0"
      class: "btn--inverse btn--small"
    - label: "⬇ Downloads"
      url: "https://github.com/openkcloud/openkcloud.github.io/blob/main/downloads/2025/openKcloud%20DevDay%202025%20Presentations.zip"
      class: "btn--inverse btn--large"

feature_row:
  - image_path: /assets/images/feature-1.png
    alt: "AI반도체 클라우드 서비스"
    title: "AI반도체 클라우드 서비스"
    excerpt: "가속기,엣지,클라우드 구성요소를 모듈화하여 기능을 빠르게 확장."
    url: /docs/architecture/
    btn_label: "Learn More"
    btn_class: "btn--primary"

  - image_path: /assets/images/feature-2.png
    alt: "클라우드 운용비용 최적화"
    title: "클라우드 운용비용 최적화"
    excerpt: "데스크톱,태블릿,모바일에서 문서,대시보드 탐색이 편리."
    url: /docs/intro/
    btn_label: "Learn More"
    btn_class: "btn--primary"

  - image_path: /assets/images/feature-3.png
    alt: "초거대 AI모델 실행환경"
    title: "초거대 AI모델 실행환경"
    excerpt: "이슈,문서,릴리스 노트를 기준으로 투명하게 협업."
    url: /contact/
    btn_label: "Learn More"
    btn_class: "btn--primary"
---

{% include feature_row %}
## Recent News

<div class="recent-news">
  <ul>
    {% for post in site.posts limit:5 %}
      <li>
        <span class="recent-news__date">{{ post.date | date: "%Y-%m-%d" }}</span>
        <a class="recent-news__title" href="{{ post.url | relative_url }}">{{ post.title }}</a>
        {% if post.excerpt %}
          <div class="recent-news__excerpt">{{ post.excerpt | strip_html | truncate: 120 }}</div>
        {% endif %}
      </li>
    {% endfor %}
  </ul>
</div>

<a class="btn btn--primary btn--small" href="{{ '/news/' | relative_url }}">더보기</a>