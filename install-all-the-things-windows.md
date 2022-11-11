---
layout: lesson
title: "Install all the things!"
desc: "Set up your computer, install all the different web browsers, install a code editor, and set up GitHub Desktop."

hide_markbot: true

important:
  title: "Windows-specific tutorial"
  text: |
    If you have a MacOS-based computer jump to the correct lesson.

    [**☛ Go to the MacOS installation tutorial.**](/courses/web-design-1/install-all-the-things/)

steps:
  - title: "Configure File Explorer"
    before: |
      Let’s change a few settings on your computer to make development life easier.

      ![](file-explorer.jpg)

      1. Go to a folder.
      2. Go to the “View” tab.
      3. Make sure “File name extensions” is checked.

  - title: "Install Firefox"
    before: |
      We need to install a bunch of browsers because, as web designers, we don’t know what browser someone will be using—so we need to test our websites in all of them.

      ![](firefox.jpg)

      1. Go to Mozilla’s website and [download Firefox](http://getfirefox.com/).
      2. Run the installer on your computer by double clicking.
    notes:
      - label: "Warning"
        text: "Make sure to only download Firefox directly from Mozilla—other websites may inject malware."

  - title: "Install Chrome"
    before: |
      ![](chrome.jpg)

      Go to Google’s website and [download Chrome](https://www.google.com/chrome/).
      <br>*(Ditto steps above.)*

    notes:
      - label: "Warning"
        text: "Make sure to only download Chrome directly from Google—other websites may inject malware."

  - title: "Install Opera"
    before: |
      ![](opera.jpg)

      Go to Opera’s website and [download Opera](https://www.opera.com/).
      <br>*(Ditto steps above.)*

    notes:
      - label: "Warning"
        text: "Make sure to only download Opera directly from Opera—other websites may inject malware."

  - title: "Get HTML files to open properly"
    before: |
      This will make it so double clicking HTML files opens your browser instead of a code editor.

      ![](properties.jpg)

      1. <a href="fixer.html" download="fixer.html">Download this HTML file.</a>
        *(If clicking this link doesn’t download the file, `Right Click > Download Linked File`.)*
      2. Go to where it was downloaded and right click—press “Properties”.
      3. Under the “Opens with” section, click the “Change…” button and set it to “Firefox” or “Chrome”.
      5. Close the properties window and trash the HTML file.

  - title: "Install GitHub Desktop"
    before: |
      We need to install the GitHub Desktop application so that we can manage and upload our code to GitHub.

      1. Download the app from the [GitHub Desktop](https://desktop.github.com/) website.
      2. Double click the installer and let it do its thing.
      3. Sign in with your GitHub username, email address, and password.

  - title: "Install the Command Line Tools"
    before: |
      We need to install some extra development tools on our computer so Markbot can work well.

      **Go to [Git’s download page](https://git-scm.com/download/win) and download the Windows version.**

      Install Git onto your computer. One of the setup screens has options we have to change.

      *On the “Adjusting your PATH environment” screen, switch to “Use Git from the Windows Command Prompt”.*

      ![](git.jpg)

  - title: "Install the Java Developer Kit"
    before: |
      We need to install the OpenJDK because the automated marking program, Markbot, needs access to Java for performing some of it’s tasks.

      Go to the OpenJDK download page on [Adopt OpenJDK](https://adoptopenjdk.net/) website.

      ![](jdk.jpg)

      **Choose the “Open JDK 11 (LTS)” version of OpenJDK at the bottom of the list.**

      1. Download the JDK for your computer.
      3. Double click the installer and let it do its thing.
      5. Delete the downloaded file.

  - title: "Install Markbot"
    before: |
      All of the coding exercises we do in this class will be using Markbot to automatically grade your work. So, we need to set that up.

      1. Download [Markbot](https://assets.learntheweb.courses/markbot/Markbot%20Setup.exe). (*or [Markbot for Mac](https://assets.learntheweb.courses/markbot/Install%20Markbot.dmg)*)
      3. Double click the installer and let it do its thing.
      5. Delete the downloaded file.

      **Open up Markbot and sign in with your GitHub username.**

      *If Markbot gives you an “Unidentified developer” security warning—click the “More info” link and press “Run anyways”.*

      ![](markbot.jpg)

      ### Add your Progressinator API key

      Go back to your browser tab with your Progressinator profile & copy & paste the API key into Markbot:

      ![](markbot-api-key.jpg)

      **Then “Sign-in” to Markbot.**

  - title: "Final checklist"
    before: |
      Double check you’ve installed everything on your computer.

      *Here’s a checklist to help out:*
    tasks:
      - "Configure File Explorer"
      - "Firefox"
      - "Chrome"
      - "Opera"
      - "Get HTML files to open properly"
      - "Create a GitHub account"
      - "GitHub Desktop"
      - "Command Line Tools"
      - "Java Developer Kit"
      - "Markbot"
---
