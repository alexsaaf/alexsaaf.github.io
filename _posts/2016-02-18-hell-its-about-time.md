---
layout: post
title: Hell, it's about time
---

This is the start of my personal web page, which, after laying forgotten for
about a year, will hopefully feature my projects and posts. I figured my first
post would explain how I set this page up. It's extremely simple.

## Personal site setup
This page is made using a Jekyll theme called [Lanyon](http://lanyon.getpoole.com),
and it is hosted on github pages as my personal page. Doing this requires only a
few steps.
1. Create a github repository called username.github.io (Bob would name his repository
  Bob.github.io). This will also be the URL used to access your page.
2. Now you need to get the files for the theme. The easiest way to do this is to
import the code of the Lanyon repository. You can do this by pressing "Import code"
in the quick setup page of your new repository. Then enter the URL of the Lanyon repo (https://github.com/poole/lanyon).
3. Now you may get an email from Github about a build error on your page. The cause for this
should be that the Lanyon theme has relative permalinks enabled, which is no longer
supported by Github pages. I found that this could be fixed by simply removing the line
`-relative_permalinks: true` from the `_config.yml` file. This does cause some issues with links on the page, which can be fixed by changing the links from relative to absolute. For example, in index.html, `<a href="{{ site. baseurl}}/{{ post.url }}">` should be updated to `<a href="username.github.io/{{ post.url }}">`
4. Now you have your page, and it's time to start adding your own content. The theme comes with
examples of posts and pages, so figuring out how to write your own should not be all that tricky.

### Other themes
Of course, there are other Jekyll themes to use, and you could make your own if you so desire.


[More to come, pushing as a test]
