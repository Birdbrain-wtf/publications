---
id: independent-kusama
slug: independent-kusama
title: "An Independent Kusama: a counter-proposal"
summary: A position paper proposing that Kusama become the network where groups of people grow their collective intelligence, funded from what Kusama already has, with security sized to demand and checkpoints that say when to reopen cohabitation.
authors:
  - Birdbrain
published: 2026-09-23
updated: 2026-09-23
tags:
  - kusama
  - governance
  - tokenomics
  - treasury
  - jam
status: published
publicationType: position-paper
edition: 0.1.0
license: CC-BY-4.0
responds_to: https://github.com/sdfinst/publications/blob/a445bba7ab5a801e3b85168551dfa8b1e5021bc2/content/articles/proposal-kusama-future-jam-prime/index.md
---
# An Independent Kusama: a counter-proposal

**A position paper proposing that Kusama become the network where groups of people grow their collective intelligence, funded from what Kusama already has rather than by paying Polkadot.**

*23 September 2026, by [Birdbrain](https://birdbrain.wtf), a collective on Kreivo.*

**Status and purpose.** This paper responds to *[A Proposal for a Kusama Future on JAM Prime](https://github.com/sdfinst/publications/blob/a445bba7ab5a801e3b85168551dfa8b1e5021bc2/content/articles/proposal-kusama-future-jam-prime/index.md)* (Emiel Sebastiaan and Arief Ernst, SDFI BV, 17 September 2026), read at revision a445bba, and is offered into the same discussion window, which closes on 16 October 2026. It proposes a direction for KSM DAO to weigh against JAM Prime. Appendix A sets out every figure and where it was read. Funding, implementation and any change to issuance or the validator set need their own referenda.

**Disclosures.** We are a collective on Kreivo, one of Kusama's 12 non-system parachains, and §5.4 of the JAM Prime paper prices our chain out. We hold KSM and buy more of it to pay for members. Several of the mechanisms cited here (the onboarding subsidy in RFC-001, the metered query service, the Kreivo memberships) are ones we built or use, and we say which are live and which are proposed as we go. AI tools were used to assist with research, drafting and editing. We take full responsibility for the arguments and figures.

## Abstract

Kusama should be the network where groups of people grow their collective intelligence and own what it is made of: their membership, their record, the permission over it, their treasury and their rules.

**We propose keeping the direction KSM DAO already voted for in [#573](https://kusama.subsquare.io/referenda/573), a light and independent JAM, and funding it from what Kusama already has rather than by paying Polkadot.** Right-size security to demand. Give staked KSM a job on Kusama's own validator set. Stop selling the treasury and spend its surplus on members. Build the route from real revenue to the security budget during the runway, and measure it. If it fails the measures, KSM DAO goes to DOT DAO later with numbers rather than with a request.

## What Kusama is for

The JAM Prime paper lists candidate visions in §4.7: privacy-preserving KSM, a ksmUSD stablecoin, private governance and personhood credentials. Each is useful. None of them says who Kusama is for, so together they read as a feature list, and a feature list cannot tell the DAO what to fund first or what to turn down.

We propose one direction that gives those features a subject: **Kusama is where groups of people grow their collective intelligence.**

The case starts outside crypto. The most valuable systems now being built are made from human work: the writing, judgement, disagreement and decisions of people in real scenes. That material sits beneath every model, and it usually travels without a record of who made it, what they agreed it could be used for, or where the value went. Nobody designed it that way out of malice. It is what a system built to gather material at scale produces when consent and attribution were never part of the objective. Change the rules and the result changes. [Our guide](https://birdbrain.wtf/guide) takes that stack apart layer by layer.

A network that wants to rebuild the layer beneath the model needs five things, and each of the paper's candidate visions is one of them:

1. **Membership:** who is in the group. Personhood credentials belong here. Live on Kreivo today, with 21 communities and 707 memberships.
2. **A record:** what the group made and decided, with contributors attached, in a form that can be inspected and corrected. Working for a handful of groups, including us. Experimental.
3. **Permission:** what the record may be used for, with retrieval and training agreed separately. Privacy belongs here, as the way a group keeps control of its own material rather than as an end in itself. Proposed.
4. **A treasury and a currency:** so agreed use can pay the group that did the work. A ksmUSD belongs here, as does dUSD, which is already live. Small volume.
5. **Governance:** the group sets the rules for the other four. Private governance belongs here. Collectives on Kreivo vote today.

Together that is a new kind of institution: smaller than a company, owned by its members, able to remember, decide and account for itself. Labs, record labels, magazines, guilds and co-operatives each carry useful habits, but none was designed for this. Kusama began as the place code was tested before Polkadot. steven's line at #19 names the next job: a frontier tests institutions. This is the institution we think Kusama should test.

Three things follow, and they shape the rest of this proposal.

- **Many intelligences, not one centre.** The direction is many independent collectives with room to disagree. That needs a network whose rules can differ from its neighbour's, which is the case for independence (§1).
- **KSM grows with people, not with the security bill.** Every member admitted, every collective treasury and every paid query is a use of KSM that scales with the groups living here (§4, §5). Staked KSM secures the ground they stand on, and later the groups can bring stake of their own (§3).
- **Builders before infrastructure.** Coretime is only worth buying if someone has a reason to use it. The builders Kusama Vision funds are the people who will make these institutions (§6).

Where this stands: membership, treasuries, payments and voting are live at small scale. The record and permission layers work for a few groups. Whether collectives built this way turn out meaningfully different from each other, fairer or more creative is still a claim that has to earn evidence, and §8 is how the DAO would find out.

## 1. Answer Rom1's question first: independence

Rom1 asks at #21 whether Kusama wants to be more independent or a better canary for Polkadot. We think the answer is independence, for three reasons.

- **It is already decided.** #573 passed. The JAM Prime paper asks KSM DAO to reconsider it (§5.6). A vote that passed should need a reason to reverse, and a cheaper core price on another network is not one.
- **A canary role is a service, not an identity.** Emiel suggests at #20 that Kusama could adopt Parachain Service upgrades ahead of Polkadot, which is real value to Polkadot. If Polkadot wants that, it can buy it. Kusama running someone else's risk is a reason for Kusama to be paid, not a reason for Kusama to pay US$8.64m.
- **The frontier needs room.** steven puts it well at #19: "A testnet tests technology. A frontier tests institutions." Institutions only get tested where the rules can differ. That means Kusama's own governance, its own monetary policy and its own validator set.

## 2. Security, sized to demand and paid for today

#573 specifies 32 cores, one-second blocks and KSM as the native token for staking, storage and coretime. Using the JAM Prime paper's own ratio of 3 validators per core, that is about **96 validators**. At the paper's own benchmark of US$3,000 a validator-month, that costs **US$3.46m a year**.

Kusama already pays for more than that. It issues about 1.34m KSM a year to staking, which is **US$5.9m at US$4.42**. At today's price, today's issuance pays for a #573-sized set 1.7 times over. Nobody has to sell the treasury and nobody has to ask DOT DAO for anything.

The costs are not the problem. The problem is that issuance at that level is around 7% a year, and #573 wants it at around 2.4%. At 2.4%, issuance is worth about US$2.0m, which leaves a gap of roughly US$1.46m against the US$3.46m bill. So we propose:

- **Shrink the set in stages** from 700 towards the #573 configuration, as #655 already began.
- **Taper issuance against revenue, not against a calendar.** Issuance steps down each time measured protocol revenue (§5) covers another slice of the security bill. If revenue does not arrive, issuance does not fall, and the DAO can see why.

## 3. What staked KSM is for

red asks at #14 and #18 what happens to the staking economy if Kusama no longer runs NPoS. Today 8.82m KSM is staked, which is 46.7% of all KSM. Under JAM Prime the only answer so far is red's own, KSM-backed candidates competing in one shared JAM Prime set, and the authors have not replied to it yet.

Under this proposal the answer is simple. Staked KSM keeps its current job, securing Kusama's own validators. Nominators still nominate. Existing operators compete for fewer seats on the same hardware terms. Fewer validators with the same stake means more stake behind each seat, so the set gets smaller without getting cheaper to attack.

Later there is a second job. Collectives and parachains that depend on Kusama can post KSM as stake behind the set that secures them. Security is then brought by the chains that use it, rather than sold to them. This is proposed, not built.

## 4. Stop selling the treasury and spend its surplus on members

Kusama's treasury on Asset Hub holds **879,525 KSM** today, about US$3.9m. It has been growing by about 434,000 KSM a year net of spending since the burn stopped in February 2025, although single large referenda can take out tens of thousands at a time. The usual way to spend it is to hand out grants that get sold for dollars and never come back.

We propose a standing rule instead ([RFC-001](https://birdbrain.wtf/rfc/rfc-001-treasury-as-onboarding-subsidy)):

- **The standing balance is a reserve and is not spent.** Annual spending stays below net inflow.
- **An onboarding facility** pays the on-chain cost of admitting people and collectives as members, about 0.3 KSM each, at a fixed formula, with every payout on the public ledger. On Kreivo that KSM goes into a treasury governed by the collectives themselves. It does not go to a company and it does not go to us.
- **A suggested first-year bar is 100,000 subsidised memberships,** which costs about 30,000 KSM. That is 7% of one year's inflow. Today there are 707 memberships across 21 communities on Kreivo, so the bar is 140 times the current base, which is why it counts as a test.

This answers Position 9 of the paper, which asks why anyone would acquire, use or hold KSM. Membership gives KSM a use that grows with the number of people joining, rather than with the size of the security bill.

## 5. Revenue: build the route during the runway

This route does not exist yet, and we would rather say so first. Today, **no mechanism routes any Kusama-side revenue to the security budget.** Polkadot is building exactly this as its allocation pool, which is a fund between protocol income and protocol costs, with outflows that governance adjusts. We propose Kusama builds a smaller one, with these inputs:

| Source | Status today |
|---|---|
| Coretime sales | Live but small. Sale #32 had a floor of 1 KSM and no new purchases. |
| Membership admissions | Live on Kreivo, about 0.3 KSM each, paid into Kreivo's own treasury, which holds 497.7 KSM. Any share to Kusama would need a vote by Kreivo's collectives. |
| Commerce fees | Live on Kreivo: 1% from the sender and 3% from the recipient, charged in the asset paid, so a dUSD payment pays its fee in dUSD. Volume is small. |
| Canary services to Polkadot | Proposed. Priced, if DOT DAO wants it. |
| Metered queries against collectives' records | Built and priced (0.01 dUSD per query plus 0.001 per row). It has settled seven payments on mainnet, all between our own keys, so it proves the payments work but not that anyone outside wants it. |

The arithmetic sets the bar. Covering the #573 gap of US$1.46m a year from a 1% fee takes US$146m of payment volume. Across one million members that is US$146 each a year, about US$12 a month. That is arithmetic, not a forecast.

## 6. Kusama Vision and the builders

Leave #498 alone. Its 10m DOT was committed "for the sole benefit of Kusama" and the bounties built on it are for builders, not infrastructure. We agree with edvoki (#17) that KV should give a public account of what it has delivered since January, and with olanod (#16) that it should be refocused on service builders rather than JAM implementers. The builders are who the coretime is for.

## 7. A Kusama fellowship with a delivery plan, and no rushed exit

Emiel is right at #20 that an independent fellowship needs identified maintainers, a defined scope, a migration plan, a budget, security review, incident response and continuity. We take that list as the conditions. So:

- **The Polkadot Fellowship's stewardship is not given up** until a successor meets all seven conditions and KSM DAO votes that it does.
- **The budget is paid from treasury inflow, not the reserve.** Paseo's reference of US$62,500 a quarter, US$250,000 a year, is a floor, not an estimate. A realistic migration year is likely a multiple of that. At US$1m a year it is about 226,000 KSM, which together with the onboarding facility still fits inside net inflow.
- **Maintainers apply in public,** against the published scope, before any money is committed.

We cannot name the maintainers, and we should not be the ones who do. This section says what a credible call for them would require.

## 8. How the DAO would know it is failing

Every claim above should be labelled as built, borrowed, experimental or proposed, and tested against dates. We suggest four checkpoints, 18 months after a Wish For Change:

1. The validator set is at or below 200, with no rise in slashing or missed blocks.
2. The onboarding facility has admitted at least 100,000 members, and at least a quarter of them are still active after six months.
3. There is a fellowship with named maintainers and a published migration plan, and a governed route from at least one revenue source to the security budget has been built.
4. The standing treasury balance is no lower than at the start.

If the checkpoints are missed, KSM DAO reopens cohabitation. It would then do so with a real economy on the books, which is the "differentiated, connected economy" §3.6 of the JAM Prime paper says DOT DAO needs to see. So independence first is also the way to a cheaper deal later.

## What we are asking for

1. **Adopt the direction:** Kusama as the network where groups grow their collective intelligence, with the paper's candidate visions built as its components rather than as separate bets.
2. **Reaffirm #573** as the route, and treat JAM Prime as a fallback that the checkpoints above can trigger.
3. **Adopt the treasury rule:** keep the standing balance as a reserve, spend below inflow, and put a rule-bound onboarding facility in place.
4. **Taper issuance against revenue** rather than cap it, with the schedule published.
5. **Commission the fellowship call** against Emiel's seven conditions, and keep the Polkadot Fellowship's stewardship until it is met.

We are glad to bring the workings for any figure here. Every one of them can be read from the chain.

## Appendix A | figures and where they were read

Every figure below was read on 23 September 2026 unless marked otherwise, and each can be checked against the chain.

| Figure | Value | Source |
|---|---|---|
| Kusama treasury, Asset Hub | 879,525 KSM | Free balance of `F3opxRbN5ZbjJNU511Kj2TLuzFcDq9BGduA9TgiECafpg29` |
| Treasury net inflow | about 434,000 KSM a year | Twelve balance readings, 1 July to 18 September, in [`data/kusama-treasury-series.json`](data/kusama-treasury-series.json). Net of spending, over a steady ten-week period. A single large referendum can move tens of thousands, as between 1 and 10 July. |
| Total issuance | 18,875,798 KSM | Kusama Asset Hub state |
| Staked | 8,818,318 KSM (46.7%) | Era 10066 |
| Validators | 700 | Era 10066 |
| Issuance to staking | about 1.34m KSM a year | About 918 KSM per era, four six-hour eras a day |
| KSM price | US$4.42 | CoinGecko |
| Kreivo | 21 communities, 707 membership items, treasury 497.7 KSM | Kreivo state |
| Validators for #573 | about 96 | The JAM Prime paper's ratio of 3 validators per core, applied to #573's 32 cores |
| Security bill for #573 | US$3.46m a year | 96 × US$3,000 a validator-month × 12, the JAM Prime paper's own benchmark |
| Gap at 2.4% issuance | about US$1.46m a year | US$3.46m less issuance of about US$2.0m |

The US$3,000 benchmark and the 3-validators-per-core ratio are the JAM Prime paper's, used here so the two proposals are priced on the same terms. We do not claim they are the right numbers, only that they are shared ones.
