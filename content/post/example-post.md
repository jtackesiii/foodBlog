---
title:  Example Post
date: 2020-05-19
tags: ["yams", "begonias"]
---

Welcome to your new blog!

There are a few things you should familiarize yourself with before you begin blogging. I've broken up this post into several sections to help get you started.

### Making New Posts

Hugo is a website generator that turns markdown (.md) files into web pages. So each "post" of your blog will be a separate markdown file. If you haven't already, locate and open this file in your text editor (Atom). If you navigate to content > post, you should see "example-post.md". That file is what you are reading in your browser!

There are three things to pay attention to when creating a new post.

1. Photos folder or Post folder? For now, we'll create a new post in the "post" folder. This will be where all of your posts go that do not contain _galleries_ of photos (I have given you instructions about making photo gallery posts below, so don't worry).
2. Correct filename. When you create a new file in the "post" folder, you have to ensure that you _include the proper file extension_ for a markdown file. Try creating a new file, naming it "my-first-blogpost.md".
3. Your blogpost must contain _frontmatter_; that is, some information that the website uses to sort it. Notice the very top of this file in your text editor. There are "title," "date," and "tags" fields, sandwiched between two sets of three dashes (-\-\-\). That formatting is very important. It may be easiest to copy-paste lines 1-5 of this file into your new markdown file, changing the title, date, and tags to your preferences.

That's all you need to start making new blog posts! But you may have noticed that the text in this markdown file looks different from the webpage. Next, I'll walk you through how to write stylish posts in markdown files.

### Using Markdown

You won't be coding at all in order to add new content to your blog -- in many ways, this blog will be easier to manage than if you used wordpress or wix! The majority of what you need to _learn_ in order to write attractive blog posts is how to format text in markdown files.

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

You should always separate two paragraphs of text with a blank line in markdown. If you don't formatting issues can ensue. For the same reason, a markdown file should always end with a blank line.

#### Adding Photos

Adding photos is easy, but your markdown file will look different from your web page. To add a photo, you need to do two things:

1. Place the photo file in the "static" folder. **Do NOT place it in the "photos" folder -- that will be for your photo galleries** (I will teach that to you below).
2. Write a **shortcode** in your markdown file. You'll notice that in the markdown file, there is a funny line of text wrapped in "{{" "}}" symbols. Hugo transforms that text into your image on the web.

For example, I have placed this incredible photo of you in the "static" folder:

{{< figure src="/old-radio-pic-of-angie.jpeg" caption="You're so cute!" >}}

> **Note that the file name and file extension are CASE-SENSITIVE!**

You can copy-paste this shortcode into future posts, changing the filename and the caption text as needed.

#### For Photo Galleries

You may have noticed that there is a separate "photos" folder above "posts." If you want to make a post that is primarily photos, Hugo can turn them into a lovely photo gallery for you. This is really easy to do, but there is one trick. You need to create a folder inside of "photos" to represent your photo-gallery blog post. Navigate to the "photos" folder and you will see a "sample-photo-gallery" folder. Inside are several pictures and a markdown file named "index.md". Hugo is smart enough to put all of the photos inside of the "index.md" file, but only _if_ the file is named "index" -- that's the trick.

Try making a new folder for a photo gallery of your own. Put some photo files inside and then make a new "index.md" file. There's only one more step!

For photo galleries, there are a few additional pieces of information to specify in the _frontmatter_. Take a look at the "index.md" file inside of the "sample-photo-gallery" folder. You'll notice that there are fields for "location," "display_date," "footer," and "banner." Let me explain what these mean:

**location**: This refers to where the photos were taken. It's an optional field, and you can leave it blank if you like.

**display_date**: Since your photo gallery may pre-date your blog post, and the photos may have been taken on various days, you can add a custom date here. This date won't affect how your blog post is sorted on the website, but the regular "date" field will, so be careful!

**footer**: By default, all of the text of your blog post will come before your photo gallery. If you want to create text _below_ the gallery, you can do so in the footer section of the frontmatter. All of the same Markdown rules apply when adding the footer, but _you have to make sure that all of the text is indented once_ -- otherwise your whole website will crash!

**banner**: Do you want one photo from your gallery to be visible on the home screen inside the blurb for your photo gallery post? If so, specify one of your gallery photos to use as a banner.

That's it! Enjoy your food blog!
