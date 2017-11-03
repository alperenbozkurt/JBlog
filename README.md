# JBlog Jekyll Theme

**[JBlog](http://alperenbozkurt.net/JBlog)** is a simple jekyll theme.

I have used this theme in my own php and ruby blogs. And there are some shortcomings. If something looks extremely ugly and you can't resist to fix it, just send me a PR. I will be grateful.

If you like this theme or using it, please give a **star** for motivation.

## Preview

![Home Page](/assets/img/screenshot-home.png)    
![Post Page](/assets/img/screenshot-post.png)

See a [live version of JBlog](http://alperenbozkurt.net/JBlog) hosted on GitHub.

## Getting Started

To learn how to install and use this theme check out the [Setup Guide](http://alperenbozkurt.net/JBlog/JBlog-theme/) for more information or apply the following instructions.

## Installation

- Fork the Repo
- Edit _config.yml file.
	- Edit url as **https**://yourusername.github.io
	- and others
- Remove sample posts from _posts folder and add yours.
- Edit index.md file in about folder.
- Change repo name to YourUserName.github.io
- Open "Github Pages" from settings page
- Click the star icon at the top of this page ;)


## How to customization

- You can change title, description, profile image and social network icons in _config.yml file.
- If you are not like this colors or fonts, you can change its in _sass/variables.scss file.
```scss
$title-font   : Lobster, cursive;
$menu-font    : Alegreya Sans SC, sans-serif;
$main-font    : Roboto Slab, serif;
```
You can add your fonts this area.
```scss
// Colors
$blue: #3498db;
$orange: #e67e22;
$red: #e74c3c;
$white: #ecf0f1;
$green: #2ecc71;
$turko: #1abc9c;
$purple: #9b59b6;
$dark-blue: #34495e;

$main-color: $white;
$background-color: $blue;
$thrid-color: rgba(52, 152, 219, 0.8);
```

$main-color is panels background color.
$background-color is background, buttons, links color.
$thrid-color is opacity version of background color.
