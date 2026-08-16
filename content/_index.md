---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  spacing: '0rem'

# Single-page site. Every nav item is an anchor into a section below;
# section `id`s must stay in sync with config/_default/menus.yaml.
sections:
  # ---------------------------------------------------------------------------
  # About — portrait, identity, biography, interests, calls to action
  # ---------------------------------------------------------------------------
  - block: resume-biography-3
    id: about
    content:
      username: admin
      text: ''
      headings:
        about: ''
        interests: 'Research interests'
      # Rendered as small buttons in the same row as the profile icons.
      # A button with no `url` renders inert — clicking it does nothing.
      # Restore `url: '/uploads/CV_April26.pdf'` to make the CV downloadable.
      buttons:
        - text: 'CV'
          label: 'CV available on request'
    design:
      # Keeps the original site background gradient
      css_class: hbx-bg-gradient
      avatar:
        size: medium
        shape: circle

  # ---------------------------------------------------------------------------
  # Publications — selected papers with teaser figures.
  # The full year-grouped list is available as a `publications-list` block if
  # it is ever wanted back; Google Scholar covers the rest for now.
  # ---------------------------------------------------------------------------
  - block: publications-featured
    id: publications
    content:
      title: 'Selected publications'
      text: 'A few papers that best represent my current work. See [Google Scholar](https://scholar.google.com/citations?user=qR180McAAAAJ) for the full list.'
      count: 0 # 0 = show every paper flagged `featured: true`
    design:
      spacing:
        padding: ['4rem', 0, 0, 0]

  # ---------------------------------------------------------------------------
  # Experience
  # ---------------------------------------------------------------------------
  - block: resume-experience
    id: experience
    content:
      username: admin
      show: work
    design:
      # Years only; same-year roles fall back to months automatically
      date_format: '2006'
      spacing:
        padding: ['4rem', 0, 0, 0]

  # ---------------------------------------------------------------------------
  # Education
  # ---------------------------------------------------------------------------
  - block: resume-experience
    id: education
    content:
      username: admin
      show: education
    design:
      date_format: '2006'
      spacing:
        padding: ['4rem', 0, 0, 0]

  # ---------------------------------------------------------------------------
  # Honours — the ones flagged `selected: true` show; the rest expand in place
  # ---------------------------------------------------------------------------
  - block: resume-awards
    id: honours
    content:
      title: 'Honours'
      username: admin
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
      text: 'Im glad to hear from researchers and students working on multimodal models, or anyone applying them to cross-domain problems. Feel free to reach out for potential collaborations.'
      buttons:
        - text: 'Email me'
          url: 'mailto:vanquangn@uow.edu.au'
          icon: 'hero/envelope'
          primary: true

    design:
      spacing:
        padding: ['4rem', 0, '4rem', 0]
---
