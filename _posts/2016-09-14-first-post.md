---
layout: post
title: "September 14, 2016"
---
What's `jekyll-minimal-theme`?

It's another minimal(istic) Jekyll static site generator theme,
that is, a ready-to-fork template pack. For example:

~~~
├── _config.yml                               # site configuration
├── _posts                                    # sample blog posts
|   ├── 2014-04-test-styles.md     #   filename format:
|   ├── 2015-01-31-welcome.md
├── _layouts                           
|   ├── default.html                   # master layout template
|   └── post.html                      # single blog post template
├── css                               
|   ├── _settings.scss                 # style settings (e.g. variables)
|   └── style.scss                     # master style page
├── feed.xml                           # web feed template (e.g. in atom format)
├── archive.html                       # archive template
└── index.html                         # index template
~~~

will result in (with `permalink: /:title.html`):

~~~
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
~~~

To use - delete all sample posts in the `_posts` folder and
change the settings in `_config.yml` to use your own `site.title`
and `site.url`: