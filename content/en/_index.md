---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
#type: landing
type: home_index
#subTitle: Animal Physiological Ecology and Conservation







heroBlock:
  block: hero
  content:
    title:
#    image:
#      filename: research_topic.jpg
    text: |
      The APEC (Animal Physiological Ecology and Conservation) Lab at Sun Yat-sen University focuses on the physiological ecology and conservation of terrestrial animals, especially reptiles and birds. Our research integrates field and controlled experiments with mechanistic and statistical models to explore how animals interact with their environment. By studying physiological responses and ecological dynamics, we assess species’ adaptability and vulnerability to environmental change. Our work aims to enhance biodiversity conservation by bridging experimental research with predictive modeling.

  
heroSlideBlock:
  block: slider
  content:
    slides:
    - title: 
      content: 
      align: center
      background:
        image:
          filename: group_slides/group_members_202509.jpg
          filters:
            brightness: 1.1
        position: right
        color: '#666'  
    # - title: 
    #   content: 
    #   align: left
    #   background:
    #     image:
    #       filename: group_slides/group_photo2.jpg
    #       filters:
    #         brightness: 1
    #     position: right
    #     color: '#666'  
  design:
    # Slide height is automatic unless you force a specific height (e.g. '400px')
    slide_height: '400px'
    is_fullscreen: false
    # Automatically transition through slides?
    loop: false
    # Duration of transition between slides (in ms)
    interval: 2000


newsBlock:
  block: collection
  content:
    title: Latest News
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


publicationsBlock:
  block: collection
  content:
    title: Publications
    count: 5
    filters:
      folders:
        - publication
#      publication_type: 'article-journal'
      publication_type: 
  design:
    view: card
    columns: '1'      

teamsBlock:
  block: markdown
  content:
    title:
    subtitle:  
    text: |
      {{% cta cta_link="./people/" cta_text="Meet the team →" %}}
  design:
    columns: '1'





sections:
  - block: hero
    content:
      title: |
        Random Matrix Optics
        Research Group
      image:
        filename: research_topic.jpg
      text: |
        <br>
        
        Random matrix optics introduces the random matrix toolbox to the representation of light wave-particle duality. Starting in 2019, our group focused on light field representation, decomposition, detection, and manipulation using the random matrix representation. Random matrix representation provides a statistical gating strategy for different components in the light field. For example, the single and multiple scattering component in wide-field reflective imaging; the ballistic and multiple scattering component in spectral-domain OCT. The gated multiple scattering component facilitates the calculation of absorption information for in-vivo tissue imaging.
  
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
  
#  - block: markdown
#    content:
#      title:
#      subtitle: ''
#      text:
#    design:
#      columns: '1'
#      background:
#        image: 
#          filename: coders.jpg
#          filters:
#            brightness: 1
#          parallax: false
#          position: center
#          size: cover
#          text_color_light: true
#      spacing:
#        padding: ['20px', '0', '20px', '0']
#      css_class: fullscreen

  - block: collection
    content:
#      title: Latest Preprints
      title: Latest Publications
      text: ""
      count: 5
      filters:
        folders:
          - publication
#        publication_type: 'article'
        publication_type: 'article-journal'
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
