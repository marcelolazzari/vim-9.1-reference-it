# vim-9.1-reference-it

Guida pratica a Vim 9.1 — riferimento completo in Italiano.

Questo repository contiene:
- `vim-9.1-reference-it.md` — guida pratica e molto completa per Vim 9.1 (IT).
- `vim-cheatsheet-it.md` — cheat-sheet una pagina.
- `.github/workflows/build-pdf.yml` — workflow GitHub Actions per costruire i PDF automaticamente.

Come generare i PDF localmente:
- Prerequisiti: pandoc, una distribuzione LaTeX (es. texlive).
- Esempio:
  pandoc vim-9.1-reference-it.md -o "Vim-9.1-Reference-IT.pdf" --pdf-engine=xelatex -V geometry:margin=1in -V mainfont="DejaVu Sans Mono" --highlight-style=tango

Licenza: MIT (vedi file LICENSE)
