TL;DR me and some friends (but mostly me) thought it would be funny to whip up the most abhorrent website we could think of. It's not that abhorrent and not that funny.

---

```
anatol: guys look at this:
```

```bash
whois why69.com

Whois Server Version 2.0

Domain names in the .com and .net domains can now be registered
with many different competing registrars. Go to http://www.internic.net
for detailed information.

No match for "WHY69.COM".
>>> Last update of whois database: Fri, 29 Jan 2016 21:45:35 GMT <<<
```

```
anatol: there you go
anatol: 5char domain
anatol: ideal for porn
marius: :))
tvararu: or dating advice
tvararu: relationship, rather
anatol: it should just have a big h1 tag
anatol: dead centre
anatol: font 48 or bigger
anatol: <h1>WHY NOT?</h1>
tvararu: <H1>
marius: and the stylesheet:
```

```css
body {
  background-color: black;
}

h1 {
  font-size: 48;
  color: red;
}
```

```
anatol: font-size: 69
marius: yeah
anatol: color: pink
marius: no dude, color: red-light-district;
anatol: @tvararu yeah, <H1> for consistency
```

```bash
cd github
mkdir why69
cd why69
cat > index.html
<!DOCTYPE HTML>
<STYLE>/* etc */</STYLE>
<H1>WHY NOT?</H1>^D
surge . -d why69.surge.sh
```

```
tvararu: http://why69.surge.sh/
tvararu: done, deployed
anatol: color: hotpink
anatol: and centre the thing, dude
marius: yeah dude you suck
tvararu: @marius garbage in garbage out
```

```diff
+ text-align: center;
```

```
tvararu: done
anatol: vertically as well dude omg
tvararu: GOD DUDE IS THERE ANYTHING ELSE YOU WANT FFS
anatol: centre it vertically.
```

```diff
h1 {
- text-align: center;
}
+ html, body {
+   width: 100%;
+   height: 100%;
+ }
+ body {
+   display: flex;
+   align-items: center;
+   justify-content: center;
+ }
```

```
tvararu: done
anatol: did you test it on ie6?
tvararu: works great on all supported IEs
tvararu: actually who am I kidding, works *great* on every browser!
tvararu: just that some of them get loser centering
anatol: wtf are these margins and scrollbars
```

```diff
html, body {
+  margin: 0;
}
```

```
tvararu: which margins fam
anatol: wait
anatol: <screenshot of booting up windows xp>
anatol: just wait...
tvararu: LOL
marius: LOL I nearly cohked on this potato
tvararu: developing this website is a pretty practical example of how product development works
tvararu: "ah, it'll be 8 lines of code total"
tvararu: ends up being 19, a 2x increase
tvararu: because of constantly shifting requirements
tvararu: oh I know, we should do fancy wordart animated text
marius: <marquee>
tvararu: no not marquee
tvararu: I mean like one of those that defines a sine wave
marius: I think you can do it in css
tvararu: yeah if you break every letter into spans and animate them individually
marius: no
tvararu: I don't think you can use transform: skew
marius: you can tesselate your image with a filter
tvararu: yeah but that's basically not even html anymore, that's just webgl
anatol: I have bad news
marius: it does involve vertex shaders, indeed
marius: but it's still css
marius: no webgl
anatol: <screenshot of IE6 displaying uncentred text>
tvararu: no problem, you ready for these top strats?
anatol: that sounds like you're getting ready to slap me
tvararu: nah, look
tvararu: I got this
marius: <table style="width: 100%; height: 100%">?
tvararu: fam you don't who you're talking to
marius: until you use that filter it's shit
```

```bash
<take screenshot of browser>
cp ~/Desktop/Screenshot.png .
```

```diff
- <H1>WHY NOT?</H1>
+ <IMG SRC="Screenshot.png" />
```

```
tvararu: check it out fam
tvararu: I even fixed the shitty font rendering on winxp
anatol: <screenshot of IE6 rendering flawlessly>
anatol: I haven't inspected the source yet
tvararu: am I a demigod or what
anatol: but it works even in compatibility mode
diana: =)))))
diana: oh my god what is going on in here
tvararu: of course, cuz I'm a god
marius: <screenshot of source code containing IMG tag>
marius: =)))))))))))))))
tvararu: BRUV.css
anatol: @tvararu... but what about SEO?
tvararu: I got dis
```

```diff
- <IMG SRC="Screenshot.png" />
+ <IMG SRC="Screenshot.png" alt="WHY NOT SEO BRUV" />
```

```
tvararu: done, fixed
anatol: :))
anatol: how about mobile?
tvararu: <screenshot of mobile browser with really tiny fonts because image scales like shit>
tvararu: it's peng, innit bruv
anatol: those fonts are tiny
marius: pretty unreadable, bruv
marius: it's SEO but it's not responsive
anatol: <screenshot of google pagespeed insights, 89/100>
tvararu: 89/100
tvararu: I'm good BRUV
tvararu: oh dude
tvararu: we need to get it down
tvararu: to 69/100
anatol: LOL
tvararu: let me just install react
anatol: don't forget the server side rendering plz, LOL
```

```bash
npm init -y
npm i --save react
```

```diff
+ <SCRIPT SRC="/node_modules/react/dist/react-with-addons.js"></SCRIPT>
```

```
tvararu: guys brainstorm more ideas to wreck the perf
marius: no that's shit
marius: npm remove react && npm install angular
tvararu: ffs dude google doesn't give a shit about my react
tvararu: still 89/100
anatol: LOL
tvararu: I'm going to put it above the fold
```

```diff
+ <SCRIPT SRC="/node_modules/react/dist/react-with-addons.js"></SCRIPT>
<!DOCTYPE HTML>
```

```
tvararu: there we go
diana: omfg this is like watching comedy
tvararu: 82/100
tvararu: guys how do I add flash
anatol: try to find some shitty wysiwyg generator
tvararu: nah dude we're not rebuilding the whole thing in flash
tvararu: just adding 1 file
tvararu: to make google mad
tvararu: I found this random game from the internet
anatol: why not a java applet?
tvararu: how do I even grab this guy's flash wtf
anatol: just wget it
tvararu: ah yeah thx
tvararu: how do you add one of these?
anatol: like this
```

```diff
+ <EMBED NAME="test" WIDTH="640" HEIGHT="400" ALIGN="middle" ID="test" SRC="cricket.swf" MENU="false" QUALITY="high" ALLOWSCRIPTACCESS="sameDomain" ALLOWFULLSCREEN="false" PLUGINSPAGE="http://www.macromedia.com/go/getflashplayer" TYPE="application/x-shockwave-flash">
```

```
tvararu: score is still 82/100 :(
anatol: .bmp?
anatol: create another site as a cdn
anatol: e.g. why69cdn.surge.sh
anatol: and request stuff from there instead so it gets mad over additional dns queries
tvararu: I'll just add something from cdnjs
tvararu: I know, mootools
```

```diff
<SCRIPT SRC="/node_modules/react/dist/react-with-addons.js"></SCRIPT>
+ <SCRIPT SRC="//cdnjs.cloudflare.com/ajax/libs/mootools/1.6.0/mootools-core.js"></SCRIPT>
<!DOCTYPE HTML>
```

```
tvararu: speed 73/100 🔥
tvararu: it's saying that CSS is nice and minified
tvararu: what is the FATTEST CSS library
tvararu: bootstrap?
anatol: yui?
tvararu: yeah let's see
tvararu: it's like 1000 different files screw it what are these guys http2
tvararu: going for bootstrap 4.0 alpha
anatol: alpha = less code
anatol: use the latest v3
tvararu: FFS OK
tvararu: the best part about my amazing image strats
tvararu: adding bootstrap won't ruin our terrible fonts
marius: =))
```

```diff

<SCRIPT SRC="/node_modules/react/dist/react-with-addons.js"></SCRIPT>
<SCRIPT SRC="//cdnjs.cloudflare.com/ajax/libs/mootools/1.6.0/mootools-core.js"></SCRIPT>
+ <LINK REL="stylesheet" HREF="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css">
<!DOCTYPE HTML>
```

```
tvararu: 69/100 SPEED GOT EM
tvararu: UX rating is still 82/100
anatol: LOL
anatol: put tiny links one next to the other
tvararu: yeah wait I got this
```

```diff
/* To break the viewport. */
body, html {
-  width: 100%;
+  width: 101%;
-  height: 100%;
+  height: 101%;
}
body {
+  font-size: 1px;
}
```

```
tvararu: 63/100 UX
tvararu: gotta fix some stuff
```

```diff
<!-- At the end of the file, of course. -->
+ <META NAME=viewport CONTENT="width=device-width, initial-scale=1">
```

```
tvararu: 67/100 UX
tvararu: I should fix something tiny
tvararu: that plugin didn't do much
```

```diff
- <EMBED NAME="test" WIDTH="640" HEIGHT="400" ALIGN="middle" ID="test" SRC="cricket.swf" MENU="false" QUALITY="high" ALLOWSCRIPTACCESS="sameDomain" ALLOWFULLSCREEN="false" PLUGINSPAGE="http://www.macromedia.com/go/getflashplayer" TYPE="application/x-shockwave-flash">
```

```
tvararu: 68/100 UX
tvararu: hnnnnngggg
anatol: ))))))))))
```

```diff
body, html {
-  width: 101%;
+  width: 100%;
-  height: 101%;
+  height: 100%;
}
```

```
tvararu: 71/100
tvararu: ffs
tvararu: alright so adding the plugin will remove 1 point
tvararu: so I can get to 68 or 70
tvararu: but not 69
tvararu: hmm
```

```diff
+ <A HREF="https://google.com/">tap</A><A HREF="https://twitter.com/">tap</A>
```

```
tvararu: 60/100
tvararu: damn it
tvararu: so basically
```

```
[x] fix content breaking viewport = +3
[x] remove plugin = +1
[x] meta viewport = +3
[ ] fix tiny fonts = +19
[ ] fix tiny tap targets = +11
```

```
tvararu: these are my tweakable inputs
tvararu: I'm at 60 currently
tvararu: but I see no way to get 69
anatol: try .bmp
tvararu: wow it's 4.3MBs
tvararu: it improved the speed to 71/100 @____@
tvararu: wat
anatol: add a huge CSS file with a big license
tvararu: that would influence speed, not UX
anatol: ah yeah damn
dragos: why is there no react on codeschool
dragos: those guys know how to explain something for retards
anatol: @dragos you're being off-topic
dragos: ffs
dragos: sup
tvararu: @dragos https://facebook.github.io/react
tvararu: stfu rtfm
anatol: you're disturbing the creative process
dragos: to hell with their docs
dragos: yo @tvararu
dragos: what's 0.1 + 0.2 in JS
tvararu: 0.3000000000004
dragos: well why??
marius: just like every other programming language
anatol: because floats
tvararu: IEEE floating point standard
anatol: <link to StackOverflow explanation>
dragos: I don't think python does that
```

```bash
$ python
Python 2.7.10 (default, Oct 23 2015, 18:05:06)
[GCC 4.2.1 Compatible Apple LLVM 7.0.0 (clang-700.0.59.5)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> 0.1 + 0.2
0.30000000000000004
>>>
```

```
tvararu: there qed
tvararu: now stfu
dragos: goood joooob
tvararu: 70/100 LADS WE GOT THIS
tvararu: just remove a plugin
tvararu: ah ffs I already did
tvararu: I'VE BEEN HERE EARLIER OMG
anatol: ))))))
anatol: use black on black text
tvararu: it already is
ilie: add some random stupid <BR>s and <DIV>s
ilie: that ought to do it
tvararu: doesn't work like that, algorithm don't care
ilie: also where are you getting the scores from
diana: pagespeed insights
tvararu: I don't think I can get 69 UX guise
tvararu: maybe if I add an interstitial overlay...
ilie: anyway, just finished reading, haven't laughed this hard in a while
marius: toasting in golden thread
marius: or rather... color: hotpink thread
tvararu: yeah, one hell of a way to spend a friday night
tvararu: k I give up
```
