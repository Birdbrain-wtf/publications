---
id: seeds-protocol-specification
slug: seeds-protocol-specification
title: "Seeds: Protocol Specification"
summary: The technical specification. The one application pallet of the Seeds reference runtime, as definitions, invariants and algorithms, with a 28-check run on a three-node network and what is not yet built.
authors:
  - Birdbrain
published: 2026-10-05
updated: 2026-10-05
tags:
  - seeds
  - identity
  - membership
  - attribution
status: published
publicationType: technical-specification
edition: 3.1.0
license: CC-BY-4.0
---

# Seeds: Protocol Specification

**Read it:** [paper.pdf](paper.pdf) · source [paper.tex](paper.tex) · companion: [the white paper](../seeds-a-store-of-values/)

## Abstract

Seeds is a chain that records who joined a community, what they put forward and which of it stood. A member is admitted when enough existing members witness them against the same session evidence. A contribution is a digest that matures unless enough members challenge it. Units are minted when a contribution matures and nowhere else: joining mints nothing, there is no bond and units do not move between members. The runtime is five pallets: four from a standard Substrate solo chain and one application pallet of about a thousand lines. It has no balances pallet, no fees, no sudo and no treasury. This paper specifies that pallet as definitions, invariants and algorithms. It reports a run of twenty-eight checks on a three-node network, derives from the constants what a colluding set of members can do, and lists what is not built. The argument for the design is in the companion white paper.

## Code

The reference runtime is at [github.com/Birdbrain-wtf/seeds](https://github.com/Birdbrain-wtf/seeds/tree/main/chain). The same rules run as JAM services on [Jambo](https://github.com/Birdbrain-wtf/jambo).

## Building the PDF

The source is LaTeX. With a TeX Live install:

```
lualatex paper.tex && bibtex paper && lualatex paper.tex && lualatex paper.tex
```

`seeds.bib` and `seeds-academic.sty` are shared by both Seeds papers and are copied into each folder so either builds on its own.
