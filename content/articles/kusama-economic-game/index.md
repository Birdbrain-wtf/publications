---
id: kusama-economic-game
slug: kusama-economic-game
title: "The Game That Decides Kusama: stake, conviction and who can enact a direction"
summary: A research note on the decision machinery behind Kusama's JAM-era choice. Who holds the voting weight, what the on-chain record shows about how it is used, and what that means for any proposal that changes what KSM holders are paid.
authors:
  - Birdbrain
published: 2026-09-25
updated: 2026-09-25
tags:
  - kusama
  - governance
  - opengov
  - tokenomics
  - jam
status: published
publicationType: research-note
edition: 0.1.0
license: CC-BY-4.0
responds_to: https://forum.polkadot.network/t/a-proposal-for-a-kusama-future-on-jam-prime/18683/26
related:
  - https://github.com/sdfinst/publications/blob/a445bba7ab5a801e3b85168551dfa8b1e5021bc2/content/articles/proposal-kusama-future-jam-prime/index.md
  - https://github.com/Birdbrain-wtf/publications/blob/7488de34272274d1a3ff393a7e84849589c9ecb9/content/articles/independent-kusama/index.md
---
# The Game That Decides Kusama: stake, conviction and who can enact a direction

**A research note on the decision machinery behind Kusama's JAM-era choice.**

*25 September 2026, by Birdbrain. Figures read from Kusama Asset Hub at block 21,805,917 and from the Subsquare vote index the same day. Every figure is in the `data/` folder next to this note.*

**TL;DR.** The discussion of Kusama's future has been about strategy: independence or canary, how many cores, at what price. Very little of it has been about how any of those directions would actually be enacted. Kusama is a single-asset game. Every decision is settled in one numeraire, KSM balance multiplied by conviction, and whoever holds enough of it decides. On the record of 245 referenda, one block of about 20 unlabelled accounts, voting in perfect lockstep, holds roughly **2.56 million KSM: 13.6% of all KSM and 29% of all staked KSM.** Five of those accounts are the source of Web3 Foundation's own Decentralized Voices delegations. The block took part in 110 of the referenda we sampled, carried a median 77% of the weight cast in them, and reversed the outcome of 12, eight of them in 2026. The largest organised voice outside it, ChaosDAO, carries about 90,000 delegated KSM, of which 80,000 comes from a single account. JAM Prime would end staking issuance for the 8.8 million KSM that is staked today, and it would be decided by the same KSM. We think the people proposing a direction, and the people holding the weight, should say plainly how they expect it to be enacted.

---

## Our interest, declared

We are [Birdbrain](https://birdbrain.wtf), a collective on [Kreivo](https://github.com/virto-network/kreivo), one of Kusama's 12 non-system parachains, which uses KSM as its fee token. We published [a counter-proposal](https://github.com/Birdbrain-wtf/publications/blob/7488de34272274d1a3ff393a7e84849589c9ecb9/content/articles/independent-kusama/index.md) to the JAM Prime paper on 23 September, and it carries our full disclosures. We hold a small amount of KSM and no voting weight that would register in anything below. Two Wish for Change referenda associated with us, [#506](https://kusama.subsquare.io/referenda/506) and [#623](https://kusama.subsquare.io/referenda/623), failed in this same machinery, so we have seen it from the losing side. [Referendum 665](https://kusama.subsquare.io/referenda/665), our 8 KSM bounty, is deciding now. Read what follows with that in view.

## 1. The question the thread has not asked

The [JAM Prime paper](https://github.com/sdfinst/publications/blob/a445bba7ab5a801e3b85168551dfa8b1e5021bc2/content/articles/proposal-kusama-future-jam-prime/index.md) addresses three parties by name. Appendix A is for the Polkadot Fellowship and the JAM implementers. Appendix B is for Web3 Foundation and its economists, to inform Vision Fund decisions. The settlement is a negotiation with DOT DAO. The fourth party, the KSM vote that would have to pass the proposed Wish for Change and reverse [#573](https://kusama.subsquare.io/referenda/573), appears only as a procedural step.

Two of those parties hold the resources outright. The 10 million DOT recorded in [WFC #498](https://kusama.subsquare.io/referenda/498) came from Web3 Foundation's own treasury, and the paper itself says W3F's authorisation of its contribution is separate from anything KSM DAO decides. That money moves at W3F's discretion. Everything else, the direction, the reversal of #573, the monetary redesign, the end of the validator set, has to pass through KSM governance.

The paper does not say whose KSM would pass it. Nor, so far, has anyone in the thread. The confidence of the proposition, and much of the engagement with it, reads as though the enacting weight were already known. We do not think a paper by a team with no route into W3F and Parity's strategic thinking, and no stake behind it, would have been received this way. It would have been read as one more Wish for Change, of which Kusama has had 48.

That is not a criticism of the authors. They declare more than most: a JAM implementation project, business interests in staking operations, ventures that would use JAM infrastructure, and exposure to both ecosystems. It is a description of how the game works, and it is the part of the conversation we would like to make explicit.

## 2. The rules of the game

Kusama and Polkadot are, at their simplest, economic games played around one asset each. On Kusama that asset decides everything:

- **Voting weight is balance times conviction.** Any KSM can vote, staked or not. Conviction multiplies it in exchange for a lock after the vote: 0.1x with no lock, then 1x, 2x, 3x, 4x, 5x and 6x for 1, 2, 4, 8, 16 and 32 lock periods. The lock period is set in the runtime at 100,800 blocks, seven days, so a 6x vote locks the KSM for 224 days.
- **Delegation is per track and carries conviction with it.** A holder can hand their weight to someone else on any of the governance tracks, at up to 6x. Delegated weight is voted by the delegate, and it is invisible in the delegate's own balance.
- **A Wish for Change is decided by whoever turns up.** On the Wish for Change track the approval threshold falls to a simple majority over a 14-day decision period and the support threshold falls to zero. [#573](https://kusama.subsquare.io/referenda/573), the independent JAM, passed with 42,691 KSM of support, 0.23% of all KSM. Any holder large enough to outweigh everyone else who turns up can decide a Wish for Change on their own.
- **A Wish for Change binds nobody.** It is a remark on chain. It records what the DAO wants and leaves the Fellowship, W3F and every other party free to act on it or not. Its weight is political, which is why who voted for it matters more than the tally.

The founding idea of proof of stake is that those with the most at stake should have the most say. Delegated proof of stake makes that more liquid, because weight can be lent to people who show up. Those are the rules, and they are not in dispute. What follows is what they produce.

## 3. Who holds the weight

We read every vote in 245 referenda (every one with more than 300,000 conviction-weighted votes cast, plus the Wish for Change referenda that shaped this discussion), resolved the on-chain identity of 2,899 voting and delegating accounts on the Kusama People chain, and read current balances from Kusama Asset Hub. The method and its limits are in Appendix A.

**One block dominates.** About 20 accounts with no on-chain identity each hold between 108,000 and 165,000 KSM, nearly all of it staked. They vote the same way as each other every time they vote together: 81 out of 81 shared referenda for one pair, 70 out of 70 for another. They vote mostly on runtime upgrades, system spends and treasury proposals, mostly aye, usually at 1x or 2x conviction.

We split them into two tiers, because we can prove one and can only infer the other.

| Tier | Accounts | KSM held today | How we know |
|---|---|---|---|
| A | 7 | 656,816 | Each was the source of a 5,000 KSM delegation at 6x to a Decentralized Voices delegate. [Web3 Foundation states](https://medium.com/web3foundation/decentralized-voices-program-93623c27ae43) that it delegates its own KSM to that programme, in exactly that shape. Five of the seven also vote directly with 124,000 to 130,000 KSM each. |
| B | 17 | 1,907,597 | No identity, same size, same staking pattern, and the same vote as tier A in every referendum both took part in. We cannot see who controls them. |
| **Block** | **24** | **2,564,413** | **13.6% of all KSM (18,885,656). 29.1% of all staked KSM (8,800,865).** |

We cannot tell Web3 Foundation's accounts from Parity's on chain, and we have not tried to. We call it the W3F/Parity-aligned block because tier A is W3F's by W3F's own description, and tier B moves with it without exception. If any of tier B belongs to someone else, we would welcome the correction, and the list is in `data/block-accounts.csv`.

At 1x conviction the block is 2.56 million votes. At 6x it is 15.4 million. The largest aye tally in Kusama's OpenGov history is 2.42 million.

**The organised community is smaller, and more concentrated than it looks.** [ChaosDAO](https://forum.polkadot.network/t/decentralized-voices-program-chaosdao/6138) is the largest identified voting body outside the block, and it decides its votes by one member, one vote among roughly 80 active voters. Its weight is delegated. On [#659](https://kusama.subsquare.io/referenda/659) in September, 85 accounts delegated it 89,443 KSM, voted at 3x for about 277,000 votes. **80,000 of that KSM, 89%, came from one account**, which still delegates 80,000 KSM to ChaosDAO at 3x today. The same account voted directly on [#596](https://kusama.subsquare.io/referenda/596), and on its own carried 37% of the weight that rejected it.

Beyond that, the Decentralized Voices delegates each carry 30,000 votes of W3F's KSM, and a long tail of individuals carries the rest. Roughly 16 million KSM, most of the supply, does not vote at all.

## 4. What the record shows

**The block is the swing vote whenever it chooses to be one.** It took part in 110 of the 245 referenda we sampled and carried a median 77% of the weight cast in them. In 12 of them, removing its votes reverses the result, and eight of those were this year:

| Ref | Date | What | Block | Result |
|---|---|---|---|---|
| [#627](https://kusama.subsquare.io/referenda/627) | Jan 2026 | Sustainable KSM Economics via Burn Mechanisms | 537,500 nay | Rejected |
| [#643](https://kusama.subsquare.io/referenda/643) | Mar 2026 | System Parachain Collator top-up | 1,594,400 aye | Executed |
| [#647](https://kusama.subsquare.io/referenda/647) | May 2026 | Kusama Vision Proof of Personhood bounty | 1,047,000 aye | Executed |
| [#649](https://kusama.subsquare.io/referenda/649) | May 2026 | Kusama Vision ZK Proofs bounty | 1,047,000 aye | Executed |
| [#650](https://kusama.subsquare.io/referenda/650) | May 2026 | Funding for public RPC providers | 1,594,400 aye | Executed |
| [#652](https://kusama.subsquare.io/referenda/652) | Jun 2026 | Subscan invoice, 2025 Q3 to Q4 | 1,778,000 aye | Executed |
| [#653](https://kusama.subsquare.io/referenda/653) | Jun 2026 | Subscan licence, 2026 | 1,778,000 aye | Executed |
| [#659](https://kusama.subsquare.io/referenda/659) | Sep 2026 | System Collator Bounty second top-up | 1,778,000 aye | Executed |

In seven of those eight, ChaosDAO voted nay and the block voted aye. That is Kusama's governance as it actually runs: two organised positions, one about thirty times the weight of the other.

**On strategy, the block mostly stays out, and it does not have to.** It did not vote on #573, the independent JAM, which is why that passed on 42,691 KSM of support. It did not vote directly on #498 either. That was carried by two unlabelled accounts holding about 1 KSM each, voting with 68,000 and 52,000 KSM delegated to them at 3x by two tier B accounts, which together cast 59% of all the weight on the referendum that committed W3F's 10 million DOT. Those delegations have since lapsed. The block can abstain on a direction, let a small turnout pass it, and remain the only party able to overturn it later. That is where a Wish for Change reversing #573 would land.

**On tokenomics, the record runs against the holder's short-term interest as often as with it.** The block voted against the burn mechanism in #627, which would have reduced supply. The capped and stepped supply schedule failed on Kusama as [#596](https://kusama.subsquare.io/referenda/596), decided largely by one delegator's direct vote, while [the same proposal](https://polkadot.subsquare.io/referenda/1710) passed on Polkadot as #1710 with 81% in favour. [#640](https://kusama.subsquare.io/referenda/640), asking that the Fellowship not be removed from Kusama without a Kusama vote, was rejected with 98% of the weight coming from ChaosDAO alone.

## 5. Polkadot's own experience

Polkadot runs the same machinery on a larger asset, and its record is both a demonstration of the power and a warning. On [Polkadot #644](https://polkadot.subsquare.io/referenda/644), a sports sponsorship fund in 2024, two wallets cast 38% of all the weight and pushed it over the line, [one of them created days earlier](https://www.reddit.com/r/dot/comments/1ckn73w/what_is_going_on_with_opengov_ref_644_two_whale). On #1710, the hard cap now in force, the six largest voters cast about half the weight between them. The rules worked exactly as written in both cases. Whether the outcome reflected the network or its largest balances is the question Polkadot has been living with since.

## 6. What JAM Prime changes in the game

The JAM Prime proposal would retire Kusama's validator set. Today 8,800,865 KSM, 46.6% of the supply, is staked, and staking issuance is what it earns. The proposal replaces that with a DOT-settled endowment, a planned hard cap and burns, and, in Emiel's words at [#26](https://forum.polkadot.network/t/a-proposal-for-a-kusama-future-on-jam-prime/18683/26), an assumption that released KSM will not all be sold that is "too strong", and an assumption of no economic effect that would be "equally careless".

What it does not change is the voting machinery. OpenGov weight is balance times conviction, not stake, so the people asked to decide are the same holders whose yield the proposal removes. The block alone holds 29% of staked KSM. The question every large holder faces is simple: does this direction serve my basic economic interest better than the alternatives?

That is where the untested part of the system sits. KSM DAO has never faced a proposal that materially changes what its holders are paid, against the wishes of a large share of them. The instruments for a holder under duress are all there: conviction up to 6x for 224 days, delegation to whoever will vote their way, and a turnout so low that a determined minority can decide a Wish for Change. KSM DAO is not a monolithic entity, but its governance has so far been monolithic. Anyone hoping to move the network in a direction a large holder dislikes should price in what that holder can do, the same way the paper prices cores.

## 7. Making the implicit explicit

We are not questioning anyone's motives. We are asking for the same thing the JAM Prime paper asks of every alternative: who delivers, who pays, which assumptions remain unverified. For enactment, that means four questions.

1. **To the authors.** Whose KSM do you expect to carry the Wish for Change in Appendix C, and in particular the reversal of #573? If the expectation is the block described here, say so, so holders can weigh the proposal knowing that.
2. **To Web3 Foundation and Parity.** Which Kusama accounts are yours, and will you vote on a Wish for Change about Kusama's JAM-era direction? Neutrality is a legitimate answer. Silence while holding 29% of staked KSM is also a position, because it leaves the decision to whoever turns up and the reversal to you.
3. **To ChaosDAO and its largest delegator.** The community's organised vote rests largely on one delegation. Is that delegator's interest the community's, and will it stay put through a vote about the validator set?
4. **To everyone else.** Most of the supply never votes. A direction that ends staking issuance will be decided by a handful of balances unless that changes.

## 8. Who operates the network

There is one more asymmetry worth naming. The people who proposed JAM Prime sit close to a large, well-funded and salaried research and engineering organisation, and to its strategic thinking. The people who have iterated Kusama's purpose, its capabilities and its story beyond what the core team imagined, from ChaosDAO's governance to Kreivo's communities to the parachains §5.4 would price off the network, have mostly done it for years on close to no funding, motivated by more than money.

Both sets of instincts matter. But when the question is which instincts should decide what Kusama becomes, and the builders are the ones facing extreme information asymmetry and unpredictable decisions made in rooms they are not in, it is worth pausing. Creativity loves constraints. In many ways that has become the working rule behind Kusama's "expect chaos". We expect the network's future to be decided by whoever best understands the incentives of the game we are all playing, and we would rather those incentives were on the table than assumed.

## Appendix A. Method, data and limits

**Referenda sampled.** Every Kusama OpenGov referendum from #0 to #666 with more than 300,000 conviction-weighted votes cast (240), plus #573, #600, #640, #654 and #665, for 245 in all. Votes from `kusama-api.subsquare.io/gov2/referenda/<n>/votes`, read 25 September 2026. `data/referenda-sample.csv` has each referendum's tally, the block's votes and whether removing them flips aye against nay.

**Identities.** `identity.identityOf` and `identity.superOf` on the Kusama People chain for all 2,899 accounts that voted or were delegated to in the sample.

**The block.** Tier A is any account that delegated exactly 5,000 KSM at 6x to a Decentralized Voices delegate, the shape W3F describes. Tier B is any account with no identity, at least 50,000 KSM in a single direct vote, and 100% agreement with the majority side of tier A across at least three shared referenda, plus the two proxy accounts that voted #498. `data/block-accounts.csv` lists every account and the evidence for each.

**Balances.** `system.account` on Kusama Asset Hub at block 21,805,917 (free plus reserved; frozen shown separately). Total issuance, active era and total stake from the same block. `data/chain-snapshot.json`.

**ChaosDAO.** Delegations to `DCZyhphXsRLcW84G9WmWEXtAA8DKGtVGSFZLJYty8Ajjyfa` on #596, #627, #650 and #659, in `data/chaosdao-delegations.csv`.

**Limits.** The block could be larger: exchange, custodial and liquid-staking balances are invisible here, as is any account that shares the block's controller but never voted with it. It could be smaller: tier B is an inference from behaviour, not a disclosure. "Flips the outcome" compares ayes with nays after conviction and ignores the approval and support curves, so it is a floor on the block's influence rather than a full reconstruction. We have not tried to attribute any account to a named person, and we would ask readers not to either. The point is the machinery, not the players.
