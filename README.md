# The Minimal Light Theme

[![LICENSE](https://img.shields.io/github/license/yaoyao-liu/minimal-light?style=flat-square&logo=creative-commons&color=EF9421)](https://github.com/yaoyao-liu/minimal-light/blob/main/LICENSE)

\[[Demo the theme](https://minimal-light-theme.yliu.me/)\]  \[[简体中文](https://github.com/yaoyao-liu/minimal-light/blob/master/README_zh_Hans.md) | [繁體中文](https://github.com/yaoyao-liu/minimal-light/blob/master/README_zh_Hant.md) | [Deutsch](https://github.com/yaoyao-liu/minimal-light/blob/master/README_de.md)\]
 
*This repository contains the source code for my homepage. The website is based on [minimal](https://github.com/orderedlist/minimal).*
<br>
*Feel free to use and share the source code anywhere you like.*

An improved version from [@Xiao-Chenguang](https://github.com/Xiao-Chenguang): [[link](https://github.com/Xiao-Chenguang/minimal-light)]

**The latest version of my homepage is available here: <br><https://github.com/yaoyao-liu/homepage>**

## Features

- A simple and elegant personal homepage theme
- A Jekyll theme that can be automatically deployed with GitHub Pages
- Basic search engine optimization
- Mobile-friendly layout
- Markdown support
- Dark mode support

## Project Architecture

```
.
├── _data                    
|   └── publications.yml                      # the YAML file for publications
├── _includes                    
|   ├── publications.md                       # the Markdown file for publications
|   └── services.md                           # the Markdown file for services
├── _layouts                  
|   └── homepage.html                         #  the HTML template for the homepage
├── _sass
|   ├── minimal-light.scss                    #  compiled into a CSS file to control the page style
|   └── minimal-light-no-dark-mode.scss       #  this file is similar to minimal-light.scss with the dark mode disabled
├── assets                                    #  static assets
├── html_source_file                          #  compiled HTML files
├── .gitignore                                #  this file specifies intentionally untracked files that Git should ignore
├── CNAME                                     #  the custom domain used by GitHub Pages
├── Gemfile                                   #  a RubyGems-related file
├── LICENSE                                   #  the license file
├── README.md                                 #  the readme file (English)
├── README_de.md                              #  the readme file (German)
├── README_zh_Hans.md                         #  the readme file (Simplified Chinese)
├── README_zh_Hant.md                         #  the readme file (Traditional Chinese)
├── _config.yml                               #  the Jekyll configuration file, including page options
└── index.md                                  #  the content of the index page, using Markdown
```

## Getting Started

This template can be used in two ways:
- **Using GitHub Pages.** GitHub provides a server to generate and host web pages.
- **Using Jekyll locally.** You can install Jekyll on your own computer and generate static web pages (i.e., HTML files) with this template. After that, you can upload the HTML files to your own server.

The detailed instructions are available below.


### Using GitHub Pages

There are two ways to use this template on GitHub:

#### Fork this repository
- Fork this repository (or [use this repository as a template](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-from-a-template)) and change the name to `your-username.github.io`.

- Enable GitHub Pages for that repository by following the steps [here](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site#creating-your-site).

#### Using this repository as a remote theme
To use this theme, add the following to your repository's `_config.yml`:

```yaml
remote_theme: yaoyao-liu/minimal-light
```

Please note that adding the line above will apply all default settings from this repository to yours.

If you want to edit any files (e.g., `index.md`), you still need to copy them to your repository.

### Using Locally with Jekyll

First, install [Ruby](https://www.ruby-lang.org/en/) and [Jekyll](https://jekyllrb.com/). The installation instructions are available here: <https://jekyllrb.com/docs/installation/#guides>

Then, clone this repository:

```bash
git clone https://github.com/yaoyao-liu/minimal-light.git
cd minimal-light
```
Install and run:

```bash
bundle install
bundle add webrick
bundle exec jekyll serve
```
View the live page locally at:
<http://localhost:4000>. The generated HTML files are available in the `_site` folder.

### Using the HTML version

The compiled HTML files are available in the `html_source_file` folder. If you prefer not to use Jekyll, you can edit and use the HTML version directly.

## Customizing

### Configuration variables

The Minimal Light theme will respect the following variables, if set in your site's `_config.yml`:

  ```yaml
# Basic Information 
title: Your Name
position: Ph.D. Student
affiliation: Your Affiliation
email: yourname (at) example.edu

# Search Engine Optimization (SEO)
# The following information is used to improve the website traffic from search engines, e.g., Google.
keywords: minimal light
description: Minimal Light is a simple and elegant Jekyll theme for academic personal homepages.
canonical: https://minimal-light-theme.yliu.me/

# Links 
# If you don't need one of them, you may delete the corresponding line.
google_scholar: https://scholar.google.com/
cv_link: assets/files/curriculum_vitae.pdf
github_link: https://github.com/
linkedin: https://www.linkedin.com/
twitter: https://twitter.com/

# Images (e.g., your profile picture and your website's favicon) 
# "favicon" and "favicon_dark" are used for the light and dark modes, respectively. 
avatar: ./assets/img/avatar.png
favicon: ./assets/img/favicon.png
favicon_dark: ./assets/img/favicon-dark.png

# Footnote
# You may use the option to disable the footnote, "Powered by Jekyll and Minimal Light theme."
enable_footnote: true

# Auto Dark Mode
# You may use the option to disable the automatic dark theme
auto_dark_mode: true

# Font
# You can use this option to choose between Serif or Sans Serif fonts.
font: "Serif" # or "Sans Serif"

# Google Analytics ID
# Please remove this if you don't use Google Analytics
google_analytics: UA-111540567-4
  ```
### Edit `index.md`

Create `index.md` and add your personal information. It supports **Markdown** and **HTML** syntax.

### Edit included files

There are two Markdown files included in `index.md`: `_includes/publications.md` and `_includes/services.md`. These two files also support **Markdown** and **HTML** syntax. If you do not want to include these files, you can remove the following lines in `index.md`:
https://github.com/yaoyao-liu/minimal-light/blob/b38070cd0b6bce45d8a885f3828549af8f82b7cb/index.md?plain=1#L21-L23

If you want to edit the publication list without changing the format, you can edit `_data/publications.yml`:
https://github.com/yaoyao-liu/minimal-light/blob/77b1b3b31d4561091bcd739f37a2e1880e8b5ca5/_data/publications.yml#L3-L11


### Stylesheet

If you'd like to add your own custom styles, you may edit `_sass/minimal-light.scss`.

### Layouts

If you'd like to change the theme's HTML layout, you can edit `_layouts/homepage.html`.

## License

This work is licensed under a [Creative Commons Zero v1.0 Universal](https://github.com/yaoyao-liu/minimal-light/blob/master/LICENSE) License.

## Acknowledgements

This project uses source code from the following repositories:

* [pages-themes/minimal](https://github.com/pages-themes/minimal)

* [orderedlist/minimal](https://github.com/orderedlist/minimal)

* [al-folio](https://github.com/alshedivat/al-folio)
