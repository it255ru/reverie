# Build A Blog With Jekyll And GitHub Pages

## What Is Jekyll?

Jekyll is a website generator that’s designed for building minimal, static blogs to be hosted on GitHub Pages.

In this article we’ll walk through the following:

* the quickest way to set up a Jekyll powered blog;
* how to avoid common problems with using Jekyll;
* how to import your content from WordPress, use your own domain name, and blog in your favorite editor;
* how to theme in Jekyll, with Liquid templating examples;
* a couple of Jekyll 2.0’s new features, including Sass and CoffeeScript support and collections.

## Creating Post Files

To create a new post, all you need to do is create a file in the */_posts* directory. Jekyll requires blog post files to be named like these:

    2011-12-31-new-years-eve-is-awesome.md
    2012-09-12-how-to-write-a-blog.markdown

## Content

All blog post files must begin with YAML Front Matter.

To improve the user experience for both reading and writing posts, TeXt made some enhancements for markdown and some additional styles.

### YAML Front Matter

    ---
    layout: article
    title: Document - Writing Posts
    mathjax: true
    ---

Between these triple-dashed lines you can set variables. you can consider it as page configuration, these would overrides the global configuration in *_config.yml*.

Beside Jekyll’s predefined variables, TeXt define some new variables for each layouts, see [Layouts](https://tianqi.name/jekyll-TeXt-theme/docs/en/layouts) for details.
