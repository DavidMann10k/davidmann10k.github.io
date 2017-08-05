---
layout: post
title: Open Graph for Jekyll
header: Open Graph for Jekyll
subtitle: Make your static site a rich social graph object
category: blog

og_title: Open Graph for Jekyll
og_description: Make your favorite static site generator a rich social graph object with the Open Graph protocol.
og_image: /assets/images/cards/jekyll-opg-logo.png
og_type: article
---

This website is made with [Jekyll](https://jekyllrb.com/) and hosted on [Github Pages](https://pages.github.com/). I wanted to share one of the blog posts I'd written on Facebook, but there was a hitch. When I simply entered the url into a new Facebook post it had to guess what information to show as a preview in my feed and it guessed wrong.

To correct this the page needs a way to tell Facebook what information should be used to represent it in the preview. The [Open Graph protocol](http://ogp.me/) is the standard, made by Facebook, for communicating this information.

To implement Open Graph on your Jekyll generated site, follow these two steps:

1\. In the header, include these meta tags.

```html
{% raw %}
<meta property="og:url" content="{{ site.url }}{{ page.url }}" />
<meta property="og:title" content="{{ page.og_title }}" />
<meta property="og:description" content="{{ page.og_description }}" />
<meta property="og:image" content="{{ site.url }}{{ page.og_image }}" />
<meta property="og:type"  content="{{ page.og_type }}" />
<meta property="og:locale"  content="en_US" />
{% endraw %}
```

2\. For each page that needs Open Graph, define the Jekyll variables in the YAML front matter:

```yaml
---
  og_title: David Mann, Minneapolis Software Engineer
  og_description: Doing projects, solving problems, having fun.
  og_image: /assets/images/mann.jpg
  og_type: website
---
```

Having performed these steps for this site, here's what the rendered meta tags look like:

```html
<meta property="og:url" content="http://mann.engineer/" />
<meta property="og:title" content="David Mann, Minneapolis Software Engineer" />
<meta property="og:description" content="Doing projects, solving problems, having fun." />
<meta property="og:image" content="http://mann.engineer/assets/images/mann.jpg" />
<meta property="og:type"  content="website" />
<meta property="og:locale"  content="en_US" />
```

And here's what it looks like when shared on Facebook:

![this page shared on facebook]({{ site.url }}/assets/images/facebook-share-open-graph.PNG)

