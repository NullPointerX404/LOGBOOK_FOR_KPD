# LOGBOOK_FOR_KPD

## How to generate PDF log book

---

### For macOS

1. **Download Pandoc**  
   Go to [macOS download pandoc](https://github.com/jgm/pandoc/releases/download/3.8.3/pandoc-3.8.3-x86_64-macOS.pkg) and install Pandoc.

2. **Verify installation**  
   ```bash
   pandoc --version
   ```

---

#### Alternative method (Homebrew)

1. **Install Homebrew** (if you don't have it):  
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. **Install Pandoc**  
   ```bash
   brew install pandoc
   ```

3. **Verify installation**  
   ```bash
   pandoc --version
   ```

4. **Install a PDF engine**  
   ```bash
   brew install mactex
   brew install wkhtmltopdf
   ```

---

#### Example usage

```bash
pandoc myfile.md -o myfile.pdf       # markdown -> pdf
pandoc myfile.md -o myfile.docx      # markdown -> word
pandoc --from=latex --to=docx -o output.docx input.tex   # latex -> word
```

---

### For Windows

1. **Download Pandoc**  
   Go to [Windows download pandoc](https://github.com/jgm/pandoc/releases/download/3.8.3/pandoc-3.8.3-windows-x86_64.msi) and install Pandoc.

2. **Download a PDF engine** (choose one):  
   - [MiKTeX](https://miktex.org/download)  
   - [TeX Live](https://www.tug.org/texlive/)

3. **Verify installation**  
   ```bash
   pandoc --version
   ```

---

#### Example usage

```bash
pandoc myfile.md -o myfile.pdf
pandoc myfile.md -o myfile.docx
pandoc myfile.docx -o myfile.md
```
```

---

