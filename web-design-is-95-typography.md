---
layout: slide-deck
title: "Web design is 95% typography"
desc: "Look over some of CSS’s text-specific properties, ways we can style text & how to make things readable."

slides:
  - type: super-big-text
    content: |
      **Web design is 95% typography**
    notes: |
      Totally ripping the title off from [IA: Web design is 95% typography](https://ia.net/topics/the-web-is-all-about-typography-period)

  - content: |
      ## Text is everywhere

      - So much of our interfaces are text label
      - Text is extremely accessible
      - Content is exceptionally important

  - content: |
      ## Typography

      *Readability on the web is critical*

      - Looser line-height than print
      - Similar line-length to print
      - Lots of breaks: headings, lists, highlights
      - Colour contrast between text & background

  - content: |
      ## CSS controls typography

      **CSS gives us lots and lots of control over typography—and it’s always getting better.**

  - type: code
    css: |
      h1 {
        background-color: #f2f1ed;      /* Colour behind text */
        color: #222;                    /* Text colour */
        font-family: Georgia, serif;    /* Suggested typeface & backup */
        font-size: 2rem;                /* Suggested size of the type */
        font-style: italic;             /* Italic or normal */
        font-weight: bold;              /* Bold, normal, or number like 200 */
        line-height: 1.5;               /* Multiplier against the size */
        list-style-type: square;        /* Bullets: none, circle, decimal, lower-alpha, etc. */
        text-align: center;             /* Left, right, center, justify */
        text-decoration: underline;     /* Underline or none */
        text-transform: uppercase;      /* Uppercase, lowercase */
      }
      img {
        width: 100%;                    /* Make the width fill the whole space */
      }

  - content: |
      ## Core typefaces

      - Arial
      - Verdana
      - Georgia
      - Times New Roman
      - Comic Sans *(um… really!?)*
      - Courier
      - Impact *(not as reliable)*
    notes: |
      We can guarantee that these typefaces will exist on every computer (as much as we can guarantee on the web).

      The only reason they exist is because Microsoft gave away all the typefaces in the early 90s to help the web be a consistent platform.

  - content: |
      ## Google Fonts

      Can’t just use any typeface available on your computer

      Google has many good typefaces (Typekit too)

      Include another CSS `<link>` tag
    notes: |
      As designers you’ll likely want to use more than just the default typefaces. That’s where online services like Google Fonts of Typekit help out. They provide large databases of properly web-licensed fonts for you to use on your website.

      You cannot just use any font that’s on your computer, like you can in print, because the user of the website would have to also have that font installed on their computer to view it properly. Not to mention the fact that almost all of the fonts on your computer aren’t licensed to be used on the web so it’d be illegal to use the in a website anyways.

  - content: |
      ## Font sizes

      Suggestions for the size to be displayed—user is always in control

      - **`rem` — scalable size based on browser settings**
      - `em` — scalable size based on parent element
      - `px` — don’t use for font-size—ever
    notes: |
      We are not—and shouldn’t be—in control of the font-size a person uses to view our website. They can increase or decrease the font-size however they want.

      Instead we specify a scale of font-sizes. Using the `rem` unit we can say that the font-size should be 1.5× larger than the body copy.

      The default font-size in browsers (assuming you didn’t change it) is `16px`. This is a nice readable size and you **should never** make the body copy small than that. So, translated to `rem`: *the body copy of your website should never be smaller than `1rem`*

  - content: |
      ## Videos & tutorials

      - [Basic typography ➔](/topics/basic-typography/)
      - [Using Google Fonts ➔](/topics/google-fonts/)
      - [Web typography cheat sheet ➔](/topics/web-typography-cheat-sheet/)

---
