# writer-slideshow-template

> iA Writer template that turns Markdown document into a simple slideshow

![](https://www.annefortuin.nl/writer-slideshow-template.png)

This [iA Writer](https://ia.net/writer) template turns a simple Markdown file into a simple slide deck, as inspired by [this Tweet from 2016](https://twitter.com/iawriter/status/766580903116017664). It splits the HTML output of a Markdown file into slides by use of the horizontal ruler (`<hr>` element in HTML, or `---` in Markdown):

```markdown
# Welcome to my slideshow

This is my first slide.

---

This is my second slide!
```

When going into preview mode in iA Writer, each slide is rendered 'full screen'. You can navigate forward by using the <kbd>→</kbd> (right), <kbd>↓</kbd> (down) and <kbd>⎵</kbd> (space) keys. Navigate back with <kbd>←</kbd> (left), <kbd>↑</kbd> (up) and <kbd>⌫</kbd> (backspace) keys.

## Installation and usage

- Clone this repository or [download as a zip](https://github.com/phortuin/writer-slideshow-template/releases)
- Double-click the `Slideshow.iatemplate` template in Finder

To use the template, do any of these things:

- Select the _Slideshow_ template via the _Templates_ preference pane
- Select it in the menu _View > Templates > Slideshow_
- When previewing your document, select _Slideshow_ from the toolbar at the bottom of the screen

[More information can be found here](https://github.com/iainc/iA-Writer-Templates#installing-templates).

## Typography

The template was styled around [Adelle Sans](https://www.type-together.com/adelle-sans-font) and [MonoLisa](https://www.monolisa.dev/). They’re not free and [I didn’t include webfont files in this repository](https://pixelambacht.nl/2017/github-font-piracy/). The fallback fonts should look fine. However, if you have access to the following font files, you can put them in the `Slideshow.iatemplate/Contents/Resources/fonts` folder:

```
fonts/AdelleSans-Regular.woff
fonts/AdelleSans-Regular.woff2
fonts/AdelleSans-Bold.woff
fonts/AdelleSans-Bold.woff2
fonts/MonoLisa-Regular.woff
fonts/MonoLisa-Regular.woff2
```

**Tip:** the `Slideshow.iatemplate` ‘file’ can be opened like a regular folder by right-clicking it in Finder and choosing _Show Package Contents_. Remember to reinstall the template after changing its contents.

## Possible FAQ

**Does it support Dark mode?**\
Yes, it does (see _Appearance → Dark_ in preferences).

**Can I print my slides?**\
This template doesn’t support printing to paper or PDF. It will likely throw an error. A simple solution is to choose a (built-in) template that does support printing.

**Does it work on iOS?**\
No, I expect it to break ungloriously.

**The slideshow sort of breaks after I edited some text. What gives?**\
Because Writer tries to sync the preview scroll position with the editor scroll position, the slideshow position and behavior may break. Your best bet is to right-click in the preview and click _Reload_. Putting the cursor at the top of the editor might also work.

**Can I have horizontal sliding?**\
Horizontal sliding would be cool, but is much harder to implement than vertical sliding, since a browser’s natural behavior is to move vertically (iA Writer preview uses the Safari browser engine).

**Why won’t the template respond to changing the text size?**\
The template is responsive to window size, but ignores zoom/text size settings. The reason is that a presentation is built to balance large font sizes and the right amount of room for content. Adopting variable text sizes would make it harder to find this balance.

**Why can’t I...**\
If you want more features, I can heartily recommend [Deckset](https://www.deckset.com/).

## License

[MIT](/license)
