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
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        I design human-centered intelligent systems at the intersection of **human-AI interaction**, **large language model agents**, and **multi-agent systems**. My recent work studies socially collaborative, relationship-centered multi-agent systems — AI companions that support people through shared experiences rather than one-off answers. More broadly, I build systems for health and well-being that translate advances in multimodal and agentic AI into tools that meet genuine human needs.

        I'm always glad to talk about research and new collaborations 😃
    design:
      columns: '1'
  - block: collection
    id: projects
    content:
      title: Featured Research
      text: ""
      count: 0
      filters:
        folders:
          - project
        featured_only: true
    design:
      view: article-grid
      fill_image: false
      columns: 2
  - block: collection
    id: papers
    content:
      title: Publications
      text: ""
      count: 0
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
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
