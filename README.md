# run-it-app.github.io

Web pages for **Run It**:

- `/`: the landing page (invite only, so no links to the app).
- `/privacy/`: the privacy policy, linked from the Intervals.icu OAuth app.
- `/w/#…`: opens a shared workout. The workout is in the URL fragment, which never reaches the server.
- `/app/`: the iPhone web app.
  - It's built in the app repo with `scripts/build-web.sh` and copied from `dist/web/`.
  - `404.html` sends reloads of its inner pages back to it.
  - It's kept out of search engines.
- `.nojekyll`: so Pages serves `_expo/` as it is.
