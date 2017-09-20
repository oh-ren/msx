# msx.org URL 3nc0d%6Fr (URL encoder bookmarklet)

The msx.org forums have trouble parsing links sometimes.
I thought it would be fun to create a small <a href="https://en.wikipedia.org/wiki/Bookmarklet" rel="noreferrer">bookmarklet</a> that might be of aid in those cases:

<noscript><p>JavaScript is required to generate the bookmarklet links, it seems to be missing..</p></noscript>

<script>
(function() {
var bookmarklet = '(function(){var e=window,t=document,n={w:400,h:180},r="msx.org URL 3nc0d%6Fr",a=null,o=function(){var n=5,r=t.createTextNode(n);s.appendChild(r),a=e.setInterval(function(){0==n&&l.close(),n--,r.textContent=n},1e3)};e.clearInterval(a);var i;if(i=prompt(r+".\\nRemember: be happy.\\n\\nEnter problematic URL:")){console.log(i);var l=e._ren_urlEncod0r=e.open("","urlEncod0rWin","resizable,scrollbars,status,width="+n.w+",height="+n.h+",left="+(e.screenX+(e.innerWidth/2-n.w/2))+(navigator.userAgent.search("Firefox")>-1?",top="+(e.screenY+(e.innerHeight/2-n.h/2)):",top="+(e.screenY+(e.outerHeight-e.innerHeight))));l.focus();var d=l.document.body;d.innerHTML="",l.document.title=r;var c=t.createElement("input"),p=t.createElement("button"),s=t.createElement("p"),h=t.createElement("p");c.size=40,c.readOnly=!0,c.value=encodeURI(i).replace(/[!\'()*]/g,escape),p.type="button",p.textContent="copy to clipboard",p.addEventListener("click",function(){e.clearInterval(a),c.select(),l.document.execCommand("copy")&&(s.innerHTML=\'Copied to clipboard. Now paste it and <a href="javascript:window.open(\\\'https://youtu.be/4muYe8lw1hw\\\')" rel="noopener noreferrer">be happy</a>.<br>Closing in.. \'),o()}),h.textContent="Try this:",d.appendChild(h),d.appendChild(c),d.appendChild(p),d.appendChild(s),c.select();var m=t.createElement("style");m.appendChild(t.createTextNode("* { box-sizing: border-box; margin: auto; } body { font: 14px Helvetica, Arial, sans-serif; padding: 1em; } body * { margin: 0.5em 0; } input { font-size: 1em;padding: 0.5em 0.5em; line-height: 1.0; margin: auto; display: block; letter-spacing: 0.03em; }")),l.document.head.appendChild(m)}})()';

var h = '<p><a href="javascript:' + encodeURIComponent(bookmarklet) + '">msx.org URL 3nc0d%6Fr</a></p>\
    <p>Alternatively you can use the following link for e.g. mobile devices that aren\'t able, or have trouble bookmarking the link above. Click it (this will add a fragment to this page\'s URL), then bookmark this page, then edit (and rename perhaps) the bookmark, deleting everything up to and including the "#" so that the remaining URL starts with "<code>javascript:(function</code>": <a href="#javascript:' + encodeURIComponent(bookmarklet) + '">alternative link</a>.</p>';

document.write(h);
})();
</script>


## Still having issues?
If you're still having problems with the URL/link in the forums, try to use this tool only on the *part* of the URL that seems to give problems.

