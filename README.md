# Build A Blog With Jekyll And GitHub Pages

## What Is Jekyll?

Jekyll is a website generator that’s designed for building minimal, static blogs to be hosted on GitHub Pages.

In this article we’ll walk through the following:

* the quickest way to set up a Jekyll powered blog;
* how to avoid common problems with using Jekyll;
* how to import your content from WordPress, use your own domain name, and blog in your favorite editor;
* how to theme in Jekyll, with Liquid templating examples;
* a couple of Jekyll 2.0’s new features, including Sass and CoffeeScript support and collections.

### THE ADVANTAGES OF GOING STATIC
* Simplicity. Jekyll strips everything down to the bare minimum, eliminating a lot of complexity:
  * **No database.** Unlike WordPress and other content management systems (CMS), Jekyll doesn’t have a database. All posts and pages are converted to static HTML prior to publication. This is great for loading speed because no database calls are made when a page is loaded.
  * **No CMS.** Simply write all of your content in Markdown, and Jekyll will run it through templates to generate your static website. GitHub can serve as a CMS if needed because you can edit content on it.
  * **Fast.** Jekyll is fast because, being stripped down and without a database, you’re just serving up static pages. My base theme, Jekyll Now, makes only three HTTP requests — including the profile picture and social icons!
  * **Minimal.** Your Jekyll website will include absolutely no functionality or features that you aren’t using.
* Design control. Spend less time wrestling with complex templates written by other people, and more time creating your own theme or customizing an uncomplicated base theme.
* Security. The vast majority of vulnerabilities that affect platforms like WordPress don’t exist because Jekyll has no CMS, database or PHP. So, you don’t have to spend as much time installing security updates.
* Convenient hosting. Convenient if you already use GitHub, that is. GitHub Pages will build and host your Jekyll website at no charge, while simultaneously handling version control.

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
