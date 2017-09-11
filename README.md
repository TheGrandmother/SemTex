# SemTex
A halfassed Latex package for language semantics.

Only people taking the semantics course at the It department at Uppsala University will have any use for this.
This has no other purpose.

## Installation instructions
You may either just place the `.sty` files directly in your LaTeX project or install them locally. The latter is the preferred method of installation but requires a bit more work.

A minimal example would be
```latex
\documentclass{article}

\usepackage{while}
\usepackage{semtex}

\begin{document}
In natural semantics, $\AxiomNs{S}{s}{s'}$ holds if there is a derivation tree with it as its root.
\end{document}
```

To install locally, locate the `TEXMFHOME` directory by executing
```
kpsewhich -var-value=TEXMFHOME
```
You should get something like `~/texmf` back.

Create it if it doesn't exist. Then, create the subdirectories `~/texmf/tex/latex` in it and clone the repository there. You should have something like `~/texmf/tex/latex/SemTex`.

That's it!

You may test it by checking that TeX finds the files:
```
kpsewhich while.sty
kpsewhich semtex.sty
```
