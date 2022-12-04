---
layout: lesson
title: "Verbalizing code"
desc: "A quick primer on reading code & learning to speak code—helps with cognition and memory."
playlist: verbalizing-code

hide_markbot: true
hide_show_for_marks: true

steps:
  - title: "Code is words"
    before: |
      First & foremost, the code we write is for human beings. It’s for humans to consume. It’s for humans to updates. And it’s for humans to understand.

      *We need to be able to read the code to better understand what it’s try to accomplish.*

      Learning to read our code correctly can help our brains understand how to apply the code—and especially help us remember the code.

  - title: "Glossary"
    before: |
      When it comes to HTML, here are a few keywords you should remember when speaking out your code.

      - **Tag** — the primary driver of HTML’s code syntax, a word starting with `<` and ending with `>`, e.g. `<h1>`, `<ul>`, `<article>`
      - **Open tag** — the part that begins HTML content, starts with `<`, has one or more words, and ends with `>`, e.g. `<p>`, `<div>`, `<time>`
      - **Close tag** — the part that finalizes the chunk of HTML content, starting with `</`, then *1* word, then `>`, e.g. `</p>`, `</div>`, `</time>`
      - **Attribute** — extra, meta information, stored inside the open tag—never in the close tag, e.g. `class=""`, `src=""`
      - **Element** — is a shortform way to say the open tag, its attributes, all the content inside, and the close tag. Some elments only have an open tag, like `<img>`
      - **Document** — the whole contents of the HTML file, all the code, all the content.
      - **Head** — the meta information stored within the open & close `<head>` tags.
      - **Body** — the HTML document’s content, stored between the open & close `<body>` tags.

  - title: "Pronouncing tags"
    before: |
      When pronouncing a tag, read its name and whether it’s an open or close tag:

      - `<h1>` — “Open H.1. tag”
      - `</h1>` — “Close H.1. tag”

      Sometimes it makes sense to expand the tag’s name when reading it:

      - `<img>` — “Image tag”
      - `<abbr>` — “Abbreviation tag”

      But I probably wouldn’t expand some tags:

      - `<div>` — I’d say, “Div. tag” instead of “Division tag”
      - `<ol>` — I’d say, “O.L. tag” instead of “Ordered list tag”

      **Though, when learning, it would be very helpful to read the full tag to help remember.**

  - title: "Pronouncing attributes"
    before: |
      When pronouncing attributes, all you have to say is the attribute name, and maybe “equals”—it’s not really helpful to speak the quotation marks.

      - `class="big"` — “Class equals big”
      - `datetime="2058-10-28"` — “Date time equals 2058 dash 10 dash 28”

      Sometimes, like HTML tags, it’s helpful to speak the full word:

      - `src="/images/dino.svg"` — “Source equals slash images slash dino dot S.V.G”

      Usually you’d announce the attribute immediately after the open tag:

      - `<img src="/images/dino.svg"` — “Image tag, source attribute equals slash images slash dino dot S.V.G”

  - title: "Example reading HTML content"
    before: |
      Have a listen & watch of me reading out a chunk of HTML code. *Then below you can do some practice.*
    video: "https://video-assets.learntheweb.courses/verbalizing-code/1-example-html.mp4"

  - title: "Practice chunks"
    before: |
      Here are a couple blocks of code for you to practice reading. *They have companion spoken versions for you to hear.*
    multi_code:
      - code_file: "comment.html"
        code_lang: "html"
        code: |
          <h2>Comments</h2>
          <ol>
            <li>
              <article>
                <h3>Stegosaurus</h3>
                <time datetime="2054-04-04">April, 4, 2054</time>
                <p>These humans are so weird—they were so boring looking without back plates or feathers.</p>
              </article>
            </li>
          </ol>
        lines:
          - num: 1
            text: |
              [Listen to this piece of code being read out.](https://www.youtube.com/watch?v=rD9IxqnRkgM&list=PLWjCJDeWfDdfEm-CIR9zUtOoD_7Ywgu4I&index=3&t=0s)
      - code_file: "navigation.html"
        code_before: |
          Here’s another block of code to practic reading.
        code_lang: "html"
        code: |
          <nav>
            <ul class="nav">
              <li>
                <a href="/dinosaurs">Dinosaurs</a>
                <ul class="sub-nav">
                  <li><a href="/dinosaurs/plant-eaters">Plant-eaters</a></li>
                  <li><a href="/dinosaurs/meat-eaters">Meat-eaters</a></li>
                  <li><a href="/dinosaurs/omnivores">Omnivores</a></li>
                </ul>
              </li>
              <li>
                <a href="/pterasaurs">Pterasaurs</a>
              </li>
              <li>
                <a href="/plesiosaurs">Plesiosaurs</a>
              </li>
            </ul>
          </nav>
        lines:
          - num: 1
            text: |
              [Listen to this piece of code being read out.](https://www.youtube.com/watch?v=0bfoPRCwmtY&list=PLWjCJDeWfDdfEm-CIR9zUtOoD_7Ywgu4I&index=4&t=0s)
    after: |
      **Keep practicing reading and speaking code.** You’re going to have to record yourself reading code for assignments in the future.
---
