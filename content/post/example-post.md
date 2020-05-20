---
title:  Example Post
date: 2020-05-19
tags: ["Example Tag 1", "Example Tag 2", "Add your own Tag"]
---

Welcome to your new blog!

There are a few things you should familiarize yourself with before you begin blogging. I've broken up this post into several sections to help get you started.

### Using Markdown

You won't be coding at all in order to add new content to your blog -- in many ways, this blog will be easier to manage than if you used wordpress or wix! The majority of what you need to _learn_ in order to write attractive blog posts is how to format text in what is called a markdown file (.md).

If you haven't already, open this file in your text editor (Atom). If you navigate to content > post, you should see "example-post.md". That file is what you are reading in your browser! Hugo converts markdown files into webpages.

A markdown file itself is a type of text file with minimal styling abilities built-in. It's not as fancy as a ".doc" file, but you won't need many of the styling features that you use in a full-fledged word processor.

#### Markdown Basics

Markdown let's you _italicize_, **bold**, add footnotes,^[Hey, a footnote!] and [hyperlinks](https://wikipedia.org). For example, if you want to quote someone else at length, you can easily include a block quote by beginning a new line with a ">" sign:

> This is a block quote. Markdown takes the ">" from our file and converts the paragraph into a block quote automatically! Isn't markdown fun?

You can add a variety of headers to your documents as well. You do this by beginning a new line with any number of "#" signs. The number of "#" signs you type represents the header level. For example:

# Header1 (#)
## Header2 (##)
### Header3 (###)
#### Header4 (####)
##### Header5 (#####)

You should always separate two paragraphs of text with a blank line in markdown. If you don't formatting issues can ensue.

#### Adding Photos

Adding photos is easy, but your markdown file will look different from your web page. To add a photo, you need to do two things:

1. Place the photo file in the "static" folder.
2. Write a **shortcode** in your markdown file.

For example, I have placed an incredible photo of you in the "static folder."

{{< figure src="/old-radio-pic-of-angie.jpeg" caption="You're so cute!" >}}

> **Note that the file name and file extension are CASE-SENSITIVE!**

#### For Photo Galleries

### Making New Files
