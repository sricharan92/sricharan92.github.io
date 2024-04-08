---
title: "Getting started with GitHub Pages"
status: publish
type: post
classes: wide
toc: true
---

**This page will be updated and refined as I learn more about GitHub Pages + Jekyll**

I have been thinking about starting a blog for a long time now and realised it is time I just took that step and see where it takes me. Much better than thinking of all the possibilities, getting overwhelmed and doing nothing — hopefully. 

### The basics

For blogging, I decided to go with [GitHub Pages](https://pages.github.com) + [Jekyll](https://jekyllrb.com). For creating this website, I learnt a lot from [Jekyll's Documentation](https://jekyllrb.com/docs/).

GitHub Pages is a tool to build websites without a lot of the know-how of building them. I don't need to maintain databases or have knowledge of front end design languages like `css` and `javascript`. Jekyll is a tool that helps abstract the user from the backend even further. It helps convert plain text (usually in markdown) to beautiful web content. 

I found it useful to start by choosing a theme first. The theme I am presently using here is [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes). Apart from the design aspects set as defaults, a theme also usually allows you to modify a lot of parameters. These options could be general for the website or for a particular type of page like a **post**.  ****A general option could be if you want a 'dark' version or 'light' version of the theme. All of these general options and defaults for different pages are set in `_config.yml` which is one of the most important files for your website.  

The `_config.yml` is written in [YAML](https://en.wikipedia.org/wiki/YAML). YAML is a neat way to organise a dictionary, hash or a structure. It uses indentation to create subfields. The following is an example of some YAML code. 

```yaml
# Defaults
defaults:
  # _posts
  - scope:
      path: ""
      type: posts
    values:
      layout: single
      author_profile: true
      read_time: true
      comments: # true
      share: true
      related: true
```

The above snippet, taken from my `_config.yml` file, defines the defaults for pages of type `posts`.  

I installed my present theme as a **gem**. A gem is a software package that can be easily installed and used for your project. Installing my theme as a gem abstracts me from the files that the theme might require to function, for example, the css files, layout files, among other things. Since I don't have the files pertaining to the theme locally, being up-to-date with the present version of the theme also becomes incredibly simple. I just have to update the gem 🙂. You put all the gems you want installed for your website in a `Gemfile` and then use a gem called `bundler` to install or update them all at once. Pretty neat! 

To get your website up and running quickly using minimal mistakes, it's a good idea to start with their [starter template](https://github.com/mmistakes/mm-github-pages-starter). This will get you up and going pretty soon and save you a LOT of googling (speaking from limited experience...)

### Creating a post

Posts have to be named in a particular format that helps Jekyll parse it properly. The format is `yyyy-mm-dd-title-of-post.md`. This has to be placed in the `_posts` folder for Jekyll to categorise it as a post. By default, in my case, the layout and other fields are set in the `_config.yml` file as shown before. Although, if I want to change it, I can do this by including the changes on the top of the post's markdown file as follows: 

```yaml
---
layout: single
author_profile: false
---
```

The '—-' tell Jekyll to parse it differently and not as part of the post.

### Testing your website

You should typically test your website locally before you host it online. This is good for two reasons: 

1. It does not break the already hosted website
2. The hosted website takes a while to get updated after you push it 

TIP: It typically takes a couple minutes for the changes to reflect on your webpage. 

To test the website locally, run `bundle exec jekyll serve`. Once it builds without errors, you can access your website at `127.0.0.1:4000` 

### Push to production

Once you are satisfied with the updates you've made, commit those changes to your repository and the changes will be reflected at `[username.github.io](http://username.github.io)` 🙂

There is probably a lot more that I need to explore and a lot of unknown unknowns as well. Hopefully the fog will clear up as I keep writing here and updating this website! 

### Issues

*Theme changes reflect in the local server but not after pushing it*: 
This takes ~10 minutes to update on the website. 

Cheers, 

Sricharan