# starter for ten

Just my current set of files which I tend to use when starting a new website. It changes all the time, it's probably of no use to anyone but me but if you're interested, right now, this is what I tend to start with.

So taking the HTML, CSS, and JavaScript element in order.

## HTML

Mostly this is nicked from HTML5 Boilerplate.

<http://html5boilerplate.com/>

I've taken some of the basic HTML template and the various meta-tag and icons etc. Oh and the .htaccess file that they have which is AWESOME! ;-) They also use a lot of good standard stuff like the IE conditional comment on the HTML tag and stuff like that. I've got some HTML polifil things (and even belatedPNG - remember that?!) in at the bottom and some boilerplater Google Analytics code (as a reminder as much as anything).

## Inuit.css

<http://inuitcss.com/>

Secondly there's inuit.css (by [Harry Roberts](https://twitter.com/csswizardry)) which I've recently stuck in there (replacing a ragtag bunch of CSS bits and pieces which I used to have). It seems really cool and it's bound to be better thought-out than the stuff I was using before. So this is partly a learning thing. I may move on (or more likely hack it up) later so don't expect what's in there to be a real, approved (or even working) verison of Inuit.

## Javascript

The only thing worth mentioning is that the javascript is kind of gathered into a /lib/ folder. You'll notice in there, theres a -order.txt. This is used for a custom built JavaScript minifier which I use. It's basically the [YUI JS compressor](http://yui.github.io/yuicompressor/) which is triggered by a PHP script which is us to "watch" the /js/ directory. I may stick that PHP script up at some point but until then all you really need to know is that anything I want to use I name in the -order.txt file and it gets stuck into all.min.js for me by the script.

(There are loads of better ways of doing that I'm sure but for now I'm happy with what I've got).