# Markdown Resources

[Markdown](http://en.wikipedia.org/wiki/Markdown) is a [lightweight markup language](http://en.wikipedia.org/wiki/Lightweight_markup_language), similar to [AsciiDoc](http://en.wikipedia.org/wiki/AsciiDoc), [MediaWiki](http://en.wikipedia.org/wiki/MediaWiki), [Org-mode](http://en.wikipedia.org/wiki/Org-mode), [reStructuredText](http://en.wikipedia.org/wiki/ReStructuredText), [Textile](http://en.wikipedia.org/wiki/Textile_(markup_language)), and many others.[^1]


## About Markdown (and the purpose of this collection)

Markdown is said to be “invented” by John Gruber, who, in any case, worked on it together with [Aaron Swartz](http://en.wikipedia.org/wiki/Aaron_Swartz) (1986–2013). Since the release of “original” Markdown in 2004, the language has been “forked” many times over. Today, there are several “[extensions](http://en.wikipedia.org/wiki/Markdown_extensions)” and dialects in circulation. Many more apps have been created (for the Web, OSX, iOS, Android, Windows).

Depending on the specific Markdown implementation (parser) those apps use under the hood, they support one or more Markdown dialects or “flavors”. It is not always obvious to end users which apps (and backend scripts) can do what exactly. This collection of resources tries to clear up some of that confusion.


## This repo

At the moment the repository has lists for Markdown editors (apps with a graphical user interface), dialects/extensions, implementations, and stylesheets (themes in `css`):

- [Markdown Apps](markdown-apps.yml)
- [Markdown Dialects](markdown-dialects.yml)
- [Markdown Implementations](markdown-implementations.yml)
- [Markdown Stylesheets](markdown-stylesheets.yml)

The lists are formatted using [YAML](http://en.wikipedia.org/wiki/YAML). Not unlike Markdown, YAML is a lightweight markup language with a syntax that is intended to be easily readable by  humans, all while formally structured for machine processing. But unlike Markdown, YAML is more suited to author, edit, and store non-sequential data.

Feel free to grab the `.yml` files, [convert them into `.json`](http://nodeca.github.io/js-yaml/), `.xml` or whatever suits your needs, and import them into a searchable data store. Enjoy!

### Wiki

If you want to quickly add a Markdown editor app that is not on the list already, you can do so on the [wiki page](https://github.com/rhythmus/markdown-resources/wiki/Markdown-Apps).

## Discussion

There’s a [Markdown Community Page on GitHub](http://markdown.github.io/), but it seems it never got further than initial enthusiasm. There’s also an official [W3C Markdown Community Group](http://www.w3.org/community/markdown/), but that too seems abandoned. The actual discussion on Markdown takes place at the [Markdown mailing list](http://six.pairlist.net/mailman/listinfo/markdown-discuss) — and on private blogs…

---

[^1]: This document (`README.md`) is itself formatted using the GitHub Flavored Markdown dialect. The specs are [here](https://help.github.com/articles/github-flavored-markdown). The repo is kept at <https://github.com/rhythmus/markdown-resources>.