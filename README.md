# run-it-app.github.io

Web pages for **Run It**:

- `/`: the landing page (invite only, so no links to the app).
- `/privacy/`: the privacy policy, linked from the Intervals.icu OAuth app.
- `/w/#…`: opens a shared workout. The workout is in the URL fragment, which never reaches the server.
- `/start/`: the quick start guide for invitees, with a printable PDF (`run-it-quick-start.pdf`). It's printed from the same page and kept out of search engines. The source is `marketing/guide/` in the app repo.
- `/app/`: the iPhone web app.
  - It's built in the app repo with `scripts/build-web.sh` and copied from `dist/web/`.
  - `404.html` sends reloads of its inner pages back to it.
  - It's kept out of search engines.
- `.nojekyll`: so Pages serves `_expo/` as it is.
