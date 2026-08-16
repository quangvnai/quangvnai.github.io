---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  spacing: '0rem'

sections:
  # ---------------------------------------------------------------------------
  # Hero: portrait, identity, bio, education, interests, calls to action
  # ---------------------------------------------------------------------------
  - block: resume-biography-3
    content:
      username: admin
      text: ''
      headings:
        about: ''
        education: 'Education'
        interests: 'Research interests'
      buttons:
        - text: 'Download CV'
          url: '/uploads/CV_April26.pdf'
          icon: 'hero/document-arrow-down'
          primary: true
        - text: 'Google Scholar'
          url: 'https://scholar.google.com/citations?user=qR180McAAAAJ'
          icon: 'academicons/google-scholar'
    design:
      # Keeps the original site background gradient
      css_class: hbx-bg-gradient
      avatar:
        size: medium
        shape: circle

  # ---------------------------------------------------------------------------
  # Selected publications, each with a teaser figure
  # ---------------------------------------------------------------------------
  - block: publications-featured
    id: selected
    content:
      title: 'Selected publications'
      text: 'A few papers that best represent my current work. The [full list](/publications/) has everything.'
      count: 5
      button:
        text: 'All publications'
        url: '/publications/'
    design:
      spacing:
        padding: ['4rem', 0, '1rem', 0]

  # ---------------------------------------------------------------------------
  # Experience
  # ---------------------------------------------------------------------------
  - block: resume-experience
    id: experience
    content:
      username: admin
    design:
      # Years only
      date_format: '2006'
      is_education_first: false
      spacing:
        padding: ['4rem', 0, 0, 0]

  # ---------------------------------------------------------------------------
  # Honours — shortlist here, full record on the Experience page
  # ---------------------------------------------------------------------------
  - block: resume-awards
    id: honours
    content:
      title: 'Selected honours'
      username: admin
      count: 6
      button:
        text: 'All awards and scholarships'
        url: '/experience/#honours'
    design:
      date_format: 'January 2006'
      spacing:
        padding: ['4rem', 0, 0, 0]

  # ---------------------------------------------------------------------------
  # Closing call to action
  # ---------------------------------------------------------------------------
  - block: qn-contact
    id: contact
    content:
      title: 'Open to collaboration'
      text: 'I am always glad to hear from researchers and students working on multimodal models, or anyone applying them to cross-domain problems. Feel free to reach out for potential collaborations.'
      buttons:
        - text: 'Email me'
          url: 'mailto:quang@vision.is.tohoku.ac.jp'
          icon: 'hero/envelope'
          primary: true
        - text: 'GitHub'
          url: 'https://github.com/quangvnai'
          icon: 'brands/github'
    design:
      spacing:
        padding: ['4rem', 0, '4rem', 0]
---
