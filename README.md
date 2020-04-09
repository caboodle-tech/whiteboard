# Whiteboard
Whiteboard is a (mostly) standalone JavaScript backed web based whiteboard. As long as a users browser or device supports HTML canvas elements you can transform any DIV element on a page into a whiteboard. For the best experience possible the whiteboard should fill the browser and be the only element on the page.

### Seeing is Believing!
Check out the [live demo](https://caboodle-tech.github.io/whiteboard/index.html) to see whiteboard in action. The demo page is kept very minimal so viewing the source code should teach you all you need to know to get Whiteboard working for you.

### Where are the source files!?
Everything you need is in the docs folder. If you plan to integrate Whiteboard into your own project this reference table will help:

File | Where is it? | What is it?
---|---|---
whiteboard.js | docs/js/whiteboard.js | This is the main app script.
katex.min.js | docs/js/katex.min.js | This is the library that takes LaTeX math and turns it into human readable math.
katex.css | docs/css/katex.css | KaTeX can't work without it's styles. This will also load the fonts from the font directory which should be in the same directory.
fonts* | docs/css/fonts/* | All the font files needed for KaTeX to work on as many browsers as possible.

Here is a handy guide to the rest of the files and directories in this GitHub repo and why we have them:

File | Where is it? | What is it?
---|---|---
rescources | ./ | Anything useful to whiteboards development but not needed in production.
FontAwesomeLicense.md | ./ | The license file for the free Font Awesome SVG icons Whiteboard uses.
LICENSE | ./ | Whiteboard's license file.

### Getting Started
Once you have all the files as explained in the source files table or from the `docs` directory you only need two things:

1) A DIV element on your page with an ID; and nothing else inside it.

```html
<div id="page-wrapper"></div>
```

2) JavaScript to kick everything off:

```javascript
var board = new Whiteboard();
board.init( 'page-wrapper' );
```

### Can I Help?
Yes you can! Whiteboard was developed with the mindset of helping teach University classes online; I developed this as a professor. If you share that vision, please help me grow and maintain whiteboard.

If you have other use cases for Whiteboard please feel free to add them and submit a pull request. As long as the changes don't make it hard for students to use Whiteboard it will probably get merged.
