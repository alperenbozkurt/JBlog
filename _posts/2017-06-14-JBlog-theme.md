---
layout: post
title:  "JBlog Jekyll Theme"
image: "http://dab1nmslvvntp.cloudfront.net/wp-content/uploads/2015/02/1424055625jekyll.png"
date:   2016-03-21
excerpt: "Simple Jekyll theme for your blog by Alperen Bozkurt."
project: true
tag:
- jekyll
- JBlog
- blog
- about
- theme
---

![jekyll Image](http://dab1nmslvvntp.cloudfront.net/wp-content/uploads/2015/02/1424055625jekyll.png)
{: .image-pull-right}

<center><b>JBlog</b> is a simple jekyll theme.</center>

## About

I have used this theme in my own php and ruby blogs.I got inspired by [taylantatli](https://github.com/taylantatli/)'s [moon](https://github.com/taylantatli/moon) and [ramme](https://github.com/taylantatli/ramme) themes to use this theme in Jekyll.

I'm not a designer or something, so I'm sure there is a better way to make this theme. But it's working and looks acceptable for different screen sizes. If something looks extremely ugly and you can't resist to fix it, just send me a PR. I will be grateful.

I see some people using this theme. I need to search on Github to find who use it. But I don't want to search like this. If you like this theme or using it, please give a **star** for motivation.

## Installation
* Fork the [Repo](https://github.com/alperenbozkurt/JBlog/fork)
* Edit `_config.yml` file.
* Remove sample posts from `_posts` folder and add yours.
* Edit `index.md` file in `about` folder.
* Change repo name to `YourUserName.github.io`    

That's all.

## Scaffolding    
How JBlog is organized and what the various files are. All posts, layouts, includes, stylesheets, assets, and whatever else is grouped nicely under the root folder.    

{% highlight text %}
├── 404.html                                    # 404 page
├── about                                       # About Page
├── assets
│   ├── css                                     # Compiled stylesheets
│   ├── fonts                                   # webfonts
│   ├── img                                     # Folder for images
│   │   ├── favicon                             # Folder for favicons
│   └── js                                      # Folder for scripts
├── blog                                        # Post list for blog
├── _config.yml                                 # Configuration file for jekyll
├── _data
│   └── navigation.yml                          # Navigation links
├── _includes
│   ├── favicon.html                            # Favicon links
│   ├── footer-home.html                        # Footer for home page
│   ├── footer.html                             # Footer for other pages
│   ├── head-home.html                          # Head for home page
│   ├── head.html                               # Head for other pages
│   ├── nav-home.html                           # Top navigation for home page
│   ├── nav.html                                # Top navigation for other pages
│   ├── open-graph.html                         # Twitter Cards and Open Graph meta data
│   ├── scripts.html                            # Site scripts
│   ├── social-links.html                       # Social links to show in homepage
│   └── toc.html                                # Table of contents to use in some posts
├── index.html                                  # Homepage
├── _layouts
│   ├── home.html                               # Home layout
│   ├── page.html                               # Page layout
│   ├── post.html                               # Post layout
│   ├── post-index.html                         # Post list layout
│   └── project.html                            # Project list layout
├── _posts                                      # MarkDown formatted posts
├── _sass                                       # Sass stylesheets
└── projects                                    # Projects list page
{% endhighlight %}   

---

## Site Setup
A quick checklist of the files you’ll want to edit to get up and running.    

### Site Wide Configuration
`_config.yml` is your friend. Open it up and personalize it. Most variables are self explanatory but here's an explanation of each if needed:

#### title

The title of your site... shocker!

Example `title: My Awesome Site`

#### url

Used to generate absolute urls in `sitemap.xml`, `feed.xml`, and for generating canonical URLs in `<head>`. When developing locally either comment this out or use something like `http://localhost:4000` so all assets load properly. *Don't include a trailing `/`*.

Examples:

{% highlight yaml %}
url: http://alperenbozkurt.net/JBlog
url: http://localhost:4000
url: //cooldude.github.io
url:
{% endhighlight %}

#### Google Analytics and Webmaster Tools

Google Analytics UA and Webmaster Tool verification tags can be entered in `_config.yml`. For more information on obtaining these meta tags check [Google Webmaster Tools](http://support.google.com/webmasters/bin/answer.py?hl=en&answer=35179) and [Bing Webmaster Tools](https://ssl.bing.com/webmaster/configure/verify/ownership) support.

---

### Navigation Links

To set what links appear in the top navigation edit `_data/navigation.yml`. Use the following format to set the URL and title for as many links as you'd like. *External links will open in a new window.*

{% highlight yaml %}
- title: Home
  url: /

- title: Blog
  url: /blog/

- title: Projects
  url: /projects/

- title: About
  url: /about/

- title: JBlog
  url: http://alperenbozkurt.net/JBlog
{% endhighlight %}

---

## Layouts and Content

Explanations of the various `_layouts` included with the theme and when to use them.

### Post and Page

These two layouts are almost similar. Only difference is page layout doesn't show date under title.

### Post Index Page

A [sample index page]({{ site.url }}/blog/) listing all blog posts. The name can be customized to your liking by editing a few references. For example, to change **Blog** to **Posts** update the following:

* In `_data/navigation.yml`: rename the title and URL to the following:
{% highlight yaml %}
  - title: Posts
    url: /posts/
{% endhighlight %}
* Rename `blog/index.md` to `posts/index.md` and update the YAML front matter accordingly.

### Thumbnails for OG and Twitter Cards

Site logo is used by [Open Graph](https://developers.facebook.com/docs/opengraph/) and [Twitter Cards](https://dev.twitter.com/docs/cards).

**Pro-Tip**: You need to [apply for Twitter Cards](https://dev.twitter.com/docs/cards) before they will begin showing up when links to your site are shared.
{:.notice}

### Kramdown Table of Contents

To include an auto-generated **table of contents** for posts and pages, add the following `_include` before the actual content. [Kramdown will take care of the rest](http://kramdown.rubyforge.org/converter/html.html#toc) and convert all headlines into list of links.

{% highlight html %}
{% raw %}{% include toc.html %}{% endraw %}
{% endhighlight %}

---

## Questions?

Found a bug or aren't quite sure how something works? By all means [file a GitHub Issue](https://github.com/alperenbozkurt/JBlog/issues/new). And if you make something cool with this theme feel free to let me know.

---

## License

This theme is free and open source software, distributed under the MIT License. So feel free to use this Jekyll theme on your site without linking back to me or including a disclaimer.
