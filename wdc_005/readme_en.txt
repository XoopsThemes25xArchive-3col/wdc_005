Befor you can use tis the at your website, you need to change the following URL´s

First you need to change the pngHack.css inthe pngHack folder.
You change the linie  2:

behavior: url('http://www.yoursite.com/modules/themes/WDC_005/pngHack/pngHack.htc');

Replase http://www.yoursite.com with the URL of your site

The next step is to change the linie 17:

var transparentImage = "http://www.yoursite.com/themes/WDC_005/pngHack/transparent.gif";

Replase http://www.yoursite.com with the URL of your site

Now, thw IE die .png can show the .png grfiks in teh right way.

If you want to change the links in the theme.html, you need to this:

an example:

<{if $xoops_cmod == "system"}>
<td width="126px" height="49px" align="left"><a href="http://www.yoursite.com/index.php" class="buttonactiv"><div style="padding-top: 14px; padding-left: 28px;">Home</div></a></td>
<{else}>
<td width="126px" height="49px" align="left"><a href="http://www.yoursite.com/index.php" class="button"><div style="padding-top: 14px; padding-left: 28px;">Home</div></a></td>
<{/if}>

<{if $xoops_cmod == "system"}> is the name of the module. This tells the system, that it need to show the picture for the sctiv modul. This is working with every modul, witch is installed on you Xoop system.

If you want to add the News modul, you need to cahnge it in the following way

<{if $xoops_cmod == "news"}>
<td width="126px" height="49px" align="left"><a href="http://www.yoursite.com/modules/news" class="buttonactiv"><div style="padding-top: 14px; padding-left: 28px;">News</div></a></td>
<{else}>
<td width="126px" height="49px" align="left"><a href="http://www.yoursite.com/modules/news" class="button"><div style="padding-top: 14px; padding-left: 28px;">News</div></a></td>
<{/if}>

This can you do with all the 6 links.

please let the rest of the link untouched.

If you have more questions http://www.webdesigncustoms.com/modules/newbb/ 

Your WebdesignCustoms Team
