# Catalyze Engineering Blog

![status](https://codeship.com/projects/47c697e0-2408-0133-22b1-2235479d6523/status?branch=master)

![Cover Image](http://i.imgur.com/7U90qCR.png)

### Prerequisites

- Ruby
- Bundler
- Sass

### Local Setup

- Clone this repo, `git clone https://github.com/catalyzeio/catalyze-engineering-blog.git`
- Navigate to this repo, `cd catalyze-engineering-blog`
- Install gems, `bundle install`
- Run the server, `rake run`
- View the site locally, `http://localhost:2113`

### Writing Guide

Engineers are required to write a blog post at the conclusion of each project or at their own discretion throughout the course of a project. Topics are entirely up to each individual but should focus on some technology being used at Catalyze or of interest to the engineer.

There are no hard requirements for blog posts, but they should be grammatically correct and intriguing to read.

Engineers are encouraged to mix up posts between long form articles detailing an entire project to short snippets and tutorials.

Posts can include media such as images, video and audio. The requirements for those are outlined below.

#### The following instructions detail how to create and publish a new post:

_Once you have the repository cloned, have pulled/checked out `master` and running locally you'll want to create a new branch for your post:_

```
$ git branch draft-<lastname>
$ git checkout draft-<lastname>
```

If you have two drafts going at once you'd simply add a number after `draft`:

```
$ git branch draft2-<lastname>
```

Now that you're on a new branch you can start writing your post. Below is a template for new blog posts:

```
---
title:
date: yyyy-mm-dd
author:
author_full:
author_alt:
tags:
---
```

**`title`:**
Corresponds to whatever you want to name your blog post. It does not have to match the file name.

**`date`:**
Should correspond to the date the article is intended to be published. It should also match the date in the file name. If it does not match the date in the file name the build will fail.

**`author`:**
Corresponds to an image of the author. This bit should be your first name only and all lowercase.

**`author_full`:**
The full name of the author that wrote the article. Whatever is written here will be displayed with the post next to the image corresponding to author.

**`author_alt`:**


#### Media requirements

**Images:**
Images should always be optimized and saved for the web. It's not reasonable to expect every engineer to have a copy of photo editing software on their machine. Therefore we encourage the use of free tools such as [kraken.io](https://kraken.io/web-interface). If engineers require graphics for their post they may reach out to any designer at Catalyze for assistance.

**Audio:**
Engineers are encouraged to use [SoundCloud](https://soundcloud.com/) for audio snippets.

**Video:**
Videos can be taken either with QuickTime and uploaded to YouTube or with [Quickcast](http://quickcast.io/).

### Publishing

Publishing is handled by Codeship. Any push to master results in a deployment to the blog server.