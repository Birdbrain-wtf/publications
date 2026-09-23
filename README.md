# Birdbrain publications

The canonical, version-controlled source for Birdbrain's long-form publications: position papers, RFCs and responses in governance discussions.

## Reading and citing

Each article lives at `content/articles/{slug}/index.md`, with its changelog alongside. A branch URL points to the current edition. For a citation that will not change, replace the branch in a GitHub `blob` or `raw` URL with the full commit SHA of the edition you mean.

Published editions are also tagged:

```text
publication/{slug}/v{major}.{minor}.{patch}
```

## Revising

A revision updates the article at its existing path, adds a changelog entry and gets a new tag. Published history is never rewritten, so every earlier commit-SHA link keeps pointing at the edition it cited.

## Licence

Text is CC-BY-4.0 unless an article says otherwise. Data files under an article's `data/` folder are published so the figures can be checked.

This layout follows [sdfinst/publications](https://github.com/sdfinst/publications), whose approach to versioned position papers we found worth copying.
