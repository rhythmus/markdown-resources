# Markdown Resources

[Markdown](http://en.wikipedia.org/wiki/Markdown) (John Gruber & Aaron Swartz, 2004) is a [lightweight markup language](http://en.wikipedia.org/wiki/Lightweight_markup_language), similar to [Setext](http://en.wikipedia.org/wiki/Setext) (Ian Feldman, 1992), [AFT](http://www.maplefish.com/todd/aft.html) (Todd Coram, 1999), [Grutatxt](http://www.triptico.com/software/grutatxt.html) (Ángel Ortega, 2000), [atx](http://www.aaronsw.com/2002/atx/intro) (Aaron Swartz, 2002), [AsciiDoc](http://en.wikipedia.org/wiki/AsciiDoc) (Stuart Rackham, 2002), [MediaWiki](http://en.wikipedia.org/wiki/MediaWiki) (Magnus Manske & Lee Daniel Crocker, 2002), [reStructuredText](http://en.wikipedia.org/wiki/ReStructuredText) (David Goodger, 2002), [Org-mode](http://en.wikipedia.org/wiki/Org-mode) (Carsten Dominik, 2003), [Textile](http://en.wikipedia.org/wiki/Textile_(markup_language)) (Dean Allen, 2004), and many others (listed [here](http://en.wikipedia.org/wiki/Lightweight_markup_language#Comparison_of_language_features),
[here](http://micans.org/zoem/ecosphere.html) and [here](http://outl.sourceforge.net/lightweight.html)).[^1]

Lightweight markup languages are abundant. Markdown seems to have have won the race, but its popularity comes at a cost. Whereas original Markdown in its early days, ca 2004, had to compete with many alternatives, today it is clearly king, but its realm is falling apart into many baronnies. Markdown dialects, forks, and supersets, are competing amongst each other. While they all remain true to the original Markdown syntax subset, new initiatives arise, which abandon the Markdown syntax. Noteworthy are [SkrivML](http://markup.skriv.org/) and [z.](http://www.z-m-l.com/)[m.](http://zenmagiclove.com/marchforth/march-forth-manifesto.zml)[l.](http://zenmagiclove.com/phrase-change-display.html) [Rumor](https://twitter.com/jpleboeuf/status/459739776858718208) has it that there is even a “Markdown Operating System” in the make…


## About Markdown (and the purpose of this collection)

Markdown is said to be “invented” by [John Gruber](http://en.wikipedia.org/wiki/John_Gruber), who, in any case, worked on it together with [Aaron Swartz](http://en.wikipedia.org/wiki/Aaron_Swartz) (1986–2013). Since the release of “original” Markdown in 2004, the language has been “forked” many times over. Today, there are several “[extensions](http://en.wikipedia.org/wiki/Markdown_extensions)” and dialects in circulation. Many more apps have been created (for the Web, OSX, iOS, Android, Windows).

Depending on the specific Markdown implementation (parser) those apps use under the hood, they support one or more Markdown dialects or “flavors”. It is not always obvious to end users which apps (and backend scripts) can do what exactly. This collection of resources tries to clear up some of that confusion.


## This repo

At the moment the repository has lists for Markdown editors (apps with a graphical user interface), dialects/extensions, implementations, and stylesheets (themes in `css`):

- [Markdown Editors: native apps](markdown-editors-nativeApps.yml)
- [Markdown Editors: browser-based](markdown-editors-browserBased.yml)
- [Markdown Dialects](markdown-dialects.yml)
- [Markdown Implementations](markdown-implementations.yml)
- [Markdown People](markdown-people.yml)
- [Markdown Stylesheets](markdown-stylesheets.yml)

Feel free to grab the `.yml` files, [convert them into `.json`](http://nodeca.github.io/js-yaml/), `.xml` or whatever suits your needs, and import them into a searchable data store. Enjoy!


### On the use of YAML

The lists in this repo are formatted using [YAML](http://en.wikipedia.org/wiki/YAML). Not unlike Markdown, YAML is a lightweight markup language with a syntax that is intended to be easily readable by  humans, all while formally structured for machine processing. But unlike Markdown, YAML is more suited to author, edit, and store non-sequential data.

YAML and Markdown only seem to be competing languages, but they are not mutually exclusive. Indeed, some Markdown editors and implementations even support YAML: while the document’s body is formatted in Markdown syntax, its front matter (metadata) is structured using YAML syntax. Just like documents can exist without front matter, and be formatted in Markdown exclusively, so can documents consist out of nothing else than ~~(meta)~~data and be completely formatted in YAML.

One might put it like this: Markdown is for text (i.e. text that is meant for continuous reading), while YAML is for structured data (not sequentially read, but randomly accessed/queried).

While both languages are concise enough to be easily read in raw format by a human editor, the intended output of a text file formatted in Markdown is a (typographically) styled document, whereas a text file formatted in YAML is expected to be eventually read into a datastore.


## Contributions

Markdown is gaining enormous popularity and dozens of implementations and applications are pumped out almost every single week, it seems. Maybe one could set up some sort of automated tracking, but as it stans now, the present collection is curated manually. It cannot be exhaustive without some help, and contributions are gratefully welcomed!

Please fork, edit, commit, and send pull requests, or just [file an issue](https://github.com/rhythmus/markdown-resources/issues).

Alternatively, if you want to quickly add a Markdown resource (that is not on a list already), and you don’t like how the YAML format is presented by Github, you can do so on the [Wiki](https://github.com/rhythmus/markdown-resources/wiki).


## Discussion

There’s not much room for discussion here on Github, and the present repo is just a shared store of resources. If you want to take part in the vibrant discussions on the future of Markdown, there’s no exact place to point to.

There’s a [Markdown Community Page on GitHub](http://markdown.github.io/), but it seems it never got further than some initial enthusiasm. There’s also an official [W3C Markdown Community Group](http://www.w3.org/community/markdown/), but that too seems abandoned. The actual discussion on Markdown takes place at the [Markdown mailing list](http://six.pairlist.net/mailman/listinfo/markdown-discuss), and on private blogs.


## Other useful Markdown resources

While this entire repository is made up of links to useful Markdown resources, the following stand apart as they too are curated collections of links to other Markdown resources, and/or provide more context.

- <http://whatismarkdown.com/>
- <http://markdowntutorial.com/>
- <http://johnmacfarlane.net/babelmark2/faq.html> – Testing and comparison suite for Markdown implementations, by John MacFarlane.

---

[^1]: This document (`README.md`) is itself formatted using the GitHub Flavored Markdown dialect. The specs are [here](https://help.github.com/articles/github-flavored-markdown). The repo is kept at <https://github.com/rhythmus/markdown-resources>.
