# Monitor guidelines for danysbees

These add to the factory monitor guidelines.

- The live site is https://danysbees.com, served by GitHub Pages.
- The deploy is the "Deploy to GitHub Pages" workflow, which runs on every push to `main`. Wait for it with `gh run list --workflow deploy.yml --limit 3` and `gh run watch`.
- Check every changed page in all three languages: `https://danysbees.com/en/…`, `/fr/…` and `/ar/…`, at laptop and mobile size.
- GitHub Pages can take a few minutes to serve the new version after the workflow finishes. Reload with a cache-busting query, for example `?v=<commit>`, before calling it not live.
