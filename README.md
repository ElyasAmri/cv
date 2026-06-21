# Elyas Al-Amri — CV & Personal Statements

LaTeX sources for my curriculum vitae, tailored CV variants, and graduate
application personal statements.

## Repository layout

```
cv.tex                      Main CV (primary document)
variants/
  cv-no-qeeri.tex           CV variant without QEERI/QCRI research roles
  engineer-resume.tex       One-page engineering resume
personal-statements/
  ps.md                     Personal statement (draft, Markdown)
  ps-dse.tex                Statement — Data Science & Engineering
  ps-icsd.tex               Statement — Information & Computing Science
.claude/                    Editor build hooks (latexmk on save)
```

`examples/` (reference templates) and `archive/` (previous versions) are kept
locally but excluded from version control.

## Building

Each `.tex` file is a standalone document. Compile with `latexmk`:

```sh
latexmk -pdf cv.tex
latexmk -pdf variants/engineer-resume.tex
```

Requires a TeX distribution (TeX Live / MiKTeX) with the `fontawesome`,
`titlesec`, `enumitem`, and `hyperref` packages.

## Remotes

This repository is mirrored on Overleaf (`origin`) and GitHub (`github`).
