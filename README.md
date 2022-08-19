# UNISA COS1501 Notes

This repo contains the LaTex files needed to compile a set of notes for the course **Theoretical Computer Science** at the University of South Africa.

## Contents
- [Accessing the Notes](#accessing-the-notes)
- [Note](#note)
- [Contributing](#contributing)
- [The Code](#the-code)
  - [The Structure](#the-structure)
  - [Packages Used](#packages-used)

## Accessing the Notes

A PDF can be generated using **latexmk**. If you want to access pregenerated PDFs, please check the **Releases** section on the sidebar.

## Note
This is a work in progress, with chapters and examples to come.  
If you are able, and interested in contributing, please do!  
If there is something missing, or something that you feel needs further clarification, please open an issue.

## Contributing
Please fork this repo, make your changes, and then open a pull request.

## The Code
### The Structure
- The file `notes.tex` contains the general structure and order of the files, including package imports. Building this file should build all the other `.tex` files, and include them in one `.pdf` called `notes.pdf`
- Each unit has a separate `tex` file where the notes are written. These are contained in the `units` folder.

### Packages Used
TeX packages that have been used are:
- [geometry](https://ctan.org/pkg/geometry): Used for document margins
- [amsmath, amssymb](https://www.ctan.org/pkg/amsmath): Used for mathematical symbols and environments
- [amsthm](https://ctan.org/pkg/amsthm): Used for the proof and theorem environments
- [enumitem](https://ctan.org/pkg/enumitem): Used to improve the way lists are displayed
- [xcolor](https://ctan.org/pkg/xcolor): used to get more colors
- [hyperref](https://ctan.org/pkg/hyperref): Add PDF bookmarks
- [babel](https://ctan.org/pkg/babel): Use description environment, and chapter renaming
- [fontenc](https://ctan.org/pkg/fontenc), [charter](https://ctan.org/pkg/charter), [inconsolata](https://ctan.org/pkg/inconsolata), [cabin](https://ctan.org/pkg/cabin), [newtxmath](https://ctan.org/pkg/newtx), [bm](https://ctan.org/pkg/bm): Font display
- [tikz](https://ctan.org/pkg/tikz): Used for images
- [venndiagram](https://ctan.org/pkg/venndiagram): Easier support for Venn Diagram display than using pure tikz
- [etoolbox](https://ctan.org/pkg/etoolbox): Allow commands to be patched
- [mathtools](https://ctan.org/pkg/mathtools): For bold math and other math display, related to [amsmath](https://www.ctan.org/pkg/amsmath)
- [tcolorbox](https://ctan.org/pkg/tcolorbox), [adjustbox](https://ctan.org/pkg/adjustbox): Create colored boxes for different environments
- [changepage](https://ctan.org/pkg/changepage): Allow paragraphs to be indented
- [fancyhdr](https://ctan.org/pkg/fancyhdr): Improve header and footer display
- [subfiles](https://ctan.org/pkg/subfiles): Allow `tex` files to be written separately, but built together


