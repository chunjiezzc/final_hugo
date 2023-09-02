---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  
  
  - block: collection
    id: featured
    content:
      title: Publication
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Working Paper
      text: |-

      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Contact me:
      # Contact (add or remove contact options as necessary)
      email: zc.zhang.2023@pbs.smu.edu.sg
      phone: (+65) 80671032
      address:
        street: Lee Kong Chian School of Business, 50 Stamford Road
        city: Singapore
        postcode: '178899'

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
