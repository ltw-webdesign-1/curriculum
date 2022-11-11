---
layout: slide-deck
title: "Semantics map-out"
desc: "An activity to help learn the HTML semantics by working in small groups to identify pieces of content."

group_work: true

slides:
  - type: super-big-text
    content: |
      **Semantics map-out**

  - content: |
      ## What & why

      When learning to write HTML, you have to start thinking about content differently—about its purpose and meaning.

      Using some pre-written content we’ll go through, learn & discuss how & why choose HTML tags.

      **With some practice, and some memorization, we can grasp what content HTML describes.**

  - content: |
      ## Set up

      1. Form into pairs
      2. [Download the files](https://github.com/ltw-webdesign-1/semantics-map-out/archive/master.zip)
      3. Print “content.pdf” and draw on the paper
        <br>Or do the whole thing digitally

  - content: |
      ## Instructions

      1. You’ll be shown some HTML tags & their purposes
      2. Find content that’s appropriate for those tags
      3. Mark that content with the tag name
        <br>*You don’t need to write full HTML or even tags—just the tag names—something as simple as `h1`*

  - content: |
      ## 1 Content elements

      - Heading
      - List
      - Image
      - Paragraph

      *Not actually tags. But let’s start with grouping content types.*

  - type: image
    image: content.jpg

  - content: |
      ## 2 Heading elements

      *Each number denotes a sub-heading of the heading above.*

      `<h1>` `<h2>` `<h3>` `<h4>` `<h5>` `<h6>`

  - type: image
    image: headings.jpg

  - content: |
      ## 3 List elements

      `<ul>` — Unordered list
      <br>`  <li>` — Each individual item inside

      `<ol>` — Ordered list
      <br>`  <li>` — Each individual item inside

      `<dl>` — Description list
      <br>`  <dt>` — The item title
      <br>`  <dd>` — The item description

  - type: image
    image: lists.jpg

  - content: |
      ## 4 Image elements

      `<img>`
      <br>— A visual image

      `<figure>`
      <br>— An image with a caption, wraps an image

      `<figcaption>`
      <br>— The descriptive text inside a figure

  - type: image
    image: images.jpg

  - content: |
      ## 5 Quote elements

      `<q>` — Small quotes inside other text

      `<blockquote>` — Large, stand-alone quotes

      `<cite>` — The source of the quote

  - type: image
    image: quotes.jpg

  - content: |
      ## 6 Text level elements

      `<em>` — Emphasis

      `<strong>` — Lots of emphasis

      `<b>` — A keyword

      `<i>` — Another language, technical term, title

  - type: image
    image: text-level.jpg

  - content: |
      ## 7 Link elements

      `<a>` — A clickable hyperlink

  - type: image
    image: links.jpg

  - content: |
      ## 8 Document elements

      `<header>` — The most important information
      <br>`<nav>` — The navigation for the page
      <br>`<main>` — The primary content
      <br>`<article>` — A chunk of unique content
      <br>`<aside>` — Secondary information
      <br>`<footer>` — The least important information

  - type: image
    image: document.jpg

  - content: |
      ## 9 Extra elements

      `<data>` — Some numerical, computer information

      `<time>` — A date or time

      `<small>` — Fine print, copyright notice

  - type: image
    image: extra.jpg
---
