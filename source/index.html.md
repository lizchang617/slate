---
title: API Reference

language_tabs:
  - shell
  - markdown
  - markup

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/tripit/slate'>Documentation Powered by Slate</a>

includes:
  - publish

search: true
---

# Setting Up Slate

Fork the [Slate](https://github.com/lord/slate) repository on Github by clicking the fork button on the top right corner.
Open your terminal and run the following command lines

To clone and start slate locally, use these command lines:

``` shell
# Clone your forked repository (not our original one) to your hard drive
git clone https://github.com/lizchang617/slate.git
# go into your slate directory
cd slate
# Initialize and start Slate locally
bundle install
bundle exec middleman server

```

You can now see the docs at http://localhost:4567.

# Editing Slate Markdown

Check out the following links for Documentation in Markdown:
  - [Markdown syntax used in Slate](https://github.com/lord/slate/wiki/Markdown-Syntax)
  - https://daringfireball.net/projects/markdown/
  - http://www.markdowntutorial.com/

Open your Slate folder in a text editor of your choice, and navigate to the *index.html.md* file located in **Slate>source** to start editing your markdown file.

## Adding Pages

You can add pages in the *includes* folder located under **Slate>source**. Make sure you add an underscore("_") before the name of the page. To reference the page, input the following code in your *index.html.md* file

``` markdown
includes:
  - errors
  
```

