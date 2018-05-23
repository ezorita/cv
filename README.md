# Eduard Valera i Zorita
This is my CV. Feel free to [download in PDF](cv_ezorita.pdf).

## Using Friggeri template
This template has been adapted from Friggeri's CV template.

### **Requirements** (other combinations may also work):
- XeLaTeX (XeTeX 3.14+)
- biblatex 3.3
- biber 2.4

### How to compile
First, clone the repo and try to compile using:
```
xelatex cv_ezorita.tex
biber cv_ezorita
xelatex cv_ezorita.tex
```
This should generate an output file `cv_ezorita.pdf` with the correct format and bibliography.

### It does not work!
If that didn't work, try the following:
- Install XeTeX: `sudo apt-get install texlive-xetex`
- Manually install biblatex 3.3:  https://sourceforge.net/projects/biblatex/files/biblatex-3.3/
- Manually install biber 2.4: https://sourceforge.net/projects/biblatex-biber/files/biblatex-biber/2.4/

#### To manually install LaTeX packages (applies to biblatex):
- Download the package from https://sourceforge.net/projects/biblatex/files/biblatex-3.3/
- Copy the folder structure to your texlive path (/usr/share/texlive/texmf-dist/ in Ubuntu 14.04).
- Run `sudo texhash` to update the library.

#### Installing biber:
- Download and extract the biber binary.
- Replace the old biber binary with this one (if you had a previous version): `sudo cp biber $(which biber)`
- If you had no previous `biber` binary, just: `sudo cp biber /usr/bin/`

#### Installing the fonts:
- Extract the file `fonts.tar.gz` in `~/.fonts/`.
- Run `sudo fc-cache -fv`.
