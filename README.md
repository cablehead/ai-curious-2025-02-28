## Installation

Install rym using eget:

```bash
eget KmolYuan/reveal-yaml-rs
```

## Development

To work on the slides locally:

```bash
rym serve . --no-open
```

This will start a local development server where you can preview your changes.

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

https://cablehead.github.io/ai-curious-2025-02-28/
