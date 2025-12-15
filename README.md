# LOGBOOK_FOR_KPD

how to generate pdf log book

for macos:go to <a href="https://github.com/jgm/pandoc/releases/download/3.8.3/pandoc-3.8.3-x86_64-macOS.pkg">macos download pandoc</a>
and install pandoc

Verify installation:
pandoc --version

or

2 

install homebrew(if you don't have homebrew)
type this in terminal
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

Install Pandoc
brew install pandoc

Verify installation:
pandoc --version

Install a pdf engine:
brew install mactex
brew install wkhtmltopdf

Example usage:
pandoc myfile.md -o myfile.pdf (markdown->pdf)
pandoc myfile.md -o myfile.docx (markdown->word)
pandoc --from=latex --to=docx -o output.docx input.tex (latex->word)


for window:

go to <a href="https://github.com/jgm/pandoc/releases/download/3.8.3/pandoc-3.8.3-windows-x86_64.msi">window download pandoc</a>
and install pandoc

download pdf engine (choose 1 from 2 pdf engine)
<a href="https://miktex.org/download">miktex</a>
<a href="https://www.tug.org/texlive/">TeX Live</a>

Verify installation:
pandoc --version


pandoc myfile.md -o myfile.pdf
pandoc myfile.md -o myfile.docx
pandoc myfile.docx -o myfile.md

