Bevor Sie dieses Theme auf Ihrer Webseite nutzen k�nnen, m�ssen folgende URL�s angepasst werden. 

Als erstes m�ssen Sie die Datei pngHack.css im Ordner pngHack bearbeiten.
Die Ver�nderung befindet sich in Linie  2:

behavior: url('http://www.yoursite.com/modules/themes/WDC_005/pngHack/pngHack.htc');

Sie m�ssen http://www.yoursite.com gegen die URL ihrer Seite tauschen.

Als n�chstes muss die Datei pngHack.htc ge�ndert werden
Bitte �ndern Sie folgende Linie (Linie 17):

var transparentImage = "http://www.yoursite.com/themes/WDC_005/pngHack/transparent.gif";

Sie m�ssen http://www.yoursite.com gegen die URL ihrer Seite tauschen.

Nun kann der IE die .png Grafiken des Themes richtig darstellen.

Nun m�ssen Sie die Links in der theme.html �ndern, so dass sie Ihrer Webseite entsprechen.

Ein Beispiel:

<{if $xoops_cmod == "system"}>
<td width="126px" height="49px" align="left"><a href="http://www.yoursite.com/index.php" class="buttonactiv"><div style="padding-top: 14px; padding-left: 28px;">Startseite</div></a></td>
<{else}>
<td width="126px" height="49px" align="left"><a href="http://www.yoursite.com/index.php" class="button"><div style="padding-top: 14px; padding-left: 28px;">Startseite</div></a></td>
<{/if}>

<{if $xoops_cmod == "system"}> ist der Name des Modules. Dies sagt dem System, wenn eine Seite des system Modules gelandes ist, zeige as Bild des aktiven Links.

Wenn Sie nun z.B das News Modul an dieser Stelle haben wollen:

<{if $xoops_cmod == "news"}>
<td width="126px" height="49px" align="left"><a href="http://www.yoursite.com/modules/news" class="buttonactiv"><div style="padding-top: 14px; padding-left: 28px;">News</div></a></td>
<{else}>
<td width="126px" height="49px" align="left"><a href="http://www.yoursite.com/modules/news" class="button"><div style="padding-top: 14px; padding-left: 28px;">News</div></a></td>
<{/if}>

So verfahren sie mit allen 6 Links. 

Bitte den Rest nicht �ndern, denn es dient zu korekten anzeige der Links

Bei weiteren fragen bitte unter http://www.webdesigncustoms.com/modules/newbb/ fragen

Das WebdesignCustoms Team
