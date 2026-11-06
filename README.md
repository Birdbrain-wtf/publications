# Birdbrain publications

The canonical, version-controlled source for Birdbrain's long-form publications: position papers, RFCs and responses in governance discussions.

## Contents

### Seeds

| Paper | Type | Edition | Status |
| --- | --- | --- | --- |
| [Seeds: A Store of Values](content/articles/seeds-a-store-of-values/) | white paper | 3.3.0 | published |
| [Seeds: Protocol Specification](content/articles/seeds-protocol-specification/) | technical specification | 3.3.0 | published |

### Kusama's future

| Paper | Type | Edition | Status |
| --- | --- | --- | --- |
| [An Independent Kusama: a counter-proposal](content/articles/independent-kusama/) | position paper | 0.2.0 | published |
| [The Game That Decides Kusama](content/articles/kusama-economic-game/) | research note | 0.1.0 | published |
| [An independent Kusama on a reduced JAM: the fifth option](content/articles/independent-kusama-fifth-option/) | position paper | 1.0.2 | published |

### Other

| Paper | Type | Edition | Status |
| --- | --- | --- | --- |
| [The Changing Shape of Polkadot](content/articles/polkadot-changing-shape/) | review | 0.1.0 | draft |
| [Pala: a specification of the society in Huxley's Island](content/articles/pala-a-specification/) | reference | 0.2.0 | draft |

### Moved

| Old path | Now |
| --- | --- |
| [seeds-a-chain-with-one-job](content/articles/seeds-a-chain-with-one-job/) | [Seeds: Protocol Specification](content/articles/seeds-protocol-specification/), from 3.1.0. The 3.0.0 tag keeps the old name. |

Papers are grouped by the `series` field in their front matter, not by folder, so a paper's path never changes when a series grows. A moved paper keeps a stub at its old path with `status: moved`.

## Reading and citing

Each article lives at `content/articles/{slug}/index.md`, with its changelog alongside. A branch URL points to the current edition. For a citation that will not change, replace the branch in a GitHub `blob` or `raw` URL with the full commit SHA of the edition you mean.

Published editions are also tagged:

```text
publication/{slug}/v{major}.{minor}.{patch}
```

## Revising

A revision updates the article at its existing path, adds a changelog entry and gets a new tag. Adding a front-matter field such as `series` does not change the text and is not a new edition. A revision also updates its row in the contents above. Published history is never rewritten, so every earlier commit-SHA link keeps pointing at the edition it cited.

## Licence

Text is CC-BY-4.0 unless an article says otherwise. Data files under an article's `data/` folder are published so the figures can be checked.

This layout follows [sdfinst/publications](https://github.com/sdfinst/publications), whose approach to versioned position papers we found worth copying.
