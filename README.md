# SemTex
A halfassed Latex package for language semantics.

Only people taking the semantics course at the It department at Uppsala University will have any use for this.
This has no other purpose.

## Installation instructions
First, locate the `TEXMFHOME` directory by executing
```
kpsewhich -var-value=TEXMFHOME
```
You should get something like `~/texmf` back.

Create it if it doesn't exist. Then, create the subdirectories `~/texmf/tex/latex` in it and clone the repository there. You should have something like `~/texmf/tex/latex/SemTex`.

That's it! Now `\usepackage{semtex, while}` works like you would expect.

You may test it by checking that TeX finds the files:
```
kpsewhich while.sty
kpsewhich semtex.sty
```
