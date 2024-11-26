---
type: PageLayout
title: Shaun Hammond
colors: colors-b
backgroundImage:
  type: BackgroundImage
  url: /images/featured-Image2.jpg
  backgroundSize: cover
  backgroundPosition: center
  backgroundRepeat: no-repeat
  opacity: 0
sections:
  - elementId: ''
    colors: colors-c
    backgroundSize: full
    title: 'Gidday, I''m Shaun Hammond a Game UI/UX Designer'
    subtitle: >-
      I started my career with New Blood Interactive in 2014, worked over 5
      years with RocketWerkz Studios and then nearly 3 years with my friends at
      Usual Suspects Studios. I'm based in Dunedin, New Zealand and open to new
      opportunities.
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
          - ml-0
          - mr-0
        padding:
          - pt-36
          - pb-36
          - pl-4
          - pr-4
        alignItems: center
        justifyContent: center
        flexDirection: row-reverse
      title:
        textAlign: left
        fontWeight: 500
      subtitle:
        textAlign: left
      text:
        textAlign: left
      actions:
        justifyContent: flex-start
    type: HeroSection
    actions: []
    text: ''
  - type: TextSection
    colors: colors-f
    variant: variant-a
    title: ''
    text: >+
      Including:


      *   **UI assets** for **layouts** I've designed, and **implementation** of
      these inside of **Unreal Engine**, and **Unity**.


      *   **UI/UX Programming** in **Unreal's Blueprint**.


      *   **Logos** and **Branding** for companies, games and fake entities
      inside of those game universes.


      *   **Marketing** material, both for storefronts like **Steam** and also
      physical media such as **PAX**, **Gamescom** etc.


      *   I've also completed projects requiring **UI Shaders**, **Level
      Design**, **Lighting**, **Game Design**, and **Textures** for 3D Assets.

    elementId: ''
    styles:
      self:
        height: auto
        width: wide
        padding:
          - pt-28
          - pb-28
          - pl-4
          - pr-4
        justifyContent: center
      title:
        textAlign: left
      subtitle:
        textAlign: left
      text:
        textAlign: left
    subtitle: Below you will see some of the work I've created over the years.
  - type: FeaturedProjectsSection
    subtitle: 'Projects:'
    actions:
      - type: Link
        label: See all projects
        altText: See all projects
        url: /projects
        showIcon: false
        icon: arrowRight
        iconPosition: right
        elementId: ''
    projects:
      - content/pages/projects/project-one.md
      - content/pages/projects/project-two.md
    colors: colors-f
    variant: variant-a
    elementId: ''
    showDate: false
    showDescription: true
    showFeaturedImage: true
    showReadMoreLink: true
    styles:
      self:
        height: auto
        width: wide
        padding:
          - pt-24
          - pb-24
          - pl-4
          - pr-4
        justifyContent: center
      title:
        textAlign: left
      subtitle:
        textAlign: left
      actions:
        justifyContent: center
  - colors: colors-f
    type: FeaturedProjectsSection
    elementId: ''
    actions:
      - type: Link
        label: See all projects
        url: /projects
    showDate: false
    showDescription: true
    showFeaturedImage: true
    showReadMoreLink: true
    variant: variant-b
    projects:
      - content/pages/projects/project-two.md
      - content/pages/projects/project-three.md
      - content/pages/projects/project-one.md
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
          - ml-0
          - mr-0
        padding:
          - pt-24
          - pb-24
          - pl-4
          - pr-4
        justifyContent: center
      title:
        textAlign: left
      subtitle:
        textAlign: left
      actions:
        justifyContent: flex-end
    subtitle: Projects
  - type: ContactSection
    title: "Contact Me \U0001F4E7"
    text: |
      or reach out via social media below.
    form:
      type: FormBlock
      title: Title of the form
      fields:
        - type: TextFormControl
          name: name
          label: name
          hideLabel: true
          placeholder: Your name
          width: 1/2
          isRequired: 'true'
        - type: EmailFormControl
          name: email
          label: email
          hideLabel: true
          placeholder: Your email
          width: 1/2
          isRequired: 'true'
        - type: TextareaFormControl
          name: message
          label: message
          hideLabel: true
          placeholder: Your message
          width: full
          isRequired: true
      submitLabel: Send Message
      elementId: contact-form
      styles:
        submitLabel:
          textAlign: left
    colors: colors-c
    backgroundSize: full
    elementId: ''
    styles:
      self:
        height: auto
        width: narrow
        padding:
          - pt-28
          - pb-36
          - pl-4
          - pr-4
        alignItems: center
        justifyContent: center
        flexDirection: row
      title:
        textAlign: left
      text:
        textAlign: left
---
