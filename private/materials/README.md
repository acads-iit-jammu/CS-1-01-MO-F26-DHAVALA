# materials/ — teacher-side workspace

Mirror of the public `../../materials/` folder. Interactive artifacts (HTML),
handouts, and other student-facing files are **developed and iterated here**
(with Claude), reviewed by the instructor, and only then copied to the public
side.

## Graduation workflow

1. Develop/iterate the file here until happy (e.g., `w01-toy-computer.html`).
2. Copy it over: `cp w01-toy-computer.html ../../materials/`
3. Add a row to `../../materials/index.qmd` and link it from the relevant
   week page / lab sheet.
4. From the repo root: `quarto render && git add -A && git commit && git push
   && quarto publish gh-pages --no-prompt`

Drafts, rejected versions, and instructor-only variants (e.g., versions with
answers visible) stay here permanently.

## Naming convention

Artifacts are named `wNN-<name>.html` — the week they belong to, then the name
(e.g., `w01-turtle-computer.html`). Same name on both private and public sides.
