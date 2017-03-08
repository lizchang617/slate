---
title: API Reference

language_tabs:
  - shell
  - markdown

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/tripit/slate'>Documentation Powered by Slate</a>

includes:
  - publish

search: true
---

# Prerequisites

* Linux or OS X — Windows may work, but is unsupported.
* Ruby, version 2.2.5 or newer
* Bundler — If Ruby is already installed, but the bundle command doesn't work, just run gem install bundler in a terminal.

## Updating Ruby

You will need to update Ruby on your system. In order to do so, you will need to do the following:

1. Upgrade Your System to macOS Sierra
2. Install XCode Command Line Tools
3. Configure Git
4. Install Homebrew
5. Install GPG
6. Install RVM
7. Install Ruby
8. Update RubyGems
9. Install Rails

You can find the more detailed instructions [here](http://railsapps.github.io/installrubyonrails-mac.html)

# Setting Up Slate

Fork the [Slate](https://github.com/lord/slate) repository on Github by clicking the fork button on the top right corner.
Open your terminal and run the following command lines. To clone and start slate locally, open your terminal and run these command lines:

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

1. [Markdown syntax used in Slate](https://github.com/lord/slate/wiki/Markdown-Syntax)
2. https://daringfireball.net/projects/markdown/
3. http://www.markdowntutorial.com/

Open your Slate folder in a text editor of your choice, and navigate to the *index.html.md* file located in **Slate>source** to start editing your markdown file.

## Adding Pages

You can add pages in the *includes* folder located under **Slate>source**. Make sure you add an underscore("_") before the name of the page and make sure you save it as a markdown file. To reference the page, input the following code in your *index.html.md* file

``` markdown

includes:
  - publish

```

