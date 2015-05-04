---
layout:     post
comments:	true
title:      "Installing Jekyll with a custom template on GitHub Pages"
subtitle:   "Get it working easily!"
date:       2015-04-17 17:34:16
author:     "Rodrigo Iglesias (Areidz)"
header-img: "img/post-bg-00.jpg"
---


<p>After almost seven years using <i><a href="https://www.wordpress.com/">Wordpress</a></i> and <i><a href="https://www.blogger.com/">Blogger</a></i> as my main blogging services, I've decided to change my mind, make a step forward and install a simple web/blog with a great frontend and without a complex database or big vulnerabilities.</p>

<p>This is why I've decided to try <i><a href="http://jekyllrb.com/">Jekyll</a></i> on <i><a href="https://pages.github.com/">GitHub Pages</a></i>. It's a simple web/blog engine written in <i><a href="https://www.ruby-lang.org">Ruby</a></i> using static pages as entries and posts.</p> 

<p>Posts are written with <i><a href="http://daringfireball.net/projects/markdown/">Markdown</a></i> files as raw-text, and are automatically converted to static pages thought a template you can edit. </p>

<h2 class="section-heading">Installing the blog</h2>

<p>I'm using Windows as my main Operative System, so even if I use <i>Arch</i> or <i>Debian</i>, I've decided to install on it the server. This isn't a trivial step, so I've followed the <a href="http://jekyll-windows.juthilo.com/">official docs</a> to do so.</p>

<p>The only problem I've faced is installing <i>wdm</i>, which isn't compiling. Even with that, everything seems to be working perfectly, so I don't really care about it.</p>

<h2 class="section-heading">Folking the template</h2>

<img src="{{ site.baseurl }}/img/included-img-00.jpg" alt="Clean Blog preview">

<p>After looking for any good template to start the blog, I found <i><a href="http://startbootstrap.com/template-overviews/clean-blog/">Clean Blog</a></i>, an amazing template by <i><a href="http://startbootstrap.com/">Start Bootstrap</a></i>.</p>

<p>I've modified it to add support for <i>Disqus</i> following <a href="https://help.disqus.com/customer/portal/articles/472138-jekyll-installation-instructions">this tutorial</a>. Thanks to this, I have comments at the bottom of every post.</p>

<p>Also, I've added share buttons following <a href="http://codingtips.kanishkkunal.in/share-buttons-jekyll/">this guide</a>. I've had to adapt it to my custom template by creating some new css and html files, loading the css file in <i>head.html</i> and the html one to the post template. Maybe you find it interesting.</p>

<h2 class="section-heading">Useful links</h2>

<p>To finish the post, I want to share some useful links:</p>

<ul>
	<li><b><a href="https://github.com/jekyll/jekyll/wiki/Sites">Examples</a></b>: Some examples of websites using <i>Jekyll</i>.</li>
	<li><b><a href="http://jekyllrb.com/">Jekyll</a></b>: Main <i>Jekyll</i> website with install guides and configuration tutorials.</li>
	<li><b><a href="http://jekyll-windows.juthilo.com/">Jekyll for Windows</a></b>: A website explaining how to install <i>Jekyll</i> on <i>Windows</i>.</li>
	<li><b><a href="https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet">Markdown Cheatsheet</a></b>: Useful cheatsheet to write posts.</li>
</ul>