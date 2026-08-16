---
title: Publications
cms_exclude: true
type: landing

design:
  spacing: '0rem'

# "0 min read" is meaningless on a paper page that carries an abstract rather
# than an article.
cascade:
  reading_time: false

sections:
  - block: publications-featured
    id: selected
    content:
      title: 'Selected publications'
      count: 5
    design:
      spacing:
        padding: ['3rem', 0, '1rem', 0]

  - block: publications-list
    id: all
    content:
      title: 'All publications'
      text: 'Grouped by year. See [Google Scholar](https://scholar.google.com/citations?user=qR180McAAAAJ) for citation counts.'
    design:
      spacing:
        padding: ['3rem', 0, '4rem', 0]
---
