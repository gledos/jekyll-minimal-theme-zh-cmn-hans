# What's `jekyll-minimal-theme`?

It's another minimal(istic) Jekyll static site generator theme,
that is, a ready-to-fork template pack.

See a live demo @ [`henrythemes.github.io/jekyll-minimal-theme` »](http://henrythemes.github.io/jekyll-minimal-theme)

For example:

```
├── _config.yml                               # site configuration
├── _posts                                    # sample blog posts
|   ├── 2014-05-05-sportdb-update-v192.md     #   filename format:
|   ├── 2014-10-10-new-repo-baviria-bayern.md #    => YEAR-MONTH-DAY-TITLE.MARKUP
|   ├── 2014-10-21-sql-views.md
|   ├── 2014-11-11-new-reop-maps.md
|   └── 2014-12-15-quick-starter-datafiles.md
├── _layouts                           
|   ├── default.html                   # master layout template
|   └── post.html                      # single blog post template
├── css                               
|   ├── _settings.scss                 # style settings (e.g. variables)
|   └── style.scss                     # master style page
├── feed.xml                           # web feed template (e.g. in atom format)
├── archive.html                       # archive template
└── index.html                         # index template
```

will result in (with `permalink: /:title.html`):

```
└── _site                                # output build folder; site gets generated here
    ├── css
    |   └── style.css                    # styles for pages (copied 1:1 as is)
    ├── sportdb-update-v192.html         # blog post page
    ├── new-repo-baviria-bayern.html     # another blog post page
    ├── sql-views.html                   #  ""
    ├── new-repo-maps.html               #  ""
    ├── quick-starter-datafiles.html     #  ""
    ├── feed.xml                         # web feed (e.g. in atom format)
    ├── archive.html                     # archive page
    └── index.html                       # index page
```


## Usage

To use - delete all sample posts in the `_posts` folder and
change the settings in `_config.yml` to use your own `site.title`
and `site.url`:

```
title:   'Jekyll Minimal Theme'
url:     'http://henrythemes.github.io/jekyll-minimal-theme'
author:
  name:  'Jekyll Minimal Theme Team'
```


## Color n Typography Settings (in `css/_settings.scss`)

Typography (Fonts):

~~~
$font-family:       "Helvetica Neue", Helvetica, Arial, sans-serif;

$code-font-family:  Menlo, Monaco, "Courier New", monospace;
~~~

Colors:

~~~
$masthead-color:         #505050;
$masthead-small-color:   #C0C0C0;

$post-title-color:       #303030;
$post-date-color:        #9a9a9a;


$body-color:            #515151;
$body-background-color: #fff;

$link-color:            #268bd2;

$headings-color:        #313131;    // h1,h2,h3,h4,h5,h6

$strong-color:          #303030;    // strong

$pre-background-color:  #f9f9f9;    // pre

$blockquote-color:        #7a7a7a;  // blockquote
$blockquote-border-color: #e5e5e5;

$table-border-color:         #e5e5e5;
$table-odd-background-color: #f9f9f9;
~~~

A big thanks to the Poole theme; the `jekyll-minimal-theme` started out w/
the typography and color settings from the Poole theme.


## Alternative (Minimal) Jekyll Themes

- Poole Theme by Mark Otto - [(Source)](https://github.com/poole/poole)

- Pixyll Theme by John Otander - [(Source)](https://github.com/johnotander/pixyll)

~~~
in _main.scss:
  font-family:     "Merriweather", "PT Serif", Georgia, "Times New Roman", serif;
  code-font-family: Menlo, Monaco, "Courier New", monospace;
  h1-h6|button|form|pagination|footer -font-family:
                   'Lato', 'Helvetica Neue', Helvetica, sans-serif;

in _basscss.scss:
  font-family:       'Helvetica Neue', Helvetica, sans-serif;
~~~

- Hikari Theme by Mathieu Mayer-Mazzoli - [(Source)](https://github.com/m3xm/hikari-for-Jekyll)

~~~
in components/_syntax.scss:
  code-font-family:    'Courier', monospace;
in base/_variables.scss:
  font-family:         'Open Sans', sans-serif;
  variant-font-family: 'Lora', Georgia, serif;
in base/_global.scss:
  h1-h6-font-family:  'Open Sans', sans-serif;
in base/_reset.scss:
  font-family:         sans-serif;
  code-font-family:    monospace, monospace;
~~~


### More Themes

See the [Dr. Jekyll's Themes](https://drjekyllthemes.github.io) directory.

### More Quick Starter Wizard Scripts

See the [Mr. Hyde's Scripts](https://github.com/mrhydescripts/scripts) library.


## License

![](https://publicdomainworks.github.io/buttons/zero88x31.png)
The theme and scripts are dedicated to the public domain. Use it as you please with no restrictions whatsoever.

## Questions? Comments?

Send them along to the [wwwmake forum](http://groups.google.com/group/wwwmake).
Thanks!
