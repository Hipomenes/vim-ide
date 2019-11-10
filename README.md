# A Vim-Based Integrated Research Environment

A Vim-based academic research and writing environment, with a bare minimum of dependencies and vim plugins. Build a sprawling, densely-connected Zettelkasten, and draft academic articles, books or presentations without ever leaving Vim.  

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

## Preliminaries

- All files (notes, quotes, drafts, etc.) are ir plain text markdown. If you're still not convinced why, read ["Sustainable Authorship in Plain Text"](https://programminghistorian.org/en/lessons/sustainable-authorship-in-plain-text-using-pandoc-and-markdown).
- I strongly recommend keeping all your text files in a single folder, regardless of project, etc. I know, I known, but this anti-organizational principle is crucial. Inspired by Luhman's Zettelkasten system and my own experience, the IRE is based on the idea that file classification (through a directory structure, tags, strict file naming) is an total waste of time. As Luhman noted, taxonomies foreclose the free braching of the Zettelkasten, and cannot predict in advance the twists and turns that your ideas and your reading might take. The constant updating of directory structures and tag ontologies is energy consuming and yields few results.
- Instead of taxonomy, the IRE is based on the principle that the "life" of a note—it's retrievability but also its capacity to elicit new ideas—hinges on the density of cross-references among notes. A dead note is a note with no links braching from it or leading to it. Thus, the IRE is design to ease the establishment of cross-references, through hyperlinks and other techniques.
And instead of cumbersome taxonomies, the IRE favors the creation of ad hoc indexes (lists of notes) and indexes of indexes.

