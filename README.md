# BIG-Culture Website

This is the repository for [BIG-Culture's website](https://big-culture.github.io/).
Built using the [al-folio](https://github.com/alshedivat/al-folio) theme for [Jekyll](https://jekyllrb.com/).

## How to Contribute

1. Download [GitHub Desktop](https://desktop.github.com/)
2. Clone this repository [(guide)](https://docs.github.com/en/desktop/adding-and-cloning-repositories/cloning-and-forking-repositories-from-github-desktop#cloning-a-repository)
3. Edit and add content as required (an IDE such as [WebStorm](https://www.jetbrains.com/webstorm/) or [VSCode](https://code.visualstudio.com/) is suggested)
4. Push your changes [(guide)](https://docs.github.com/en/desktop/making-changes-in-a-branch/pushing-changes-to-github-from-github-desktop)

## Adding Content

### Blog Posts

To create a new blog post, you can add a new Markdown file in the [\_posts](_posts/) directory. The [name of the file must follow](https://jekyllrb.com/docs/posts/#creating-posts) in the format `YYYY-MM-DD-title.md`. The easiest way to do this is to copy an existing blog post and modify it. Note that some blog posts have optional fields in the [frontmatter](https://jekyllrb.com/docs/front-matter/) that are used to enable specific behaviours or functions.

If you want to create blog posts that are not ready to be published but you want to track them with git, you can store them in the [\_drafts](_drafts/) directory.

### People

You can add a new person by adding a new Markdown file in the [\_people](_people/) directory.

### Projects

You can create new projects by adding new Markdown files in the [\_projects](_projects/) directory. The easiest way to do this is to copy an existing project and modify it. Note that some blog posts have optional fields in the [frontmatter](https://jekyllrb.com/docs/front-matter/) that are used to enable specific behaviours or functions.

### Publications

To add publications, create a new entry in the [\_bibliography/papers.bib](_bibliography/papers.bib) file. You can find the BibTeX entry of a publication in Google Scholar by clicking on the quotation marks below the publication title, then clicking on "BibTeX", or also in the conference page itself. By default, the publications will be sorted by year, and the most recent ones will be displayed first. You can change this behavior and more in the `Jekyll Scholar` section in [\_config.yml](_config.yml) file.

You can add extra information to a publication, like a PDF file in the `assets/pdfs/` directory and add the path to the PDF file in the BibTeX entry with the `pdf` field. Some of the supported fields are: `abstract`, `altmetric`, `arxiv`, `bibtex_show`, `blog`, `code`, `dimensions`, `doi`, `eprint`, `html`, `isbn`, `pdf`, `pmid`, `poster`, `slides`, `supp`, `video`, and `website`.

An example of adding additional fields can be seen in sensabubble:

```
bibtex_show={true},
pdf = {https://dl.acm.org/doi/pdf/10.1145/2556288.2557087},
preview = {sensabubble.png},
html = {https://doi.org/10.1145/2556288.2557087},
video = {https://www.youtube.com/watch?v=JGUmf4HqTxM},
abbr = {CHI}
```

## Current TODOs

Current TODOs can be found in [TODO](TODO.md)

# License

The theme is available as open source under the terms of the [MIT License](https://github.com/alshedivat/al-folio/blob/master/LICENSE).
Originally, [al-folio](https://github.com/alshedivat/al-folio) was based on the [\*folio theme](https://github.com/bogoli/-folio) (published by [Lia Bogoev](https://liabogoev.com) and under the MIT license).
