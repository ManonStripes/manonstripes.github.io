---
layout: post
title: Monit Manager Service Dark Theme
date: 2017-01-18 00:00:00
---

<div class="img_row">
    <img class="col three" src="{{ site.baseurl }}/img/cover-blog2.jpg" alt="" title="Letterpress, photo by Joshua Stocker"/><br/>
</div>
<p class="caption-blog">everything possible/Shutterstock.com</p>

<div class="blog-content">
    <h1 class="blog-title"><br/>Monit Manager Service Dark Theme</h1>
    <h2>Making Open Source More Comfortable<br/><bR/></h2>



<p class="caption-music">[&#9836; Joyful and Sweet Music playing &#9836;] </p>



<p class="post-blog">You may think that a designer and a developer can make a nice couple. An efficient team who dazzles with beautiful and working websites. Lines of code and pixel perfect designs walking down the hill hand in hand... <br/><br/>

But when you are a designer, being in couple with a developer is not always an advantage... </p>



<p class="caption-music">[&#9836; Melancholic Music &#9836;] </p>



<p class="post-blog">For instance, you could find that your TV is displaying, as an opening screen, the monitoring of your boyfriend's servers... Using a renown soft that you probably never heard of, called Monit.  </p>


<p class="caption-music">[&#9836; Musical Suspens &#9836;] </p>



<p class="post-blog">Monit is an Open Source utility for managing and monitoring servers, and if you are a sysadmin, you can only praise this project. However if you have Monit as welcome screen of a 42'' TV, it makes your eyes bleed, too much bright white. </p>

<div class="img_row">
    <img class="col three" src="{{ site.baseurl }}/img/Monit-blog1.jpg" alt="" title="Monit Screenshot"/><br/>
</div>
<p class="caption-blog">Current Monit Theme</p>

<p class="caption-music">[&#9836; Motivated Music &#9836;] </p>



<p class="post-blog">I needed to fix this quickly. So after 3 months of procrastination, I took the 3 hours required to modify Monit's CSS and create a dark theme which reduces the retinal aggression. <br/><br/>

Sharing this with the world now, as it is done and easy to upgrade. </p>



<p class="caption-music">[&#9836; Zelda Chest Opening Musique &#9836;] </p>

<div class="img_row">
    <img class="col three" src="{{ site.baseurl }}/img/Monit-blog2.jpg" alt="" title="Monit Screenshot Dark Theme"/><br/>
</div>
<p class="caption-blog">New Awesome Monit Dark Theme</p>

<h3>Features </h3>

<p class="post-blog"><b>Colors</b>: New set of colors adjusted for the efficiency of a dark theme <br/>

<b>Header</b>: Removed the large header and placed navigation in a left column</p>


<h3>Note</h3>

<p class="post-blog">As described on their website "Monit is designed as an autonomous system and does not depend on plugins nor any special libraries to run. ", I went kind of against it, as it integrates now a <a href="https://fonts.google.com/specimen/Open+Sans">Google Font</a> and <a href="http://fontawesome.io/">Font Awesome</a> icons.</p>



<h3>Files</h3>

<p class="post-blog"><a href="https://gist.github.com/ManonStripes/e6c6709e5fa4a99c330371e0fdf90277">Cervlet.c</a> - This is the file who contains all the modifications.</p>



<h3>How to install it</h3>

<p class="post-blog">Get the <a href="https://mmonit.com/monit/dist/monit-5.20.0.tar.gz">source</a> and extract it. <br/>

Replace <font class="word-hightlight">src/http/cervlet.c</font> with this <a href="https://gist.github.com/ManonStripes/e6c6709e5fa4a99c330371e0fdf90277">file</a>.<br/>
Then type the following command line</p>
{% highlight shell %}./bootstrap{% endhighlight %} 

{% highlight shell %}./configure{% endhighlight %}

{% highlight shell %}make{% endhighlight %}

{% highlight shell %}make install{% endhighlight %} 

<p class="post-blog">Tadaaa, it is running!</p>

 <p class="caption-blog">---</p>

<p class="post-blog">If you already installed it with your package manager, edit the service file and point it to the correct binary (in /usr/local/bin)<br/><br/>

<b>Note</b>: You might want to install the following packages autoconf, autogen, automake, libtool and libssl-dev.</p>
</div> 