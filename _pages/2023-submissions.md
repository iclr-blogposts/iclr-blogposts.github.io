---
layout: page
title: Submission and Writing Workflow
permalink: /2023/submissions
description:
nav: true
nav_order: 2
---

For this edition of the Blogposts Track, we will forgo the need for total anonymity. We will allow
authors to render their posts on their own repositories. In our opinion, this still follows the 
Double-Blind reviewing principle: it is no less double-blind than when reviewers are asked to score papers
that have previously been released to Arxiv, an overwhelmingly common practice in the ML community.
The reason we are choosing to do things this way is to lower the burden on both us and the authors: last
year, **many** submissions had to be reworked because their relative links were broken. This year, 
by allowing the authors to render their websites on Github's servers prior to merging their changes into this website, 
we hope to avoid this issue entirely.

The workflow you will use to participate in this track should be relatively familiar to you if you are
familiar with [Github Pages](https://pages.github.com/). Specifically, our website is based off of 
[AL-Folio](https://github.com/alshedivat/al-folio). This template uses Github Pages as part of its 
process, but it also utilizes a separate build step using 
[Github Actions](https://github.com/features/actions) and intermediary 
[Docker Images](https://www.docker.com/).

**We stress that you must pay close attention to the steps presented in this guide. Small mistakes
here can have very hard-to-debug consequences.**

# Setup & Writing workflows

1. First and foremost, [import this repository](https://github.com/iclr-blogposts/iclr-blogposts.github.io) using GitHub's [repository import feature](https://github.com/new/import). 
2. Rename your import following GitHub pages' [instructions](https://pages.github.com/). Namely, you probably should rename it
    using a personalized name. **This is a "project" website**, not a "user" website.
3. Follow the [`Deployment` instructions](https://github.com/iclr-blogposts/iclr-blogposts.github.io/blob/master/README.md#deployment) in the ReadMe
    **to the letter**. Pay particular attention to the instructions detailing how you must edit the `_config.yml`.
4. To render your website locally, follow the [`Local setup using Docker (Recommended on Windows)` instructions](https://github.com/iclr-blogposts/iclr-blogposts.github.io/blob/master/README.md#deployment).
    **If you are having trouble accessing your own website because you are getting redirected to this url: [https://iclr-blogposts.github.io/2023/about](https://iclr-blogposts.github.io/2023/about),
    try directly visiting `<your website url>/2023/about`.

# Submission workflow

1. Make a new Pull Request from your