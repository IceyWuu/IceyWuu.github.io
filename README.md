# Yubing Wu's Personal Homepage

Personal academic homepage of **Yubing Wu (吴钰冰)**, deployed via GitHub Pages at <https://iceywuu.github.io>.

Built on the open-source [AcadHomepage](https://github.com/RayeRen/acad-homepage.github.io) Jekyll theme (MIT License), styled after [Wei Chen's homepage](https://hoemr.github.io).

## Editing content

Nearly all page content lives in one file: [`_pages/about.md`](_pages/about.md) — About, News, Publications, Ongoing Research, Honors, Education, Internships. Publication entries support one-click BibTeX copy: add the entry HTML in `about.md` and add the corresponding key to the `bibData` object in the `<script>` at the bottom of the file.

Site-wide settings (name, avatar, email, GitHub, site description, navigation menu) are in:

- [`_config.yml`](_config.yml) — site title, author profile (sidebar), email, social links
- [`_data/navigation.yml`](_data/navigation.yml) — top navigation menu

Profile photo: `images/yubing.jpg`. Favicon / touch icon are generated from it (`images/favicon-32.png`, `images/apple-touch-icon.png`).

## Run locally

Requires Ruby and Bundler.

```bash
bundle install
bundle exec jekyll liveserve   # or: bundle exec jekyll serve
```

Then open <http://127.0.0.1:4000>.

## Deploy

Push to `main` — GitHub Pages builds the Jekyll site automatically (the `github-pages` gem in the `Gemfile` pins the supported version). No extra workflow needed.

## Notes

- The Google Scholar citation crawler and visitor counter from the original template were removed. If you want automatic Scholar stats back, see the upstream README and set `GOOGLE_SCHOLAR_ID`.
- License: MIT (see [LICENSE](LICENSE), © 2022 Yi Ren for the original theme).
