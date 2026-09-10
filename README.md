# *Vojtěch Krupička's* curriculum vitae

The source and generated outputs for **Vojtěch Krupička's** curriculum vitae.

One YAML file holds all the content. A Jinja‑templated LaTeX file turns it into a
typeset PDF, and a Markdown version is generated from the same data — so the CV
only ever has to be edited in one place.

## Contents

| File | Role |
| --- | --- |
| [`vojtech-krupicka-cv.yaml`](vojtech-krupicka-cv.yaml) | **Single source of truth** — personal details, summary, experience, projects, skills, education, languages, hobbies. |
| [`hassas-resume.tex.jinja`](hassas-resume.tex.jinja) | LaTeX template (Jinja2), based on *Jake's Resume* (MIT). Uses LaTeX‑safe delimiters: `(( … ))` for variables, `((* … *))` for blocks. |
| [`vojtech-krupicka-cv.tex`](vojtech-krupicka-cv.tex) | Generated LaTeX — the template rendered with the YAML data. |
| [`vojtech-krupicka-cv.pdf`](vojtech-krupicka-cv.pdf) | Generated PDF — the final, ATS‑parsable CV. |
| [`vojtech-krupicka-cv.md`](vojtech-krupicka-cv.md) | Generated Markdown — a plain‑text version of the same content. |
| [`.gitignore`](.gitignore) | Standard LaTeX build artifacts (`*.aux`, `*.log`, …). |

The `.tex`, `.pdf`, and `.md` files are build outputs but are committed so the
current CV can be read and downloaded straight from the repo.

## How it's built

The generator lives in a separate repo,
[`py-make-my-cv`](https://github.com/vojtech-krupicka/py-make-my-cv), which
provides `make_cv.py` and runs inside Docker (so no local LaTeX or Python
toolchain is needed). It:

1. loads `vojtech-krupicka-cv.yaml`,
2. renders `hassas-resume.tex.jinja` → `vojtech-krupicka-cv.tex`,
3. compiles the `.tex` to `vojtech-krupicka-cv.pdf` with `pdflatex`,
4. renders the same data to `vojtech-krupicka-cv.md`.

See that repo's README for the exact command and Docker invocation.

## Editing the CV

1. Edit [`vojtech-krupicka-cv.yaml`](vojtech-krupicka-cv.yaml) only.
   - LaTeX special characters must be escaped (`\&`, `\#`, `\%`, `$…$`, …) — the
     same string is fed to both LaTeX and Markdown.
2. Re‑run `make_cv.py` (see above) to regenerate the `.tex`, `.pdf`, and `.md`.
3. Commit the updated YAML together with the regenerated outputs.

## Credits

- LaTeX template adapted from [Jake's Resume](https://github.com/jakegut/resume) (MIT License).
