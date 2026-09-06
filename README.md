# heibench.github.io

The heibench org site, served at [heibench.com](https://heibench.com).

Plain HTML and CSS. No build step, no dependencies, no JavaScript — `git push`
is the deploy.

    index.html            what the org is, and the two layers
    silence.html          the core rule, and the recorded instances of the defect
    adjudications.html    open conflicts between shipped members
    assets/site.css       the whole stylesheet
    assets/mark.svg       the org mark; generated in the .github repo

## What is canonical here

The contract itself lives in
[`.github/AGENTS.md`](https://github.com/heibench/.github/blob/main/AGENTS.md).
This site is canonical for the **evidence** behind it — the defect record and
the adjudications — so that each fact lives in exactly one place.

Adding a case to the record means adding it here, not to `AGENTS.md`.

## Local preview

    python3 -m http.server 8000

Then open <http://localhost:8000>. The pages use root-relative paths, so
opening the files directly over `file://` will not load the stylesheet.
