# starter for ten

Just my current set of files which I tend to use when starting a new website. It changes all the time, it's probably of no use to anyone but me but if you're interested, right now, this is what I tend to start with.

So taking the HTML, CSS, and JavaScript element in order.

## HTML

Mostly this is nicked from HTML5 Boilerplate.

<http://html5boilerplate.com/>

I've taken some of the basic HTML template and the various meta-tag and icons etc. Oh and the .htaccess file that they have which is AWESOME! ;-) They also use a lot of good standard stuff like the IE conditional comment on the HTML tag and stuff like that. I've got some HTML polyfill things (and even belatedPNG - remember that?!) in at the bottom and some boilerplate Google Analytics code (as a reminder as much as anything).

## CSS

I used to have [Inuit.css](http://inuitcss.com/) in here, but I've removed it for now. I still really like it but for some of the littler projects and things I've been doing it was more than I needed. Rather than spend a lot of time removing bits of it I thought I'd start without it and add it back in when needed.

I still use [Harry](http://csswizardry.com/)'s [CSSWizardry-Grids](https://github.com/csswizardry/csswizardry-grids) which are an excellent off-shoot of Inuit.css and still the favourite CSS grid system I've found so far.

As well as that I use: 
- Normalize <http://necolas.github.io/normalize.css/>
- Typeplate <http://typeplate.com/>

Also I'm a big fan of [SMACSS](http://smacss.com/) which although I don't always follow religiously is definitely on my list of "things I must try harder at". So I've started putting in placeholder SCSS files for the different elements of that.

## Javascript

This is just a load of .js files and libraries which I've gathered in order to make use of them as quickly and easily as possible. There's `modernizr.js` in the head but the rest go at the foot of the page. I'm currently using the "get jQuery from a CDN" code (with a fall-back to local) but from recent reading I'm beginning to think just wrapping it into my `all.min.js` might be better.

Talking of which all these libaries etc that I want to juse are kind of gathered into a `/lib/` folder. You'll notice in there there's an `-order.txt` file. This is used for a custom built JavaScript minifier which I use. It's basically the [YUI JS compressor](http://yui.github.io/yuicompressor/) which is triggered by a PHP script which is us to "watch" the `/js/` directory and concat and minify them and spit out a single `all.min.js` file.

I may stick that PHP script up at some point. It's definitely not rocket science, but knowing a bit of PHP I was able to get it working quite easily before I was aware of all the myriad other ways to manage that kind of stuff. It's working for me right now until I can find the time to learn a better method.
