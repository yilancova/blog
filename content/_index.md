---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:

  - block: markdown
    design:
     background:
      image:
       filename: 1.jpg
       filters:
        brightness: 1
       size: cover
       position: center
       parallax: false
        
  
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
  - block: features
    content:
      title: Увлечения
      items:
        - name: Английский язык
          description: 20%
          icon: language
          icon_pack: fas
        - name: Программирование
          description: 70%
          icon: keyboard
          icon_pack: fas
        - name: Рисование
          description: 10%
          icon: pen
          icon_pack: fas
  - block: experience
    content:
      title: Опыт
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Студент
          company: РУДН
          company_url: 'https://www.rudn.ru'
          company_logo: org-rudn
          location: Россия
          date_start: '2022-09-01'
          date_end: ''
          description: |2-
              Responsibilities include:

              * Mathematics and computer science
        
    design:
      columns: '2'
  - block: Accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Достижения'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: https://www.coursera.org/learn/neural-networks-deep-learning
          date_end: ''
          date_start: '2023-01-25'
          description: 'К концу курса я лучше познакомилась с важными технологическими тенденциями.'
          organization: Coursera
          organization_url: https://www.stepik.org
          title: Нейронные сети и глубокое обучение
          url: ''
        
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: Посты
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
  - block: markdown
    id: jokes
    content:
      title: Анекдоты
      subtitle: ''
      text: |- 
        ### Анекдот 1
        Идёт Райан Гослинг по лесу, видит: машина стоит. Сел в неё, подождал ровно 5 минут и уехал.
        
        ### Анекдот 2
        Приходит мужик в бар и заказывает у бармена кофе. Бармен говорит: "Извините, у нас здесь нет кофе, но у нас есть энергетические напитки, они тоже содержат кофеин". Мужик говорит: "Ладно, дайте мне тогда энергетик". Бармен готовит напиток и говорит: "Вот ваш энергетик, но будьте осторожны, он очень сильный". Мужик выпивает напиток и начинает чувствовать себя очень энергичным и бодрым. Он решает пойти на пробежку и начинает бегать по городу, обгоняя всех прохожих. Вдруг он видит Райана Гослинга и кричит ему: "Райан, я тебя обгоняю!". Гослинг смотрит на него и говорит: "Ну и что? Я не бегаю для того, чтобы быть первым. Я бегаю для того, чтобы выглядеть красиво".
    design:
      columns: '2'
  - block: portfolio
    id: projects
    content:
      title: Проекты
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: Все
          tag: '*'
        - name: Программирование
          tag: Программирование
        - name: Другое
          tag: другое
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    content:
      title: Галерея
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: contact
    id: contact
    content:
      title: Контакты
      subtitle:
      text: |-
        Если есть вопросы к сайту, направьте мне их в письменном виде на почту.
      # Contact (add or remove contact options as necessary)
      email: yalantsova@gmail.com
      phone: 8 978 662 4419
      address:
        street: Пушкинская
        city: Москва
        region: Московская область
        postcode: '94305'
        country: Россия
        country_code: РФ
      directions: Войдите в 1 подъезд и поднимитесь на 7 этаж
      contact_links:
        - icon: video
          icon_pack: fas
          name: Коференция в zoom
          link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
