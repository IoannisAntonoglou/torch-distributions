---
title: Instructions for documentation
layout: doc
---

# Documentation for torch-cephes

## How to generate the doc
Generate using [bundler](http://bundler.io/#getting-started) and [Jekyll](http://jekyllrb.com/docs/installation/):
{%highlight bash}
cd doc/src
bundle exec jekyll build --source ./ --destination ../html
{%endhighlight}

Go back to the root of the git repository.
Then merge to the gh-pages branch:
{%highlight bash}
git subtree split --prefix doc/html --branch gh-pages
{%endhighlight}

And push:
{%highlight bash}
git checkout gh-pages
git push
{%endhighlight}
