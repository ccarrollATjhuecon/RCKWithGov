# The Ramsey/Cass-Koopmans (RCK) Model with Government

A handout for JHU Econ 180.603 (Intertemporal Choice): government spending paid for by lump-sum taxes, permanent
and temporary increases in spending, debt and Ricardian equivalence, and a tax on capital income, in the
decentralized RCK economy.

- **The source is the book's chapter,** [The Ramsey/Cass-Koopmans (RCK) Model with Government](https://intertemporal-choice.github.io/content/growth/rckwithgov/)
  (`content/growth/RCKWithGov/index.md` in
  [intertemporal-choice.github.io](https://github.com/intertemporal-choice/intertemporal-choice.github.io)).
  Edits start there and are carried into `RCKWithGov.tex`.
- **The notebook** `RCKWithGov.ipynb` is an own copy of the book's, which draws both figures (`Figures/`). Run
  it in Colab or Binder from this repo (the links are in the handout), or in the browser from the book's JupyterLite.
- **Build:** `latexmk` (the `latexmkrc` points TeX at the vendored registry in `@resources/`, econ-ark-tools
  02e344d5, notation v14.1.0, read-only).
- **Check against the book:** `./check-book-sync.py` (the book's main on GitHub), or
  `./check-book-sync.py --book-git <clone> --ref <commit>` for an unpushed book commit. It compares the words,
  the notes (a `\marginFootnote` here is a margin note in the book), the links, the citations, the printed
  symbols, the figures and the notebook, and checks rule D: every object written with its macro.
- `@local/RCKWithGov.sty` defines no notation. Since c931a72 (registry v14.1.0) the registry has every object this
  handout writes, government spending `\GovSpend`, the lump-sum tax `\TaxLev`, government debt `\Debt`, the
  Hamiltonian `\Ham` and the costate `\vk` among them.
- `RCKWithGov.bib` holds the entries the handout cites, copied verbatim from texmf-local's `economics.bib`; the
  empty `system.bib` keeps the build to them.

Revived on 2026-11-17 from the 2021 handout (the first commit holds it as found, including `LaTeX/`).
