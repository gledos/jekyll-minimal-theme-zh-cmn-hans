注意，还没有完成中文简体化

[原项目地址](https://github.com/henrythemes/jekyll-minimal-theme/)

以下是原 README.md 的内容

# 什么是 `jekyll-极简主题`?

这是又一个极简(风格)的Jekyll静态站点生成器主题，
也就是说，一个现成的主题模板包。

查看在线演示 @ [`henrythemes.github.io/jekyll-minimal-theme` »](http://henrythemes.github.io/jekyll-minimal-theme "中文简体化正在进行")

---

举例:

```
├── _config.yml                # 网站配置
├── _posts                        # 暂时储存着一些博客文章模板用作演示
|   ├── 2014-05-05-sportdb-update-v192.md
|   ├── 2014-10-10-new-repo-ba-bay.md          # 文件名格式:
|   ├── 2014-10-21-sql-views.md             # => 年-月-日-标题.格式
|   ├── 2014-11-11-new-reop-maps.md
|   └── 2014-12-15-quick-starter-datafiles.md
├── _layouts
|   ├── default.html         # 主布局模板
|   └── post.html              # 单一博客模板
├── css
|   ├── _settings.scss        # 风格设置(例如变量)
|   └── style.scss              # 主风格页面
├── feed.xml                    # web订阅源模板(如atom格式)
├── archive.html              # 归档文章
└── index.html                 # 主页模板
```

将会生成出

```
└── _site                                 # 输出生成文件夹; 网站在此生成
    ├── css
    |   └── style.css                   # 页面样式（按原样复制1：1）
    ├── sportdb-update-v192.html           # 博客文章页面
    ├── new-repo-ba-bay.md.html     # 另一个博客网站页面
    ├── sql-views.html               #  ""
    ├── new-repo-maps.html      #  ""
    ├── quick-starter-datafiles.html        #  ""
    ├── feed.xml                        # web订阅源（如atom格式）
    ├── archive.html                  # 归档文章
    └── index.html                     # 主页
```

## 使用方法

首先删除`_posts`文件夹中的所有示例文章
然后更改`_config.yml`中的设置以使用您自己的`site.title`和`site.url`：

```
title:   'Jekyll Minimal Theme'
url:     'http://henrythemes.github.io/jekyll-minimal-theme'
author:
  name:  'Jekyll Minimal Theme Team'
```


## Color n Typography Settings (in `css/_settings.scss`)

## 颜色无印刷术设置（在 `css/_settings.scss`）

排版（字体）：

~~~
$font-family:       "Helvetica Neue", Helvetica, Arial, sans-serif;

$code-font-family:  Menlo, Monaco, "Courier New", monospace;
~~~

颜色：

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

非常感谢Poole主题 (Poole theme); `jekyll-minimal-theme` 开始于Poole主题的排版和颜色设置。

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
