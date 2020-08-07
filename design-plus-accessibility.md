---
layout: slide-deck
title: "Design + accessibility"
desc: "A reminder one accessibility considerations when designing websites—things to look for & how to find them."

slides:
  - type: super-big-text
    content: |
      **Design + accessibility**

  - content: |
      ## Why?

      - Accessibility is important: not only because its the law, but because we care
      - Not everybody access The Web or uses computers the same way you do
      - We don’t want the thing we create to prevent them from completing their task

  - content: |
      ## Font sizes

      *Always test that your website works with different font sizes.*

      - 2 sizes up & 2 sizes down
      - People prefer different sizes of text—our design shouldn’t break when the text changes size
    notes: |
      In Firefox, go to the menu: `View > Zoom` & enable `Zoom Text Only`

      - `⌘+` — Increases font size
      - `⌘-` — Decreases font size
      - `⌘0` — Sets the default font size

  - content: |
      ## Length & justification

      *Always consider the text’s line-length & justification.*

      - Line-length: too long or too short is hard to read
      - Don’t full justify text on The Web—many people find it difficult to read

  - type: text-code
    content: |
      ## Link obvious-ness

      *Always make links extremely obvious—***ideally underlined (navigation bar exempted)**

      - Helps people scan to find links on the page
      - Don’t rely on colour distinction alone—not everyone can see the colour difference
    css: |
      /**
       * You can change how the underline looks!
       * Some of these properties are so new
       *   they only work in Firefox.
       */

      a {
        text-decoration: underline;
        text-decoration-color: hotpink;
        text-decoration-thickness: .3em;
        text-underline-offset: .2em;
      }

  - content: |
      ## Link hit area

      *Always make links have the largest hit areas possible.*

      - Moving a mouse is difficult for many people
      - Navigation & buttons should be extra large, especially for big thumbs & mobile screens

  - type: text-code
    content: |
      ## :focus = :hover

      *Always style the `:focus` state the same as the `:hover` state.*

      - Helps people using the keyboard follow along when pressing tab
    css: |
      /**
       * Duplicate the hover styles for focus
       */

      a:hover,
      a:focus {
        color: hotpink;
      }

  - type: text-code
    content: |
      ## Focus rings

      *Always style the selected control in an obvious manner.*

      - Helps people using the keyboard follow along when pressing tab
    css: |
      /**
       * Create a high contrast focus ring
       * Always be attentive to the contrast
       *   between the focus ring
       *   & its background colour
       */

      a:focus {
        outline: 0.15rem solid #000;
        outline-offset: 0.2rem;
      }

  - type: two-col
    text_size: peta
    col1: |
      ## Colour contrast

      *Always test colours for contrast—helping people with colour blindness.*

      - Without enough contrast text may become unreadable
    col2: |
      ![Average vision](average.png)
      ![Red-green — unreadable](red-green.png)
      ![Red-green — difficult](red-green-2.png)
      ![Blue-yellow](blue-yellow.png)
    notes: |
      1. Average vision
      1. Red-green — unreadable
      1. Red-green — difficult
      1. Blue-yellow

  - type: two-col
    text_size: peta
    col1: |
      ## Missing images

      *Always test your design without images.*

      - Some people choose to disable images: to prevent flashing & seizures, poor internet connection, etc.
      - All the content should still be vislble—usually just adding a background colour helps
    col2: |
      ![Text on image](with-image.jpg)
      ![Text unreable when image missing](image-missing.jpg)
      ![Background colour behind missing image](image-missing-bg.jpg)
    notes: |
      1. Text on image
      1. Text unreable when image missing
      1. Background colour behind missing image

  - content: |
      ## Janky designs

      *Always make sure important landmarks don’t move.*

      - It’s difficult for people to constantly have to look for something
      - It’s often easier to remember “where” something is
    notes: |
      These things should never change location:

      - Logo & company name
      - Navigation

  - type: text-code
    content: |
      ## Hidden vs. visually hidden

      *Always be careful when hiding things.*

      - `display: none` & `hidden` hide from everything—including screen readers
      - Use a `.visually-hidden` class to hide only from sited users
    html: |
      <!--
        “about Plesiosaurs” will be read by screen readers
          but not visible to sited users
      -->

      <a href="#">
        <span>Read more</span>
        <span class="visually-hidden">about Plesiosaurs</span>
      </a>
    css: |
      /**
       * Hide something from sited users
       *   but not from screen readers
       */

      .visually-hidden {
        height: 1px;
        margin: -1px;
        overflow: hidden;
        padding: 0;
        position: absolute;
        width: 1px;
        border: 0;
        clip: rect(0 0 0 0);
        clip-path: inset(50%);
      }

  - content: |
      ## Videos & tutorials

      - [Accessibility ➔](/topics/accessibility/)
      - [Content accessibility ➔](/topics/content-accessibility/)
      - [Accessibility for design ➔](/topics/accessibility-for-design/)

---
