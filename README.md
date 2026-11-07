# Hrvoje Planinić — academic website starter

This is an editable Quarto website, matching the agreed minimal design. Seven journal articles have been added from individual CroRIS records, with DOI and arXiv links. The student list is still unfinished. Confirm the homepage research description before launch. Add a CV navigation link once the PDF is present.

## Start here

1. Create or use a GitHub account. Create a public repository named hplaninic.github.io.
2. Put the contents of this folder at the repository root, including `.github/workflows/publish.yml`. GitHub Desktop is an option if browser upload misses hidden folders.
3. In repository Settings → Pages, choose GitHub Actions as the publishing source.
4. In Actions, run “Publish website”, or save a change on the main branch. This publishes the site publicly; finish or remove draft messages first if you do not want them visible.
5. Check the deployment result and visit https://hplaninic.github.io/.

The workflow installs a fixed Quarto version and publishes the generated HTML. No local installation is needed for routine text edits on GitHub. All four pages were successfully rendered using Quarto 1.6.43, and local page links were checked. Browser appearance has not yet been checked. The site has not been deployed. A rendered copy is included in `_site/`; open `_site/index.html` to preview locally.

## Routine edits

Use GitHub's file editor to edit a `.qmd` file, then commit the change to main. Publishing runs automatically. QMD files are plain text with Markdown formatting; there is no programming required for normal updates.

| Change | File |
| --- | --- |
| Biography and profile links | index.qmd |
| Publications | research.qmd |
| Course descriptions and download links | teaching.qmd |
| Students and thesis links | students.qmd |
| Navigation | _quarto.yml |
| Appearance | styles.css |

The commented examples in the pages show how to add records. Replace placeholder URLs with real links and remove `<!--` and `-->` around an entry to display it. Upload PDFs to `files/`, then add links in teaching.qmd. Keep the PDF filename unchanged for later versions and update the visible date.

## Optional local preview

Install Quarto (https://quarto.org/docs/get-started/), open this directory in a terminal, then run `quarto preview`. Run `quarto render` to build the static website in `_site/`. You can also upload that folder's contents to university hosting instead of using GitHub Pages.

## University address

After GitHub deployment is working, configure the university homepage to redirect to your actual GitHub Pages URL. Keep existing lecture-note and other file URLs working. A server-side redirect of the homepage alone is preferable where supported; otherwise a small HTML redirect page with a normal fallback link is possible. Ask departmental IT how to update your personal web directory. Do not overwrite the current homepage before keeping a backup.

## Before launch

- Confirm biography, research description, affiliation, and public email.
- Review the imported publication list and add public thesis links.
- Upload lecture notes, indicate their language and update dates.
- Add your CV if desired.
- Verify every link and the appearance on a phone.
- Remove the visible draft messages.

Lecture-note permission is included on the Teaching page. It does not apply to third-party content.
