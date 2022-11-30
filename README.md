# UNISA COS1501 Notes

This repo contains the LaTeX files needed to compile a set of notes for the course **Theoretical Computer Science** at the University of South Africa.

## Contents
- [Accessing the Notes](#accessing-the-notes)
- [Note](#note)
- [Contributing](#contributing)
- [The Code](#the-code)
  - [The Structure](#the-structure)
  - [Packages Used](#packages-used)
  - [Commands Added](#commands-added)
    - [Commands](#commands)
    - [Environments](#environments)

## Accessing the Notes

A PDF can be generated using [latexmk](https://ctan.org/pkg/latexmk). If you want to access pre-generated PDFs, please check the [Releases](https://github.com/Unisa-Notes/COS1501/releases) section on the sidebar.

## Note
This is a work in progress, with chapters and examples to come.  
If you are able, and interested in contributing, please do!  
If there is something missing, or something that you feel needs further clarification, please open an issue.

## Contributing
Please fork this repo, make your changes, and then open a pull request.

## The Code
### The Structure
- The file [notes.tex](notes.tex) contains the general structure and order of the files. Building this file should build all the other `.tex` files, and include them in one `.pdf` called `notes.pdf`
- Each unit has a separate `tex` file where the notes are written. These are contained in the [units](./units) folder.
- The styles, commands and packages used are in the package file [notestyles.sty](notestyles.sty)

### Packages Used
TeX packages that have been used are:
- [amsmath, amssymb](https://www.ctan.org/pkg/amsmath): Used for mathematical symbols and environments
- [amsthm](https://ctan.org/pkg/amsthm): Used for the proof environment\
- [babel](https://ctan.org/pkg/babel): Use description environment, and chapter renaming
- [changepage](https://ctan.org/pkg/changepage): Allow paragraphs to be indented
- [enumitem](https://ctan.org/pkg/enumitem): Used to improve the way lists are displayed
- [etoolbox](https://ctan.org/pkg/etoolbox): Allow commands to be patched
- [fancyhdr](https://ctan.org/pkg/fancyhdr): Improve header and footer display
- [fontenc](https://ctan.org/pkg/fontenc), [charter](https://ctan.org/pkg/charter), [inconsolata](https://ctan.org/pkg/inconsolata), [cabin](https://ctan.org/pkg/cabin), [newtxmath](https://ctan.org/pkg/newtx), [bm](https://ctan.org/pkg/bm): Font display
- [geometry](https://ctan.org/pkg/geometry): Used for document margins
- [hyperref](https://ctan.org/pkg/hyperref): Add PDF bookmarks
- [parskip](https://ctan.org/pkg/parskip): Set proper default values for paragraph separation
- [subfiles](https://ctan.org/pkg/subfiles): Allow `tex` files to be written separately, but built together
- [tabularray](https://ctan.org/pkg/tabularray): Better table display and management.
  * Also uses libraries to simulate [booktabs](https://ctan.org/pkg/booktabs) and [varwidth](https://ctan.org/pkg/varwidth)
- [tcolorbox](https://ctan.org/pkg/tcolorbox), [adjustbox](https://ctan.org/pkg/adjustbox): Create colored boxes for different environments
- [tikz](https://ctan.org/pkg/tikz): Used for images
- [venndiagram](https://ctan.org/pkg/venndiagram): Easier support for Venn Diagram display than using pure tikz
- [xargs](https://ctan.org/pkg/xargs): Allow commands and environments to have more than one optional argument
- [xcolor](https://ctan.org/pkg/xcolor): Used to get more colors
- [xstring](https://ctan.org/pkg/xstring): Analyze strings given as arguments to an environment


### Commands Added
For intellisense, a list of the commands is added in the [package_intellisense](./package_intellisense/) folder. These have been written in formats that can be understood by different LaTeX tools.

#### Commands
- `addfile [input] {<filename>}`: Include or input the file into the document. By default, it includes the file, the option `input` can be given to input it instead.
- `concept {text}`: Mark specific text as a concept to be learned. Puts the text in bold.
- `rulebookend`: Insert a decorative horizontal line at the end of the text.
- `rulechapterend`: Insert a decorative horizontal line at the end of each unit.

#### Environments
- `definition {title}`: Coloured box used for highlighting important concepts.
- `example`: Coloured box used to highlight examples.
- `exercise {title}`: Coloured box used to highlight exercises.
- `indentparagraph`: Indent selected text to the left.
- `sidenote`: Coloured box used to indicate extra information.
- `subproof`: Environment for proofs inside proofs.
- `theorem`: Coloured box used to highlight theorems.
- `venntwo` and `vennthree [options] [title]`: Simplified Venn Diagram environments
