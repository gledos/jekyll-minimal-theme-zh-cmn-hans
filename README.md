# jekyll-minimal-theme


Another minimial Jekyll theme  - [(Live Demo)](http://feedreader.github.io/jekyll-minimal-theme/)

```
├── _config.yml                               # site configuration
├── _posts                                    # blog posts
|   ├── 2014-05-05-sportdb-update-v192.md     #   filename format:
|   ├── 2014-10-10-new-repo-baviria-bayern.md #    => YEAR-MONTH-DAY-TITLE.MARKUP
|   ├── 2014-10-21-sql-views.md
|   ├── 2014-11-11-new-reop-maps.md
|   └── 2014-12-15-quick-starter-datafiles.md
├── _layouts                           
|   ├── default.html                   # master layout template
|   └── post.html                      # blog post template
├── css                               
|   └── style.css                      # styles for pages
├── feed.xml                           # web feed template (e.g. in atom format)
├── archive.html                       # archive template
└── index.html                         # index template
```

will result in (with `permalink: date`):

```
└── _site                                  # output build folder; site gets generated here
    ├── css                               
    |   └── style.css                      # styles for pages (copied 1:1 as is)
    ├── 2014
    |   ├── 05
    |   |   └── 05
    |   |       └── sportdb-update-v192.html  # blog post page
    |   ├── 10
    |   |   ├── 14
    |   |   |   └── sportdb-update-v192.html  # another blog post page
    |   |   └── 21
    |   |       └── sql-views.html
    |   ├── 11
    |   |   └── 11
    |   |       └── new-repo-maps.html
    |   └── 12
    |       └── 15
    |           └── quick-starter-datafiles.html
    ├── feed.xml                           # web feed (e.g. in atom format)
    ├── archive.html                       # archive page
    └── index.html                         # index page
```


## Usage

To use - delete all sample posts in the `_posts` folder and
change the settings in `_config.yml` to use your own `site.title`
and `site.url`:

```
title:   'Jekyll Minimal Theme'
url:     'http://feedreader.github.io/jekyll-minimal-theme'
author:
  name:  'Jekyll Minimal Theme Team'
```

