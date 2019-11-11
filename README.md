# A Vim-Based Integrated Research Environment

A Vim-based academic research and writing environment, with a bare minimum of dependencies and vim plugins. Build a sprawling, densely-connected Zettelkasten, and draft academic articles, books or presentations without ever leaving Vim. 

## Why Vim

The reasons for this are simple: 1) Vim is the most powerful writing/editing technology since the invention of pen and paper, and learning to use it is truly like growing wings and ["editing at the speed of though"](https://vimeo.com/53144573); 2) the original vi program was created in 1976 (43 years ago), and Vim has been around since 1991 (28 years ago). Vim is the surest way to avoid the [impending note-taking apocalypse](https://medium.com/swlh/welcome-to-the-note-taking-apocalypse-64a74481a5ab); and 3) Vim uses good old plain text files that can be viewed and edited anywhere and as long as there are computers. 

## Can I use Something Else?

Yes, albeit with a much more limited functionality. The closest you can get in a Mac is the commendable [nvALT](https://brettterpstra.com/projects/nvalt/). And of course there's always [org-mode](https://orgmode.org/), if you're willing to give it a shot.

## Dependecies

- A recent version of [Vim](https://www.vim.org/) or Neovim.
- [Pandoc](https://pandoc.org), a universal document converter. If, like me, you make heavy use of images in your work, I recommend using the [pandoc-fignos](https://github.com/tomduck/pandoc-fignos) filter, a simple and elegant way of numbering and referencing figures. 
- [vim-pandoc](https://github.com/vim-pandoc/vim-pandoc) and [vim-pandoc-syntax](https://github.com/vim-pandoc/vim-pandoc-syntax).
- A decent color scheme, such as [solarized](https://github.com/altercation/vim-colors-solarized) or [gruvbox](https://github.com/morhetz/gruvbox).
- [goyo](https://github.com/junegunn/goyo.vim), distraction-free writing in Vim.
- [fzf](https://github.com/junegunn/fzf), the command-line fuzzy finder.
- [ag](https://github.com/ggreer/the_silver_searcher), a powerful searching tool.
- A `bibtex` bibliography file, or a reference manager that can produced it, such as Zotero with [Better BibTeX](https://github.com/retorquere/zotero-better-bibtex) or [JabRef](https://www.jabref.org/).
- For previewing: [Zathura](https://pwmt.org/projects/zathura/) in any *nix distro, or [Marked2](https://marked2app.com/), in macOS. (Optional: you can also use any browser or PDF viewer.)

## Preliminaries and Conventions

- All files (notes, outlines, quotes, drafts, etc.) are to be kept in plain text markdown. If you're still not convinced why, read [this](https://programminghistorian.org/en/lessons/sustainable-authorship-in-plain-text-using-pandoc-and-markdown) and [this](http://wcaleb.org/blog/my-academic-book-in-plain-text). Plain text files are small and sustainable, do not tie you to a specific editor, and can be used with version control systems such as Git.
- I strongly recommend keeping all your text files in a single folder, regardless of project, source, etc. Inspired by Luhmann's Zettelkasten system and my own experience, the IRE is based on the conviction that file classification (through a directory structure, tags, keywords, or strict file-naming) is a total waste of time. As Luhmann noted, [categories foreclose the free braching of the Zettelkasten](https://zettelkasten.de/posts/no-categories/), and cannot predict in advance the twists and turns that your ideas and your reading might take. The constant updating of directory structures and tag ontologies is energy-consuming and yields few results. The IDE favors the quick creation of content and the branching of the database.
- Instead of taxonomy, the IRE is based on the principle that the "life" of a note—its retrievability but also its capacity to elicit new ideas—hinges on the density of cross-references among the notes. A dead note is a note with no links braching from it or leading to it. Thus, the IRE is designed to ease the establishment of cross-references, through hyperlinks and other techniques.And instead of cumbersome naming, filing or tagging, the IRE favors the creation of ad hoc indexes (lists of notes) and indexes of indexes.
- The use of hyperlinks and Vim's powerful autocompletion and search functions makes the question of file naming of less crucial significance than it held for Luhmann's system. Any sensible and sufficiently descriptive file naming convention (like [this one](https://library.stanford.edu/research/data-management-services/data-best-practices/best-practices-file-naming)) will work. In general, you should always use file names with camel case (`DasCapital.md`) or dashes (`das-Capital.md`). Avoid at all costs non-human-readable ID naming schemes, such as those favored by Luhmann himself. For reasons that will become clear later, I strongly recommend naming reading notes with the book's or article's `bibtex`key (i.e. `marx1867capital.md`), which by the way also implies that you should choose those keys wisely.

Reading more: [Manfred Kuehn, "Some Idiosyncratic Reflections on Note-Taking in General"](https://www.connectedtext.com/manfred.php), [Christian Tietze, "Create a Zettelkasten for your Notes to Improve Thinking and Writing"](https://zettelkasten.de/posts/zettelkasten-improves-thinking-writing/) and [Niklas Luhman's original "Communicating with Slip-Boxes"](https://luhmann.surge.sh/communicating-with-slip-boxes). 

## General Idea

While there are many plugins for creating a wiki-like systems in Vim (`vim-wiki` being the most popular one), the IRE relies entirely on Vim standard commands, thus avoiding the idiosyncrasies of those plugins. Vim's powerful navigation and search functions makes it possible to treat any plain text file as a wiki, so technically the IRE would work with non-markdown text files. `vim-pandoc`and `vim-pandoc-syntax` simply offer some convenient functionality for writing in markdown, such as syntax highlighting and concealment, structure folding, `bibkey`completion, previewing, etc. `fzf` and `ag` add file-name fuzzy finding and advanced content search across files. `goyo` offers a tidy writing environment, reminiscent of popular full-scree writing apps. Nothing more, nothing less. 

## Features
