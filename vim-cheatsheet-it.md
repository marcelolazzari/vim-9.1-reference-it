VIM 9.1 — Cheat-sheet (IT) — una pagina

Modalità:
- N: Normal, I: Insert, V: Visual, : Ex

Movimenti:
- h j k l
- 0 ^ $ - inizio / primo non-blank / fine riga
- w e b / W E B - parole
- gg / G - inizio / fine file
- % - matching parentesi
- f<char> / t<char> / F / T

Editing:
- dw / dd / d$ / d0
- cw / cc / c$
- yw / yy / y$
- p / P
- . ripeti ultimo comando di modifica
- u undo / <C-r> redo

Selezione:
- v - visual char
- V - visual line
- <C-v> - visual block

Macro / Registri:
- qa ... q — registra in a
- @a — esegui macro a
- "ayw — yank in registro a
- "0p — incolla ultimo yank

Ricerca & sostituzione:
- /pattern <CR> ; n / N
- :%s/old/new/gc
- :g/pat/d  (cancella righe matching)

File / Buffer / Window:
- :e file
- :w / :wq / :x
- :bn / :bp / :bd
- :sp / :vsp / <C-w> h/j/k/l

Set utili:
- :set number
- :set relativenumber
- :set expandtab
- :set tabstop=4 shiftwidth=4
- :set ignorecase smartcase
- :set mouse=a
- :set termguicolors

Tastiera italiana (note rapide):
- : = Shift + .
- / = Shift + 7
- @ = AltGr + ò
- \ | { } ~ ^ possono richiedere AltGr o combinazioni
- Consiglio: let mapleader="," nel vimrc

Comandi rapidi:
- :help <topic>
- :mksession! session.vim
- :w !sudo tee % >/dev/null  (Linux/macOS per salvare come root)
- :!make && :copen  (build + apri quickfix)

Esempi frequenti:
- Rimuovere trailing spaces: :%s/\s\+$//e
- Convertire tabs in spazi: :retab
- Yank riga corrente in clipboard: "+yy
- Commenta blocco (visual): <C-v>jjI// <Esc>

Leader tipico:
- let mapleader=","   (metti nel tuo ~/.vimrc)
- nnoremap <leader>w :w<CR>

Per maggiori dettagli: apri il documento completo o digita :help in Vim
