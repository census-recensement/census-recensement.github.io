# Census-Recensement Editing Instructions

## How this site works

This site is rendered by Jekyll. [Alex Gil has written a descriptive tutorial on Jekyll](https://www.chronicle.com/blogs/profhacker/jekyll1/60913), but in a nutshell, Jekyll is a 'static site generator' that relies on templates, metadata, and simplified code.

* [Markdown](#markdown)
* [Front Matter](#front-matter)
* [Liquid Tags](#liquid-tags)
* [General Formatting](#general-formatting)
* [Submitting Your Edits](#submitting-your-edits)

### Markdown

GitHub pages are primarily written in Markdown--a simplified markup language that turns plain text into html. There are a number of different 'flavours' of Markdown; this site is written in Kramdown. Here's a [Kramdown Cheat Sheet](https://kramdown.gettalong.org/quickref.html). Markdown files can be created right in GitHub, or written in your favourite text editor. They **must** be saved with the extension `.md`.
*(fun fact: this README is written in [GitHub flavoured Markdown](https://help.github.com/en/articles/basic-writing-and-formatting-syntax), which doesn't have as many options as Kramdown...especially when it comes to the table of contents. Make sure you specify Kramdown if you are searching outside tutorials!)*

### Front matter

Each page **needs** to start with [YAML front matter](https://jekyllrb.com/docs/front-matter/). The site won't publish a page without it. Basically, this is metadata that provides information to Jekyll on how to render the page. It looks like this:

~~~~~
---
layout: post
title:  Hello World!
date:   2018-10-04
categories: tutorial
tags: website
      jekyll
      library
lang: en
ref: hello
---
~~~~~

There are more options available for metadata at the link above, but I'll break down what's here.

- **layout**
    - this tells Jekyll which layout to use, based on pre-defined designs. The most common layouts will be `page` and `post`. Posts are only used for *News* items and **require** a date in the filename, formatted like this: `2018-10-05-hosting.md`. Pages don't need a date, but keep the filename simple and direct. These pages will rely on templates that provide items like menus and footers. The templates rarely need to be changed, but they often have names like `default` or `layout`. This **is** a mandatory field.
- **title**
    - this is the title of the document. This title will appear in the header information (meaning it'll display the title in the browser tab). You can also 'call' on this title to have it display in the body of the page itself or in other places using something called a 'liquid tag'. More on that later :) This **is** a mandatory field.
- **date**
    - this is the date the document was created. Like titles, this date field can be called on in the body of the text, and other places.
- **categories**
    - this describes the content of the page. There should be fewer categories than tags, and generally a page should only fit into *one* category, though multiple categories can be assigned. Categories can be called on to generate dynamic lists on other pages, populate menus, or just generally help to organize information. Categories can also be used to custommize the URL. For example, the URL for this page could be `http://census-recensement.github.io/tutorial/hello-world`. If the page has no set category, the URL would look like this: `http://census-recensement.github.io/hello-world`. This is **not** a mandatory field.
- **tags**
    - another way of describing the page. Pages can have multiple tags, just make sure to format them as they are in the example above. This site has a search function that uses tags. They're handy! This is **not** a mandatory field.
- **lang**
    - this field is required for any page that has a translated pair. The tag can only be *en* or *fr*. These fields will trigger our language selector. This field also requires the *ref* field, described below.
- **ref**
    - this field is required, in conjunction with the *lang* tag, to 'match' an English page to a French page. The match occurs with both pages have the **same** word in the field. Using the example above, both the English and French versions of the page must have `Hello` in the *ref* field.

### Liquid Tags

This is probably the most complex part of Jekyll, but luckily, for a simple static site like this, most of the liquid tags have already been placed out-of-site in the templates. [If you want to know more, here is some basic Jekyll documentation on liquid tags](https://jekyllrb.com/docs/variables/).
*(fun fact: the Liquid language was created by Shopify!)*

One way of using liquid tags is to call information from the Front Matter. A tag like `{page.title}` in Markdown will display the title of the page. A tag like `{page.date}`will display the date listed in the Front Matter. Liquid tags can also be used for more complex coding operations, like 'for-if' loops.

### General Formatting

Markdown is really easy. Rather than listing everything here, you can check out the [Kramdown Cheat Sheet](https://kramdown.gettalong.org/quickref.html) OR you can look at the *raw* output of this readme file to see how this page has been rendered. To access that, view the file [here](README.md), and click on 'Raw' in the top right corner. You can inspect any page in this repository by looking a the raw contents. This can be especially useful when creating new pages, simply copy and paste from the raw output that you want to emulate, and then fill it in with your own text.

### Submitting Your Edits

Our repository has been set-up so that any edits need to be approved by 2 other members of the team. Don't worry, you won't be able to *accidentally* push your edits. The process for editing will be the following:

  1. navigate to the file you want to edit (or create a whole new file)
  2.  
