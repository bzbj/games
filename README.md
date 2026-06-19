# GitHub Pages Publish Package

This folder is ready to publish with GitHub Pages.

Files:
- `index.html`: the playable game.
- `.nojekyll`: tells GitHub Pages not to run Jekyll processing.

## Fastest Way

1. Create a new GitHub repository, for example `china-vc-simulator`.
2. Upload the contents of this folder to the repository root.
3. In GitHub, open `Settings -> Pages`.
4. Set:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/ (root)`
5. Save.

The URL will usually be:

```text
https://<your-github-username>.github.io/china-vc-simulator/
```

## Command Line

From this folder:

```bash
git init
git add index.html .nojekyll README.md
git commit -m "publish vc simulator"
git branch -M main
git remote add origin git@github.com:<your-github-username>/china-vc-simulator.git
git push -u origin main
```

Then enable GitHub Pages in repository settings as described above.

## Updating

When the game changes, copy the new `dist/index.html` into this folder, commit, and push.
