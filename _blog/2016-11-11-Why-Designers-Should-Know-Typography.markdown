---
layout: post
title: Why Designers Should Know Typography
date: 2016-11-11 - 00:00
---

<div class="img_row">
    <img class="col three" src="{{ site.baseurl }}/img/cover-blog1.jpg" alt="" title="Letterpress, photo by Joshua Stocker"/><br/>
</div>
<p class="caption-blog">
Letterpress, photo by Joshua Stocker</p>

<div class="blog-content">
<h1 class="blog-title">Why Designers Should Know Typography</h1>

<h2>A Story About Webfonts And Forgotten Craft</h2>
<br/>
<p class="post-blog">When everything was printed, typography was a big deal. You even had people specialized in this.<br/><br/>

Transitioning to the web, this art form was on the edge to be lost: we thought that it wasn’t that important. Now that we have fancy websites with fancy fonts, it’s making a comeback. Problem: everyone forgot how to do it right! Let me illustrate.<br/><br/>

Last year, as the lead designer of a small R&D Team at Natexo Group, I accidentally heard an argument between one of my designer, a front end dev and our project manager.</p>

<h3>The story</h3>

<p class="post-blog">There was a typo on one of our client’s website. The word ‘profit’ appeared as ‘proit’.</p>
<div class="img_row">
    <img class="col three" src="{{ site.baseurl }}/img/typography-blog1.jpg" alt="" title="Ligatures"/><br/>
</div>

<p class="post-blog"><br/>Our unfortunate front end dev, who is at the bottom of the command chain, received all the blames. But he vigorously argued for his innocence :<br/>
<i>«The error is not in my code!».</i><br/><br/>

Overhearing the situation, and maybe excited by the strange bug, I took part in the discussion. After a while inspecting the code in my browser, I found out that the issue was with the Google Font used. Maybe I spoke too fast at that moment, because my designer hurried to find another font and replaced it in her design.<br/><br/>

But it felt wrong. A buggy Google Font? Really? Where are we heading if we can’t rely on Google anymore?<br/>
I stayed longer facing my screen, trying to understand what we missed and then… Finally… I understood. The ligatures.</p>

<h3>Ligatures? What’s That?</h3>

<p class="post-blog">Yes, that’s the reaction my team had when I said the word. A term they didn’t hear in their whole life. And probably won’t remember the next morning.<br/>
When two or more letters are combined in one character, you have a ligature.</p>
<div class="img_row">
    <img class="col three" src="{{ site.baseurl }}/img/typography-blog2.jpg" alt="" title="Ligatures"/><br/>
</div>
<p class="caption-blog">Examples: « œ » in french, « ß » in german and the whole world with « & », yes! You didn’t know that the ampersand character is e and t combined, because « et » in latin means “and”</p>

<p class="post-blog">There are two type of ligatures :<br/></p>

    <ul><li><p class="post-blog"><b>Aesthetic ligatures:</b> Because secluded monks were too lazy to lift their pen, they connected letters. We don’t use them much, optional stuff.</p></li>
    <li><p class="post-blog"><b>Technical ligatures:</b> Legacy of the printing rules about readability, ligatures prevent two letters to collide on the paper. Especially with f.</p></li>
</ul>
<div class="img_row">
    <img class="col three" src="{{ site.baseurl }}/img/typography-blog3.jpg" alt="" title="Ligatures"/><br/>
</div>
<p class="caption-blog">Especially with f</p>

<h3>Lost in Googlisation</h3>

<p class="post-blog">So we ended up with a Google Font, lacking some ligatures. At this time, this issue wasn’t in the top ranking Google results, a longer exploration of the deep and dark dev blogs was requested.<br/><br/>

I then discovered css attributes about ligatures. What a wonderful world we are living in.</p>

{% highlight css %}
-webkit-font-feature-settings: 'liga' 0, 'onum' 1, 'kern' 1;
-moz-font-feature-settings: 'liga' 0, 'onum' 1, 'kern' 1;
-o-font-feature-settings: 'liga' 0, 'onum' 1, 'kern' 1;
font-feature-settings: 'liga' 0, 'onum' 1, 'kern' 1;
{% endhighlight %}

<p class="post-blog"><font class="word-hightlight">font-feature-settings</font> gives you access to a bunch of advanced typographic settings, among them: ligature!<br/>
With <font class="word-hightlight">0</font> , we chose to disable the automatic use of ligatures, which made the letter ‘f’ appear again. Victory is mine!</p>

<h3>Conclusion</h3>

<p class="post-blog">If you take a look at History of Web Typography, you can only notice improvement. Since Google launching his own font library in 2010, to this <font class="word-hightlight">font-feature-settings</font> attribute, that allows all typography fanatics to greatly improve the readability of their web texts. Ligatures, swashes, fractions, kerning, etc. All these and more are in your power, at the tip of your fingers. Implying you have the right typeface to play with and that you master typography. And that’s the real issue.<br/><br/>

The delicate and sensible art of typography is not teached to designers anymore (or not well), lots of them don’t even know how to play with the Opentype features in Photoshop.
And don’t expect front dev to save the situation by knowing an obscure css attribute.
Certainly, you end up with a bunch of employees ready to start again from scratch just because they didn’t understand an issue.<br/><br/>

So did we lose a generation of designers to the typography cause?</p>

<p class="caption-blog">---</p>

<p class="post-blog">Want to learn more about <font class="word-hightlight">font-feature-settings</font> value? <a href="https://css-tricks.com/almanac/properties/f/font-feature-settings/">Try here</a>.</p>
</div>