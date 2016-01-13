<!--
Markdown Resources: Varia
==========================================
Copyright 2013–2016 © Dr Wouter Soudan @ Rhythmus.be
Licensed under a Creative Commons Attribution 3.0 License.

Document address: https://github.com/rhythmus/markdown-resources/markdown-tools.md
Last revision: 2016-01-13 17:45 GMT+1
-->

# Various Markdown Tools


## Preview raw Markdown with style

Dedicated stylesheets, specifically designed to make up html that was output from Markdown, are [listed separately](markdown-stylesheets.yml) (in YAML format). Low-level parsers doing MD → html conversion are [listed separately](markdown-implementations.yml), too. Going the other way around (html → MD), there’s of course [Pandoc](http://johnmacfarlane.net/pandoc/) (which does both, and much more), and these two:

- [reMarked.js](http://leeoniya.github.io/reMarked.js) ([repo](https://github.com/leeoniya/reMarked.js)) – “The ultimate goal is integration with existing WYSIWYG html editors (eg: Redactor, TinyMCE, CKeditor, Loki, CLeditor, [[and Quill](https://github.com/quilljs/quill/issues/74)]) to produce Markdown output. There are currently no WYSIWYG editors for markdown, only WYSIWYM, which still require knowledge of markdown syntax and its many quirky flavors.”
- [to-markdown.js](http://domchristie.github.io/to-markdown/) ([repo](https://github.com/domchristie/to-markdown))

Listed below are applications (with user interfaces), which use one or more of the above scripts, libraries, and other dependencies.

### Browser extensions
- [Markdown Here](http://markdown-here.com) ([Chrome](https://chrome.google.com/webstore/detail/markdown-here), [Firefox](https://addons.mozilla.org/en-US/firefox/addon/markdown-here), [Safari](https://s3.amazonaws.com/markdown-here/markdown-here.safariextz), [Thunderbird](https://addons.mozilla.org/en-US/thunderbird/addon/markdown-here/)) ([repo](https://github.com/adam-p/markdown-here)) – Targetted at previewing and editing (formatting) email, but hijacks any `<textarea>` or `contentEditable` element as well. Table support (GFM).
- [Markdown Preview](https://chrome.google.com/webstore/detail/markdown-preview) (Chrome) ([repo](https://github.com/borismus/markdown-preview)) – Preview local and remote `.md`|`.markdown` files.
- [Markdown Preview Plus](https://chrome.google.com/webstore/detail/markdown-preview-plus) (Chrome) – Preview local and remote `.md`|`.markdown` files.
- [Markdown Viewer](https://chrome.google.com/webstore/detail/markdown-viewer) (Chrome) – Outline (table of contents), table support (GFM), auto reload local file on change.
- More in the [Chrome Web Store](https://www.google.com/search?q=chrome+extension+markdown)…

### MD → html (native)
- [Marked2](http://marked2app.com) (OSX) – The famous dedicated Markdown preview app for the Mac; to be used in pair with [any Markdown editor](markdown-editors-nativeApps.yml).

### MD → html (web)
- [Strapdown.js](http://strapdownjs.com) ([repo](https://github.com/arturadib/strapdown)) – Uses Marked.js parser.

### Html → md
- [FuckYeahMarkdown.com](http://fuckyeahmarkdown.com/) — Converts any URL’s contents (using the [Readability parser API](https://www.readability.com/developers/api)) from html to markdown.


### MD ↔ html (browser-based WYSIWYG Markdown editor)

[_Some day…_](https://github.com/quilljs/quill/issues/74#issuecomment-42942223)

- [Demarcate.js](http://will-hart.github.io/demarcate.js/) ([repo](https://github.com/will-hart/demarcate.js))
- [lepture/editor](http://lab.lepture.com/editor/) ([repo](https://github.com/lepture/editor)) — Built on CodeMirror.
- [sofish/pen](http://sofish.github.io/pen/) ([repo](https://github.com/sofish/pen))
- [Hallo.js](http://hallojs.org/demo/markdown/) ([repo](https://github.com/bergie/hallo))
- [md-wysiwyg](http://md-wysiwyg.sourceforge.net/) (python; [demo](http://md-wysiwyg.sourceforge.net/cgi-bin/cgi_wysiwyg_test.py/)  — Simple html editor that outputs Markdown.
- [Mathdown](http://mathdown.net/) ([repo](https://github.com/cben/mathdown); [my fork](https://github.com/rhythmus/mathdown)) — Markdown with MathJax (for LaTeX equations) and Firepad (for real-time collaboration); built on CodeMirror.

## Editing

### General-purpose Markdown editors
- Native apps: [listed separately](https://github.com/rhythmus/markdown-resources/blob/master/markdown-editors-nativeApps.yml) (in YAML format).
- Web apps: [listed separately](https://github.com/rhythmus/markdown-resources/blob/master/markdown-editors-browserBased.yml) (in YAML format).
### Note-taking

- [Drafts](http://agiletortoise.com/drafts) — iOS note taking app

- [Notal for Android](http://fusionfenix.com/product/notal-android) — “Notal is a simple application that lets you take notes with Markdown style.” 

- [nvPY](https://github.com/cpbotha/nvpy) — “Simplenote syncing note-taking application, inspired by Notational Velocity and ResophNotes, but uglier and cross-platformerer.”


### Editing Markdown tables
- [Tables Generator](http://www.tablesgenerator.com/markdown_tables) — An online tool to create tables in a graphical interface, and have them exported into (extended) Markdown, using the syntax of GFM and MMD.
- [Table Editor](http://truben.no/latex/table/) — An online tool to create tables in a graphical interface, and have them exported into BBCode, CSV, HTML, JSON, LaTex, Mathematica, SQL, Wiki markup, and Markdown, using a simple pipe delimiter syntax.
- [Sublime Table Editor](https://github.com/vkocubinsky/SublimeTableEditor) – A Sublime Text (ST2, ST3) package for editing “ASCII art” tables in plain text files, using the syntaxes of EmacsOrgMode, Pandoc, reStructuredText, Textile, and Multi Markdown. Can convert csv into such table.
- [CSV to MMD](http://brettterpstra.com/2012/03/29/experiment-csv-to-mmd-tables-with-color-coding) — An experiment by Brett Terpstra to convert a Google Docs spreadsheet to color-coded html tables, going over MultiMarkdown.

<!-- 
- http://lou.pe/blog/converting-csv-tables-to-markdown-files
- http://tonylandis.com/python/python-csv-to-fixed-sized-text-tables/
-->

### Sanitize crufty Markdown formatting
- CLI: `$ pandoc -t markdown --atx-headers --no-wrap uglyfile.md`
- markdownfmt (Go; [repo](https://github.com/shurcooL/markdownfmt)) — “Like gofmt, but for Markdown.”


## Easy Markdown-based publishing 

### Anonymous publishing (Pastebin-style)
- [Notehub](http://www.notehub.org) (Clojure; [repo](https://github.com/chmllr/NoteHub)) — Support for plain original Markdown, using the Pagedown.js parser. Custom styling possible within `<style>`. Password-protected editing.
- [peg](http://peg.gd/1)
- [MarkdownShare.com](http://markdownshare.com/) (Perl; [repo](https://github.com/skx/markdown.share/)) — Emoji support, submission API, editable after publication.

### Prettified .md Github gists
- [Gist.io](http://gist.io/) (Python; [repo](https://github.com/idan/gistio)) — Client-side markdown processing.
- [Jist.in](http://jist.in/) (Javascript; [repo](https://github.com/zhuzhuor/jist/)) — Client-side markdown (GFM) processing ([marked.js](https://github.com/chjj/marked) parser), multiple `.md` files, custom css.
- [Mkdown.com](http://www.mkdown.com/8485599) (Ruby; [repo](https://github.com/jack7890/mkdown)) – Server-side pre-compilation, serves static html, hence no Javascript needed client side. Supports public and privat gists.
- [GitPrint.com](http://gitprint.com/) (Javascript; [repo](https://github.com/adamburmister/gitprint.com)) – Render Github markdown documents for printing.

### Self-hosted static site generators
- Apache handler (php; [repo](https://github.com/sminnee/markdown-handler)) – View `.md` named files more prettily on your webserver.
- Brog (Go; [repo](https://github.com/aybabtme/brog)) –
Deploy a collection of .md files, in a blog structure; server compiles, serves html, watches the blog path and reloads/recompiles Markdown and Templates when they change.
- [Calepin](http://calepin.co/) (Javascript & Python; [repo](https://github.com/jokull/calepin)) – Gets Markdown files from Dropbox, converts into blog posts, generates an Atom feed.
- [Contentify](http://thyb.github.io/contentify) ([repo](https://github.com/thyb/contentify/)) – Collaborative content manager in realtime over Github and Github Pages.
- [Lanyon](http://ebeab.com/2014/05/07/lanyon-a-markdown-web-server/) (Go; [repo](https://github.com/mkaz/lanyon)) — Simple web server, which reads directories of markdown files and converts them to HTML and serves.
- docstore (javascript; [repo](https://github.com/haldean/docstore)) — Simple client-side script that makes an ajax request to server, compiles Markdown, displays html. Interesting spin-off, using S3: [Composedit.net](http://composedit.net/)
- More [here](http://staticsitegenerators.net/), [here](http://staticgen.com/), and [here](https://gist.github.com/davatron5000/2254924); most of them take a pile of Markdown files as the input…

### Documentation generators & wikis
- [Ditto](http://chutsu.github.io/ditto/) (Javascript; [repo](https://github.com/chutsu/ditto/)) — Markdown code base documentation system.
- [MDwiki](http://dynalon.github.io/mdwiki/) (Javascript; [repo](https://github.com/Dynalon/mdwiki/)) — CMS/Wiki 100% client-side (marked, jQuery, Bootstrap, Bootswatch, colorbox, highlightjs).
- [Scribble](http://www.tryscribble.com) – “Simple Markdown Wikis”

### Hosted publishing
- [Draft.in](https://draftin.com) – Collaborative writing with version control.
- [Penflip.com](https://www.penflip.com/) – Collaborative writing with version control.
- [gOrge](http://gorgeapp.appspot.com/) – “New, simpler, bea[u]tiful and better mail list for the 21st century.” “… create a new discussion thread and share with everybody in the world your discussion…”
- [Visualmarks](http://www.visual-marks.com)
