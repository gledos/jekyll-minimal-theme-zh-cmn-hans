- [源项目](https://github.com/henrythemes/jekyll-minimal-theme)
- [汉化内容](#汉化内容)

<details>
<summary>点击展开原 README 汉化后的内容</summary>

# 什么是 `jekyll-极简主题`?

这是又一个极简(风格)的Jekyll静态站点生成器主题，
也就是说，一个现成的主题模板包。

查看在线演示 @ [`gledos.science/jekyll-minimal-theme-zh-cmn-hans` »](http://gledos.science/jekyll-minimal-theme-zh-cmn-hans/)

---

举例:

```
├── _config.yml                # 网站配置
├── _posts                     # 暂时储存着一些博客文章模板用作演示
|   ├── 2014-05-05-sportdb-update-v192.md
|   ├── 2014-10-10-new-repo-ba-bay.md     # 文件名格式:
|   ├── 2014-10-21-sql-views.md           # => 年-月-日-标题.格式
|   ├── 2014-11-11-new-reop-maps.md
|   └── 2014-12-15-quick-starter-datafiles.md
├── _layouts
|   ├── default.html           # 主布局模板
|   └── post.html              # 单一博客模板
├── css
|   ├── _settings.scss         # 风格设置(例如变量)
|   └── style.scss             # 主风格页面
├── feed.xml                   # web订阅源模板(如atom格式)
├── archive.html               # 归档文章
└── index.html                 # 主页模板
```

将会生成出

```
└── _site                           # 输出生成文件夹; 网站在此生成
    ├── css
    |   └── style.css               # 页面样式（按原样复制1：1）
    ├── sportdb-update-v192.html    # 博客文章页面
    ├── new-repo-ba-bay.md.html     # 另一个博客网站页面
    ├── sql-views.html              
    ├── new-repo-maps.html          
    ├── quick-starter-datafiles.html    
    ├── feed.xml                    # web订阅源（如atom格式）
    ├── archive.html                # 归档文章
    └── index.html                  # 主页
```

## 使用方法

首先删除`_posts`文件夹中的所有示例文章，然后更改`_config.yml`中的设置以使用您自己的`site.title`和`site.url`：

```
title:   'Jekyll Minimal Theme 中文简体版'
url:     'http://henrythemes.github.io/jekyll-minimal-theme'
author:
  name:  'Jekyll Minimal Theme Team'
```


## Color n Typography Settings (in `css/_settings.scss`)

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

非常感谢Poole主题 (Poole theme); `jekyll-minimal-theme` 始于Poole主题的排版和颜色设置。

## 其他的 (极简) Jekyll主题

- Poole Theme by Mark Otto - [(源代码)](https://github.com/poole/poole)

- Pixyll Theme by John Otander - [(源代码)](https://github.com/johnotander/pixyll)

~~~
in _main.scss:
  font-family:     "Merriweather", "PT Serif", Georgia, "Times New Roman", serif;
  code-font-family: Menlo, Monaco, "Courier New", monospace;
  h1-h6|button|form|pagination|footer -font-family:
                   'Lato', 'Helvetica Neue', Helvetica, sans-serif;

in _basscss.scss:
  font-family:       'Helvetica Neue', Helvetica, sans-serif;
~~~

- Hikari Theme by Mathieu Mayer-Mazzoli - [(源代码)](https://github.com/m3xm/hikari-for-Jekyll)

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


### 更多主题

查看 [Dr. Jekyll's Themes](https://drjekyllthemes.github.io) 的目录。

### 更多的快速入门向导脚本

查看 [Mr. Hyde's Scripts](https://github.com/mrhydescripts/scripts) 的库。


## License / 许可证

![CC0协议](https://publicdomainworks.github.io/buttons/zero88x31.png)
主题和脚本专用于公共领域。 尽可能地使用它，不受任何限制。

## ~~有问题和意见？~~

~~发送他们到 [wwwmake forum](http://groups.google.com/group/wwwmake).
谢谢！~~

建议发给我(gledos)，但是我不一定有能力解决，就算能解决也会花上很多时间......

</details>

# 汉化内容

- 日期中国习惯化
- 字体加入各种设备适合的中文字体(包括 Chrome OS)
- 对字体大小和边距有所调整，更佳适合中文(但也许也不是最合适的)
- 对README 和网站上首页的第一篇文章进行了汉化

## 一些提示

这个主题不需要在文章的 mayl 头文件中写入 `date` 这一项多余的东西，本主题在经过我的修改(最大限度保留原设定)选择 `post` 模板时会直接寻找在 `_post/` 里面的文章中的 `YYYY-MM-DD` 格式的时间，所以就不需要出现两份时间了。

- [liquid 模板语言中文文档](https://liquid.bootcss.com)
- [jekyll 中新增的 liquid 过滤器(英文)](https://jekyllrb.com/docs/templates/)
- [Shellphon 写的 liquid 用法笔记](http://blog.csdn.net/dont27/article/details/38097581)

## 推荐修改

- 使用 liquid 进行生成 sitemap.xml [比如](https://github.com/jekyll/jekyll/blob/master/test/source/sitemap.xml)
- 写长文要使用摘要 [Post excerpts - jekyll docs(英文)](https://jekyllrb.com/docs/posts/#post-excerpts)、[中文](http://www.cnblogs.com/coderzh/p/jekyll-readmore.html)
- 限制主页显示文章的数量，还可以加上分页。(但是 5 篇文章就一页简直浪费人生，建议 8 篇以上，因为观看者不去归档看标题，就是为了看主页中的摘要内容啊) [](https://jekyllrb.com/docs/pagination/)
