---
# Leave the homepage title empty to use the site title
---
title: ""
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      title: |
        Dr. Tamborindeguy
        Laboratory
      text: |
        <br>
        The **Tamborindeguy Lab** investigates insect–pathogen–plant interactions with an emphasis on vector-borne plant pathogens, host manipulation, and mechanisms of transmission.
      # ✅ 여기 중요: image를 content 안이 아니라, 아래처럼 “안정된 키”로 넣어줌
      image:
        filename: /media/23.jpg
        alt_text: Lab photo
    design:
      # ✅ 이거 넣으면 텍스트+이미지 레이아웃이 잘 잡힘 (버전 호환 좋음)
      columns: "2"
---
  
  - block: collection
    content:
      title: Latest News
      subtitle:
      text:
      count: 5
      filters:
        author: ''
        category: ''
        exclude_featured: false
        publication_type: ''
        tag: ''
      offset: 0
      order: desc
      page_type: post
    design:
      view: card
      columns: '1'
  
  - block: markdown
    content:
      title:
      subtitle: ''
      text:
    design:
      columns: '1'
      background:
        image: 
          filename: coders.jpg
          filters:
            brightness: 1
          parallax: false
          position: center
          size: cover
          text_color_light: true
      spacing:
        padding: ['20px', '0', '20px', '0']
      css_class: fullscreen

  - block: collection
    content:
      title: Latest Preprints
      text: ""
      count: 5
      filters:
        folders:
          - publication
        publication_type: 'article'
    design:
      view: citation
      columns: '1'

  - block: markdown
    content:
      title:
      subtitle:
      text: |
        {{% cta cta_link="./people/" cta_text="Meet the team →" %}}
    design:
      columns: '1'
---
