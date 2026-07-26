# notebooks/ — teacher-side workspace

Mirror of the public `../../notebooks/` folder. Notebooks are **developed and
iterated here** (with Claude), run end-to-end, reviewed, and only then copied
to the public side.

## Graduation workflow

1. Develop the notebook here until happy; restart-and-run-all before release.
2. Strip anything instructor-only (solutions, grading notes) — keep those in a
   `-solutions` copy that stays here.
3. Copy it over: `cp foo.ipynb ../../notebooks/`
4. Add a row to `../../notebooks/index.qmd`. To give it its own rendered page
   in the site sidebar, also list it as a chapter in `../../_quarto.yml`
   (books only render listed chapters); otherwise it is served as a raw
   downloadable file.
5. From the repo root: `quarto render && git add -A && git commit && git push
   && quarto publish gh-pages --no-prompt`
