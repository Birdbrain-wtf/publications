---
id: seeds-a-store-of-values
slug: seeds-a-store-of-values
title: "Seeds: A Store of Values"
summary: The white paper. Identity grown from witnessed participation instead of issued by an institution, a record of what each member added, and new units created only when a contribution stands.
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
publicationType: white-paper
edition: 3.1.0
license: CC-BY-4.0
---

# Seeds: A Store of Values

**Read it:** [paper.pdf](paper.pdf) · source [paper.tex](paper.tex) · companion: [the technical specification](../seeds-protocol-specification/)

## Abstract

Online, a person is either an account that an institution issued or a key that they hold. An account can be closed by whoever issued it, and a key proves only that someone holds it. Neither records what a person has done or who will stand behind them. We propose identity that is grown, not issued. A person arrives by signing in to a meeting their group already holds. The sign-ins become a public attendance record, and a person who keeps turning up alongside the same members becomes a member without anyone filling anything in. The people who were there need act only when the record is wrong. What a member contributes is recorded against them, and it stands unless three members challenge it. Joining brings a vote and no units. New units of the network's record are created only when a contribution stands, so what a member holds is what they have added. There is no treasury, no fee and no administrator. Members write for free, change the rules by one member, one vote, and run the machines that keep the record. A test network has run these rules, and every unit of its supply traced to one of them.

## Code

The reference runtime is at [github.com/Birdbrain-wtf/seeds](https://github.com/Birdbrain-wtf/seeds/tree/main/chain). The same rules run as JAM services on [Jambo](https://github.com/Birdbrain-wtf/jambo).

## Building the PDF

The source is LaTeX. With a TeX Live install:

```
lualatex paper.tex && bibtex paper && lualatex paper.tex && lualatex paper.tex
```

`seeds.bib` and `seeds-academic.sty` are shared by both Seeds papers and are copied into each folder so either builds on its own.
