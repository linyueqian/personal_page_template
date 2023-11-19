# The Minimal Light Theme modified by Yueqian Lin

<br>
*Feel free to use and share the source code anywhere you like.*

<br>
This template is momdified from [Minimal Light](https://github.com/yaoyao-liu/minimal-light/).
<br>

## Features

- Simple and elegant personal homepage theme
- Jekyll theme, automatically deployed by GitHub Pages
- Basic search engine optimization
- Mobile friendly
- Supporting Markdown 
- Supporting dark mode

## Project Architecture

```
.
├── _includes                    # the Markdown files for publications and services  
├── _layouts                  
|   └── homepage.html            #  the html template for the homepage 
├── _sass                     
|   └── minimal-light.scss       #  this file will be compiled into a CSS file to control the style of the page
├── assets                       #  some files
├── .gitignore                   #  this file specifies intentionally untracked files that Git should ignore
├── CNAME                        #  the custom domain, will be used by GitHub page sevice
├── Gemfile                      #  a RubyGems related file
├── LICENSE                      #  the license file
├── README.md                    #  the readme file (English)
├── _config.yml                  #  the Jekyll configuration file, including some options of the page  
└── index.md                     #  the content of the index page, using Markdown
```

## Usage

### Using Locally with Jekyll

*You need to install [Ruby](https://www.ruby-lang.org/en/) and [Jekyll](https://jekyllrb.com/) fisrt.*

Clone this repository:

```bash
git clone https://github.com/linyueqian/personal_page_template.git
cd personal_page_template
```

Install and run:

```bash
bundle install
bundle exec jekyll server
```

View the live page using `localhost`:
<http://localhost:4000>. You can get the html files in `_site` folder.

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
description: The Minimal Light is a simple and elegant jekyll theme for academic personal homepage.
canonical: https://minimal-light-theme.yliu.me/

# Links 
# If you don't need one of them, you may delete the corresponding line.
google_scholar: https://scholar.google.com/
cv_link: files/Curriculum_Vitae.pdf
github_link: https://github.com/
linkedin: https://www.linkedin.com/
twitter: https://twitter.com/

# Images (e.g., your profile picture and your website's favicon) 
# "favicon" and "favicon_dark" are used for the light and dark modes, respectively. 
avatar: ./assets/img/avatar.png
favicon: ./assets/img/favicon.png
favicon_dark: ./assets/img/favicon-dark.png

# Google Analytics ID
# Please remove this if you don't use Google Analytics
google_analytics: UA-111540567-4
```

### Editing `index.md`

Create `index.md` and add your personal information (e.g., publications, research).

### Stylesheet

If you'd like to add your own custom styles:

1. Create a file called `/assets/css/style.scss` in your site

2. Add the following content to the top of the file, exactly as shown:
   
   ```scss
   ---
   ---
   
   @import "{{ site.theme }}";
   ```

3. Add any custom CSS (or Sass, including imports) you'd like immediately after the `@import` line

### Layouts

If you'd like to change the theme's HTML layout:

1. [Copy the original template](https://github.com/yaoyao-liu/minimal-light/blob/master/_layouts/homepage.html) from the theme's repository<br />(*Pro-tip: click "raw" to make copying easier*)
2. Create a file called `/_layouts/homepage.html` in your site
3. Paste the default layout content copied in the first step
4. Customize the layout as you'd like

## License

This work is licensed under a [Creative Commons Zero v1.0 Universal](https://github.com/yaoyao-liu/minimal-light/blob/master/LICENSE) License.

## Acknowledgements

Our project uses the source code from the following repositories:

* [yaoyao-liu/minimal-light](https://github.com/yaoyao-liu/minimal-light/)

* [pages-themes/minimal](https://github.com/pages-themes/minimal)

* [orderedlist/minimal](https://github.com/orderedlist/minimal)

* [al-folio](https://github.com/alshedivat/al-folio)
