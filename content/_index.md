---
# Leave the homepage title empty to use the site title
title: ''
date: 2024-05-01
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: skills
    content:
      title: Skills
      text: ''
      # Choose a user to display skills from (a folder name within `content/authors/`)
      username: admin
    design:
      columns: '1'
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Director of Bioinformatics
          company: Iowa Institute of Human Genetics
          company_url: 'https://medicine.uiowa.edu/humangenetics/'
          company_logo: 
          location: Iowa City, IA
          date_start: '2019-08-01'
          date_end: ''
          description: |2-
              Responsibilities include: 
               * Leading and managing a team of 3 bioinformaticians
               * Improving core revenue by adopting 'agile' project workflows
               * Testing Director for CAP/CLIA KidneySeq targeted NGS panel
               * Co-founding and running the UI 10X Visium Spatial Consortium
        - title: Scientific Advisor & Consultant
          company: FBB Biomed
          company_url: 'https://fbbbio.com/'
          company_logo: 
          location: California
          date_start: '2022-11-01'
          date_end: ''
          description: |2-
              Responsibilities include: 
               * Setting up and managing AWS pipelines for data analysis
               * Exploratory data analysis and QC
               * Creating predictive models using machine-learning 
        - title: Associate Research Scientist
          company: Iowa Institute of Human Genetics
          company_url: 'https://medicine.uiowa.edu/humangenetics/'
          company_logo: 
          location: Iowa City, IA
          date_start: '2015-07-01'
          date_end: '2019-07-01'
          description: |2-
              Activities:
               * Created the IIHG YouTube channel (18+ technical videos, >2500 subscribers)
               * Collaborated on wide array of human and mouse genomics projects 
               * Published many co-author papers in high-impact journals 
        - title: Postdoctoral Scholar
          company: University of California, San Francisco
          company_url: 'https://www.ucsf.edu/'
          company_logo: 
          location: San Francisco, CA
          date_start: '2009-07-01'
          date_end: '2015-07-01'
          description: |2-
              Activities:
               * Worked as a lead computational biologist on discovery team for novel p97 inhibitors
               * Validated binding predictions with labeled, high molecular weight NMR measurements 
               * Performed MD simulations of protein-protein complexes to study binding free energies
    design:
      columns: '2'
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Courses'
      subtitle:
      # Date format: https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: https://coursera.org/share/37bec72a5cead802f2449debe1afa0b1
          date_end: ''
          date_start: '2017-04-07'
          description: ''
          icon: coursera
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Statistics for Genomic Data Science
          url: ''
        - certificate_url: https://coursera.org/share/baa7af433c5e063d900001bdb6928f04
          date_end: ''
          date_start: '2017-04-30'
          description: ''
          icon: coursera
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Bioconductor for Genomic Data Science
          url: https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
        - certificate_url: https://www.datacamp.com
          date_end: '2020-12-21'
          date_start: '2020-07-01'
          description: ''
          icon: datacamp
          organization: DataCamp
          organization_url: https://www.datacamp.com
          title: 'Object-Oriented Programming in R'
          url: ''
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: Recent Posts
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
#  - block: portfolio
#    id: projects
#    content:
#      title: Projects
#      filters:
#        folders:
#          - project
#      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
#      default_button_index: 0
#      # Filter toolbar (optional).
#      # Add or remove as many filters (`filter_button` instances) as you like.
#      # To show all items, set `tag` to "*".
#      # To filter by a specific tag, set `tag` to an existing tag name.
#      # To remove the toolbar, delete the entire `filter_button` block.
#      buttons:
#        - name: All
#          tag: '*'
#        - name: Deep Learning
#          tag: Deep Learning
#        - name: Other
#          tag: Demo
#    design:
#      # Choose how many columns the section has. Valid values: '1' or '2'.
#      columns: '1'
#      view: showcase
#      # For Showcase view, flip alternate rows?
#      flip_alt_rows: false
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
#  - block: collection
#    id: talks
#    content:
#      title: Recent & Upcoming Talks
#      filters:
#        folders:
#          - event
#    design:
#      columns: '2'
#      view: compact
#  - block: tag_cloud
#    content:
#      title: Popular Topics
#    design:
#      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Contact information and University of Iowa office location:
      email: michael dot chimenti AT gmail dot com
      phone: 319-335-6717 (University)
      address:
        street: 431 Newton Road
        city: Iowa City
        region: IA
        postcode: '52242'
        country: United States
        country_code: US
      directions: Enter EMRB and take the North elevator to the third floor.  My office is 329A.
      coordinates:
        latitude: '41.66199'
        longitude: '-91.54529'  
      autolink: true
    design:
      columns: '2'
---
