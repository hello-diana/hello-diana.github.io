---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
    # No background override: the section uses the site's default background and
    # text colors, which automatically follow the dark/light mode toggle.
    design:
      # Reduce the top gap between the navbar/header and the About Me content.
      spacing:
        padding: ['2rem', '0', '6rem', '0']
  - block: collection
    id: projects
    content:
      title: Featured Publications
      text: "Selected first-author and co-first-author work in multi-agent systems, self-distillation, and health sensing."
      count: 0
      sort_by: weight
      sort_ascending: true
      filters:
        folders:
          - publication
        featured_only: true
      archive:
        enable: true
        text: Full publication list on Google Scholar ↗
        link: https://scholar.google.com/citations?user=wdYlNXwAAAAJ&hl=en
    design:
      view: publication-card
      fill_image: false
      columns: 2
  - block: markdown
    id: papers
    content:
      title: Publications
      text: |-
        For my full publication list and citations, visit **[Google Scholar ↗](https://scholar.google.com/citations?user=wdYlNXwAAAAJ&hl=en)**.

        Recent collaborations include [PersonaCUABench](/publication/personacuabench/), [SourceLearn](/publication/sourcelearn/), [on-policy distillation in vision-language models](/publication/on-policy-distillation/), [FireFair](/publication/firefair/), and [Inductus](/publication/inductus/).

        Paper details and BibTeX are also available in the [publication archive](/publication/).
    design:
      columns: '1'
      spacing:
        padding: ['2rem', '0', '4rem', '0']
  - block: resume-experience
    id: experience
    content:
      title: Experience
      username: admin
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: true
  - block: resume-awards
    content:
      title: Awards
      username: admin
  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     view: article-grid
  #     columns: 1
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
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
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]

  - block: markdown
    id: visitors
    content:
      title: Visitors
      text: |-
        {{< displayVisitors >}}
    design:
      columns: '1'
---
