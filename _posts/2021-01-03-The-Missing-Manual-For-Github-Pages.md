---
layout: post
title: The Missing Manual For Github Pages
categories: ["Github Pages", "jekyll"]
---

![Github Pages](/images/Github-Pages.jpg)

Blog — a living fossil on the internet. Nowadays, people are immersed in short videos, let alone images and tweets. For writers striving for impact, social publishing platforms like [Medium](https://medium.com/) would be a better choice. But in the eyes of engineers, **their code syntax highlighting sucks**, and provide only limited config options. That’s why I can’t give up on a stand-alone blog. However, renting a VPS or using a cloud platform is breaking a butterfly on the wheel. [Github Pages](https://pages.github.com/) is just fine, though **its document is a mess**.
<!--more-->

# Launch your blog with a remote theme

First of all, you definitely want beautiful [Jekyll themes on Github](https://github.com/topics/jekyll-theme) instead of boring [default themes](https://pages.github.com/themes/). But the official “[Creating a Github Pages site with Jekyll](https://docs.github.com/en/free-pro-team@latest/github/working-with-github-pages/creating-a-github-pages-site-with-jekyll)” leads you down the wrong path — You don’t need to create a new site in your repo using Jekyll or bundle because this will generate useless stuff from a default theme. You only need 5 steps:

1. Create an empty repo named *<your Github username>.github.io* on Github as **your blog repo**. [Don’t fork a theme repo as your blog¹](https://matthiaslischka.at/2018/12/03/github-jekyll-best-practice/).
2. Choose a Jekyll theme on [Github](https://github.com/topics/jekyll-theme). Remember, it should be a [gem-based theme²](https://jekyllrb.com/docs/themes/).
3. **Fork it so you won’t be surprised when the author’s done something crazy³.** Now you get a *<your Github username>/<theme name>* as **your theme repo**.
4. Copy *_config.yml*, *Gemfile* and *index.html* from your theme repo to your blog repo. Add `remote_theme: <your Github username>/<theme name>` in *_config.yml*; add `gem “jekyll-remote-theme”` in Gemfile; add `jekyll-remote-theme` to the *plugins* section of *_config.yml*.
5. Add a *_posts* folder in your blog repo for articles. You can add markdown files named like `2021–01–03-Hello-World.md`.

Now a personal blog is served at *<your Github username>.github.io*. If you want to specify a custom domain, go to your blog repo’s settings on Github.

# Customize your blog and test it locally

In general, the above steps would be enough. But every theme may have its particular problems, and you need to customize the blog title and other stuff soon — push to Github every time for testing is time-consuming.

You can clone your blog repo to the local computer, and then install [bundler](https://bundler.io/) to manage gems locally:

- Executing `bundle exec jekyll serve` in the blog repo could preview the blog on your laptop. 
- If there is an error, fix them according to the error message. 
- Edit *_config.yml* to configure options.
- **Create folders and files with the same name as in your theme repo to override them as you please**.

------

[1] It will be very hard if you want to change that afterward. And it’s better to separate your content from the presentation.

[2] Usually, this kind of theme has an *assets* folder to store CSS and Javascript files.

[3] You can always sync updates from the original repo.

Cross-posted on [Medium](https://beyondchaos.medium.com/the-missing-manual-for-github-pages-be825f4272b1).