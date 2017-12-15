# ZIXIA DE BLOG

Here's blog from huan.

# TUTORIAL

* [Building a static website with Jekyll and GitHub Pages](https://programminghistorian.org/lessons/building-static-sites-with-jekyll-github-pages#setting-up-jekyll-)
* [To import your posts from your Blogger](http://import.jekyllrb.com/docs/blogger/)

## Setup

```shell

jekyll new JekyllDemo

ruby -rubygems -e 'require "jekyll-import";
    JekyllImport::Importers::Blogger.run({
      "source"                => "/home/zixia/Downloads/blog-12-08-2017.xml",
      "no-blogger-info"       => false, # not to leave blogger-URL info (id and old URL) in the front matter
      "replace-internal-link" => false, # replace internal links using the post_url liquid tag.
    })'

bundle exec jekyll serve --watch
```

## Local View

```shell
gem install bundler
```