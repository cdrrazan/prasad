---
layout: page
title: Ultimate Guide to setup Prasad Jekyll theme
comments: true
---

Prasad is the modified form of Affiliates Jekyll Theme.

- **Demo:** https://prasad.cdrrazan.com

>You can view the full live site using this theme <a href="https://cdrrazan.com" target="_blank">
>HERE.</a> <br>

>If you need any help open the issue in <a href="https://github.com/cdrrazan/prasad/issues/new"
>target="_blank"> here.</a>


<h3> Features </h3>

- Built for Jekyll
> Built in version 3.8.5
- Compatible with Github, Gitlab and Netlify Pages
- Featured Posts
- Index Pagination
- Post Categories
> categories/name
- Prev/Next Link
- Category Archives (this is not yet compatible with github pages though)
> compatible with netlify and gitlab pages
- Integrations:
    - Disqus Comments
    - Google Analaytics
    - Sharethis Integration
    - Formspree.io Contact
- Design Features:
    - Bootstrap v4.0.0-alpha.6
    - Font Awesome
    - Masonry
- Layouts:
    - Default
    - Sticky Sidebar
    - Page
    - Archive

#### How to Use

Let's move on to using Prasad template in Jekyll:

[Download](https://github.com/cdrrazan/prasad/archive/master.zip) or Fork *cdrrazan/prasad*.
- In your local project, open <code>_config.yml</code>. If your site is in root, for <code>baseurl</code>, make sure this is set to <code>baseurl: /</code>. Also, change your Google Analytics code, Disqus username, Authors, ShareThis code (https://www.sharethis.com/) etc.

- Prasad requires 3 plugins:
    - <code>$ gem install jekyll-paginate</code>
    - <code>$ gem install jekyll-archives</code>
    - <code>$ gem install jekyll-seo-tag</code>

- Locate the files and customize:
    - header & footer in <code>default.html</code>.
    - homepage in <code>index.html</code>
    - contact form in <code>contact.html</code> (https://formspree.io/)
     > Suitable for any third party Contact form service provider.
    - post sidebar in <code>includes/sidebar.html</code>
     > Suitable for Referral or Ads Code. You can make sidebar unsticky as well.
    - sign up form in <code>includes/newsletter.html</code>
    > Suitable for newsletter service. You can directly use the REVUE newsletter service from here.
    - search blog in <code> Search/index.html </code>
    > Theme uses Lunr.js for searching the blog.

- Start blogging by adding your .md files in <code>_posts</code>. You will see in examples in the download.
- YAML front matter
    - post featured - <code>featured:true</code>
    - post featured image - <code>image: assets/images/mypic.jpg</code>
    - page comments - <code>comments:true</code>
    > Can setup multiple commenting system as well.
    - meta description (optional) - <code>description: "this is my meta description"</code>
    - permalinks (optional) - <code>permalink: /blog/this-is-link/</code>
    > Setting up custom permalink in the post section will override permalink config from _config.yml

YAML Post Example:
<pre class="highlight">
---
layout: post
title:  "We all wait for summer"
author: john
categories: [ Jekyll, tutorial ]
image: assets/images/1.jpg
featured: true
permalink: /blog/permalinks-setup/
---
</pre>


YAML Page Example
<pre class="highlight">
---
layout: page
title: Prasad Template for Jekyll
comments: true
---
</pre>

- SEO
  - This theme uses jekyll-seo-tag plugins for SEO. Please refer to the [documentation of the plugins](https://github.com/jekyll/jekyll-seo-tag/blob/master/docs/usage.md) for additional theme uses and modification.

 - Instruction on deploying in Gitlab and Netlify
    - Gitlab: Add .gitlab-ci.yml for building Jekyll in Gitlab Pages
    - Netlify: Visit [this netlify docs](https://www.netlify.com/blog/2015/10/28/a-step-by-step-guide-jekyll-3.0-on-netlify/)

<h5> All the images posted here are for blog demo purpose only. </h5>
