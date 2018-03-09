---
layout: post
title: Setting up github pages in 2018
---

I know I know, I'm a little late to the party. [Github pages](https://pages.github.com/)
has been around for a fairly long time already. Easy personal website to showcase
yourself or your project powered by [Jekyll](http://jekyllrb.com).

### Let's jump straight to it

First, you'll need to create a new repository in Github following the format
*username*.github.io. It'll need at least an `index.html`, then you will be able
to publish as a Github page. [Documentation](https://help.github.com/articles/configuring-a-publishing-source-for-github-pages/)
helps too.

<img src="/public/post-images/2018-03-09-site-published.png"/>

### Choosing a theme

There are several ways to pretty up your github page. Github comes with a few Jekyll themes
you can choose from. Try them out by going to *Settings* in your repo tab, and
select *Choose a theme*

<img src="/public/post-images/2018-03-09-settings-tab.png"/>

<img src="/public/post-images/2018-03-09-theme-button.png"/>

<img src="/public/post-images/2018-03-09-select-theme.png"/>
Choose a theme you like and *Select theme*.

### Alternative way - Use a template

Another way to get themes is to fork it from other people who have made their Github pages.
For example [Hyde](https://github.com/poole/hyde) is a Jekyll theme made by [@mdo](https://github.com/mdo),
Art Director of Github.

Fork the theme and rename it to your *username*.github.io, then modify it as much as you like.

### Setting up _config.yml
Some dependencies have been deprecated in Jekyll 3.0, so you'll have to make sure the `_config.yml`
is working as it should. A good template/theme will allow you to change variables
easily in 1 config file.

it should look something like this:

{% highlight yaml %}
    # Dependencies
    markdown:         redcarpet
    highlighter:      rouge

    # Permalinks
    permalink:        pretty

    # Setup
    title:            Jellene Khoh
    tagline:
    description:      'Mashpotato & Rye'
    url:              https://jellene4eva.github.io
    baseurl:          /

    author:
      name:           'jellene4eva'
      url:            https://jellene4eva.github.io

    paginate:         5

    # Custom vars
    version:          0.0.1

    github:           https://github.com/jellene4eva
    linkedin:         https://www.linkedin.com/in/jellene-khoh-297571a3/
{% endhighlight %}


Aaaannnddd that should be it. Lycka till, happy typing!
