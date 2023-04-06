---
layout: post
title:  "Jekyll notes"
date:   2020-05-24 19:48:56 +0530
categories: jekyll installation
---

Installing Ruby:
{% highlight bash %}
brew install rbenv ruby-install
rbenv install -l # show all versions
ruby-install 2.7.1
rbenv local 2.7.1
{% endhighlight %}

Jekyll:
{% highlight bash %}
mkdir my-jekyll-website
cd my-jekyll-website
bundle init
bundle add jekyll
bundle exec jekyll new --force --skip-bundle .
bundle install
bundle exec jekyll serve
{% endhighlight %}

