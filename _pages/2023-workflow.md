---
layout: page
title: Submission and Writing Workflow
permalink: /2023/workflow
description:
nav: true
nav_order: 2
---

For this edition of the Blogposts Track, we will forgo the need for total anonymity. We will allow
authors to render their posts on their own repositories. In our opinion, this still follows the 
Double-Blind reviewing principle: it is no less double-blind than when reviewers have to score papers
that have previously been released to Arxiv, an overwhelmingly common practice in the ML community.
The reason we are choosing to do things this way is to lower the burden on both us and the authors: last
year, **many** submissions had to be reworked because their relative links were broken. This year, 
by allowing the authors to render their websites on Github's servers, we hope to avoid this issue 
entirely.

The workflow you will use to participate in this track should be relatively familiar to you if you are
familiar with [Github Pages](https://pages.github.com/). Specifically, our website is based off of 
[AL-Folio](https://github.com/alshedivat/al-folio). This template uses Github Pages as part of its 
process, but it also utilizes a separate build step using 
[Github Actions](https://github.com/features/actions) and intermediary 
[Docker Images](https://www.docker.com/).

**We stress that you must pay close attention to the steps presented in this guide. Small mistakes
here can have very hard-to-debug consequences.**

1. First and foremost, 
