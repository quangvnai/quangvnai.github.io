---
title: Courses
summary: My courses
type: landing

cascade:
  - target:
      path: '{/courses/*/**}'
    type: docs
    params:
      show_breadcrumb: true
  - build:
      render: never
      list: never
      publishResources: false

sections:
  - block: collection
    id: courses
    content:
      title: Courses
      filters:
        tag: Course
        kinds:
          - section
    design:
      view: article-grid
      show_read_time: false
      show_date: false
      show_read_more: false
      columns: 1

# Template demo content — excluded from the build.
# Delete this folder when you no longer need the examples.
build:
  render: never
  list: never
  publishResources: false

---
