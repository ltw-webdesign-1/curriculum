---
layout: slide-deck
title: "Flexbox"
desc: "A quick introduction to the CSS Flexbox properties, how they work and what they do."

slides:
  - type: super-big-text
    content: |
      **Flexbox**

  - type: figure
    image: flexbox.svg
    caption: |
      A **one** dimensional layout system: row **or** column.

  - content: |
      ## Works on children

      Many of the flexbox properties are applied to the parent element, but affect the child elements.

      *This is different from many other CSS properties that directly affect the selected element.*

  - type: interactive
    html: |
      <ul>
        <li>Item 1</li>
        <li>Item 2</li>
      </ul>
    css: |
      ul {
        list-style-type: none;
        padding: 0;
        display: flex;
        justify-content: space-between;
      }
    css_hidden: |
      li:nth-child(1) {
        background-color: pink;
      }
      li:nth-child(2) {
        background-color: hotpink;
      }
    css_lines:
      - num: 4
        text: |
          We’re targeting all the child elements and making them go side-by-side.
      - num: 5
        text: |
          Force the elements to be as spread out as possible.

  - type: interactive
    html: |
      <ul>
        <li>Item 1</li>
        <li>Item 2</li>
      </ul>
    css: |
      ul {
        list-style-type: none;
        padding: 0;
        display: flex;
        justify-content: space-between;
        align-items: center;
      }
    css_lines:
      - num: 6
        text: |
          Use `align-items` to control the boxes on the cross-axis.
    css_hidden: |
      li:nth-child(1) {
        background-color: pink;
        padding: 1rem 0;
      }
      li:nth-child(2) {
        background-color: hotpink;

  - type: interactive
    html: |
      <ul>
        <li>
          <h2>Unicorns</h2>
          <p>Mythical horse-like creatures with a large single horn protruding from the centre of their heads.</p>
          <a href="#">More about unicorns</a>
        </li>
        <li>
          <h2>Narwhals</h2>
          <p>Whales with a single horn protruding from their head.</p>
          <a href="#">More about unicorns</a>
        </li>
      </ul>
    css: |
      li {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
      }
      p {
        margin-bottom: auto;
      }
    css_lines:
      - num: 3
        text: |
          Make the flexbox items move in a column. Without specifying `direction`, `row` is automatic.
      - num: 7
        text: |
          Use an automatically generated margin on the bottom to fill the empty space—aligning the paragraphs to the top.
    css_hidden: |
      ul {
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 1rem;
        font-size: 50%;
      }
      h2,
      p {
        margin: 0;
      }
      a {
        align-self: start;
      }

  - content: |
      ## Videos & tutorials

      - [Flexbox ➔](/topics/flexbox/)
      - [Flexbox cheat sheet ➔](/topics/flexbox-cheat-sheet/)
      - [CSS layout cheat sheet ➔](/topics/css-layout-cheat-sheet/)

---
