---
layout: slide-deck
title: "Grid for layouts"
desc: "A brief overview of how CSS Grid can be used to make two-dimensional layouts: columns & rows."

slides:
  - type: super-big-text
    content: |
      **Grid for layouts**

  - type: figure
    image: grids.svg
    caption: |
      A **two** dimensional layout system: rows **and** columns.

  - content: |
      ## Works on children

      Many of the grid properties are applied to the parent element, but affect the child elements.

      *This is different from many other CSS properties that directly affect the selected element.*

  - type: interactive
    html: |
      <ul>
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
        <li>Item 4</li>
      </ul>
    css: |
      ul {
        list-style-type: none;
        padding: 0;
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: .25rem;
      }
    css_lines:
      - num: 4
        text: |
          Enable grid on all the direct children. The direct children will automatically flow into the grid cells.
      - num: 5
        text: |
          Tell the grid how many columns to use. `1fr` is one fraction of the available space.
      - num: 6
        text: |
          Create space between the grid cells.
    css_hidden: |
      li:nth-child(1) {
        background-color: pink;
      }
      li:nth-child(2) {
        background-color: deeppink;
      }
      li:nth-child(3) {
        background-color: hotpink;
      }
      li:nth-child(4) {
        background-color: mistyrose;
      }

  - type: code-n-image
    image: grid-areas.svg
    html: |
      <ul>
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
        <li>Item 4</li>
      </ul>
    css: |
      ul {
        list-style-type: none;
        padding: 0;
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-areas:
          "box1 box1 box1"
          "box2 box3 ."
          "box2 box4 .";
      }
    css_lines:
      - num: "6-9"
        text: |
          The `areas` syntax allows you to define columns & rows in your grid.

          - Each row is defined by a set of `"` with area names within it.
          - If you repeat an area name that area will take up multiple columsn or rows.
          - Using a `.` means that cell is empty.
          - Usually you use this in combination with `columns` or `rows` to define sizes.

  - type: interactive
    html: |
      <ul>
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
        <li>Item 4</li>
      </ul>
    css: |
      li:nth-child(1) {
        grid-area: box4;
      }
      li:nth-child(2) {
        grid-area: box2;
      }
      li:nth-child(3) {
        grid-area: box1;
      }
      li:nth-child(4) {
        grid-area: box3;
      }
    css_lines:
      - num: 2
        text: |
          Specify which grid area—by name—this element should move into.
    css_hidden: |
      ul {
        list-style-type: none;
        padding: 0;
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-areas:
          "box1 box1 box1"
          "box2 box3 ."
          "box2 box4 .";
      }
      li:nth-child(1) {
        background-color: pink;
      }
      li:nth-child(2) {
        background-color: deeppink;
      }
      li:nth-child(3) {
        background-color: hotpink;
      }
      li:nth-child(4) {
        background-color: mistyrose;
      }
    notes: |
      *Inspect this with Firefox’s grid inspector to see the lines.*

  - type: interactive
    html: |
      <div>
        <h1><img src="images/mars.svg" alt="Mars"></h1>
        <img class="pano" src="images/pano.jpg" alt="" role="presentation">
      </div>
    css: |
      div {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-rows: 1fr;
      }
      img {
        width: 100%;
      }
      h1 {
        margin: 0;
        grid-column: 1 / 2;
        grid-row: 1;
        align-self: end;
        z-index: 1;
      }
      .pano {
        grid-column: 1 / -1;
        grid-row: 1;
      }
    css_lines:
      - num: 11
        text: |
          Start at grid line 1 and extend to grid line 2.
      - num: 13
        text: |
          Align the image to the end (bottom) of the grid cell.
      - num: 14
        text: |
          Bring the image to the front.

          By default elements are stacked in code order, since the `<h1>` comes first it will naturally be behind.

          Adding `z-index` allows us to control layering: the higher the number the higher the layer & the closer to you.
      - num: 17
        text: |
          Start at grid line 1 and extend to the last grid line (-1).
    notes: |
      *Inspect this with Firefox’s grid inspector to see the lines.*

      **Just by assigning elements to the same grid columns & rows they’ll stack on top of each other.**

  - type: interactive
    html: |
      <ul>
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
        <li>Item 4</li>
        <li>Item 5</li>
        <li>Item 6</li>
        <li>Item 7</li>
        <li>Item 8</li>
      </ul>
    css: |
      ul {
        list-style-type: none;
        padding: 0;
        display: grid;
        grid-template-columns: 1fr 1fr;
      }
    notes: |
      We don’t need to specify rows—the grid will automatically figure out the correct number of rows if we don’t specify them.

  - content: |
      ## Videos & tutorials

      - [CSS grids ➔](/topics/css-grids/)
      - [CSS grid cheat sheet ➔](/topics/css-grid-cheat-sheet/)
---
