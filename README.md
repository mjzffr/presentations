# Requirements

* reveal.js is available at path `$REVEALJS` (see https://github.com/hakimel/reveal.js#basic-setup)
* pandoc is installed. (see https://github.com/jgm/pandoc/wiki/Using-pandoc-to-produce-reveal.js-slides)

# Example

```
pandoc -t revealjs -s -o out.html in.md -V revealjs-url="../reveal.js" -V transition="none" -V slideNumber="true" -V theme=black --slide-level 2 --highlight-style=zenburn -H ../presentation_mods.css.extra
```

Note that pandoc doesn't use the highlight.js dependency in reveal.js; instead
it provides its own syntax highlighting.

For notes:

```
pandoc -t html -s -o out.html in.md --highlight-style=tango -H ../notes.css.extra
```
