---
layout: page
title: submitting
permalink: /submissions
description:
nav: true
nav_order: 3
---

# A more open process

For this edition of the Blogposts Track, we will forgo the need for total anonymity. We will allow
authors to render their posts on their own repositories. In our opinion, this still largely follows the 
Double-Blind reviewing principle: it is no less double-blind than when reviewers are asked to score papers
that have previously been released to [arXiv](https://arxiv.org/), an overwhelmingly common practice in the ML community.
The reason we are choosing to do things this way is to lower the burden on both us and the authors: last
year, **many** submissions had to be reworked because their hypertext links were broken. This year, 
by allowing the authors to render their websites on Github's servers prior to merging their changes into this website, 
we hope to avoid this issue entirely. We also avoid the issue of having to host the submissions on a separate server
during the reviewing process.

However, we understand the desire for total anonymity. Authors that wish to have a fully double-blind process might
consider creating new GitHub accounts without identifying information which will only be used for this track.

# Backend

The workflow you will use to participate in this track should be relatively familiar to you if you are
familiar with [Github Pages](https://pages.github.com/). Specifically, our website is based off of 
[AL-Folio](https://github.com/alshedivat/al-folio). This template uses Github Pages as part of its 
process, but it also utilizes a separate build step using 
[Github Actions](https://github.com/features/actions) and intermediary 
[Docker Images](https://www.docker.com/).

**We stress that you must pay close attention to the steps presented in this guide. Small mistakes
here can have very hard-to-debug consequences.**

# Setup & Writing workflows

1. First and foremost, [fork this repository](https://github.com/iclr-blogposts/staging). 
    We stress that you must fork the [staging repository](https://github.com/iclr-blogposts/staging), not the main repository.
2. Rename your fork. Namely, you probably should rename it
    using a personalized name inspired by the subject of your submission. **This is a "project" website**, not a "user" website.
3. Follow the [`Deployment` instructions](https://github.com/iclr-blogposts/staging/blob/master/README.md#deployment) 
    in the ReadMe
    **to the letter**. Pay particular attention to the instructions detailing how you must edit the `_config.yml`.
4. To render your website locally, follow the
    [`Local setup using Docker (Recommended on Windows)` instructions](https://github.com/iclr-blogposts/iclr-blogposts.github.io/blob/master/README.md#deployment).
    *If you are having trouble accessing your own website because you are getting redirected to this url: [https://iclr-blogposts.github.io/2023/about](https://iclr-blogposts.github.io/2023/about),
    try directly visiting `<your website url>/2023/about`.*
5. Create a new folder in the `assets` folder. Name it after your repository name.
6. You may then add your blogpost in the `_posts` folder. You must place any accompanying pictures, HTML figures, 
    or other such data in the folder you created in Step 5. Refer to the [provided example](https://iclr-blogposts.github.io/2023/blog/2021/distill-example/).
7. Refrain from adding any identifying information.

**Should you edit ANY files other than `_config.yml`, your new post inside the `_posts` directory, and your new folder inside the `assets` directory,
your pull requests will automatically be ignored.**

# Submission workflow

1. Strip all identifying information from your blog post. It is fine if you keep your names inside comments inside the MarkDown file
2. Make a new Pull Request from your fork to the [staging repository](https://github.com/iclr-blogposts/staging). Your code will
    then be merged into the staging version of the blog
3. Submit the name of your blog post and its URL to our OpenReview [TODO LINK]

# Reviewing workflow

Reviewers will be asked to only view the live content of the blog. We ask that they act in good faith, and refrain from
digging into the repository's logs and closed Pull Requests to find any identifying information on the authors.

# Camera-ready

1. Accepted submissions will be notified
2. Authors will then add their identifying information to the blog post
3. Authors will then open a Pull Request to the [main repository](https://github.com/iclr-blogposts/iclr-blogposts.github.io)
4. The track chairs might request some changes
5. The accepted submissions will then be merged into the final blog
