## to update `gh-pages`

After changes on `main`:

1. Build the slides:

```bash
rym pack . ; cp *.png package ; git add package ; git commit -m "build slides" ; git push
```

2. Update `gh-pages`:

```bash
git push origin $"(git subtree split --prefix package main):gh-pages" --force
```

Slides will [update shortly](https://github.com/cablehead/ai-curious-2025-02-28/actions) at:

`https://<username>.github.io/<repo-name>/`
