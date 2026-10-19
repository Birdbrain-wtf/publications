---
id: polkadot-changing-shape
slug: polkadot-changing-shape
title: "The Changing Shape of Polkadot: operators, mandates, money and design in the DOT DAO's new direction"
summary: A review of the referenda, entities and designs behind Polkadot's 2026 change of direction. It traces how the Polkadot Community Foundation moved from executing OpenGov decisions to operating products and proposing strategy, explains what its "units" are, and records where the new design puts discretion and where the DAO can still check it. A reference piece, not a set of proposals.
authors:
  - Birdbrain
published: 2026-10-19
updated: 2026-10-19
tags:
  - polkadot
  - governance
  - opengov
  - pcf
  - personhood
  - stablecoins
status: draft
publicationType: review
edition: 0.1.0
license: CC-BY-4.0
responds_to: https://polkadot.subsquare.io/referenda/1954
related:
  - https://forum.polkadot.network/t/a-unified-strategy-for-polkadot-alignment-on-value-capturing-goals-for-polkadot-s-product-platform-and-the-dotdao/18999
  - https://forum.polkadot.network/t/on-the-pcf-situation/18990
  - https://polkadot.subsquare.io/referenda/1955
---
# The Changing Shape of Polkadot: operators, mandates, money and design in the DOT DAO's new direction

**A review of how Polkadot is reorganising itself in 2026: who now operates what, which referenda authorised it, how the money is being redesigned, and where the DAO can still check the result.**

*19 October 2026, by [Birdbrain](https://birdbrain.wtf), a collective on [Kreivo](https://github.com/virto-network/kreivo).*

**Status and purpose.** This is a draft review, offered while [Referendum 1954](https://polkadot.subsquare.io/referenda/1954), the DOT DAO Strategy Mandate, and [Referendum 1955](https://polkadot.subsquare.io/referenda/1955), which confirms the Polkadot Community Foundation as operator of user onboarding, are both in their decision periods. It does not argue for or against either vote, and it makes no proposals. It is a record of our understanding, written so we can weigh our own work at Birdbrain against it and come back to it as things change. It tries to describe the shape of the thing being voted on, because most of that shape was assembled across thirty referenda over two and a half years and is hard to see from inside any one of them. Every on-chain figure was read from Subsquare on 19 October 2026 and is listed in Appendix A, with the full register in [`file data/referenda.json`](data/referenda.json).

**Disclosures.** We are a collective on Kreivo, a Kusama parachain. We do not hold DOT voting positions large enough to matter in any referendum discussed here. Several things the mandate proposes, per-person incentives, passkey joining and a dollar unit on Asset Hub, are things we run at small scale on Kusama, so we have a view on how they go wrong. [Decent Partners](https://www.decent.partners), which supports Birdbrain, has a commercial interest in dUSD, a dollar stablecoin whose reserves are held by a company, through its arrangements with [Brale](https://brale.xyz), and is an investor in [Bloque](https://bloque.sh). dUSD sits on the side of the line that the mandate's stablecoin section says the DAO will not back. We say so wherever it touches the argument. AI tools were used to assist with research, drafting and editing. We take full responsibility for the arguments and figures.

## Abstract

Polkadot is changing what it is for. The mandate in Referendum 1954 asks the DAO to count users before ecosystem size, to make one native stablecoin primary, to build a single consumer product platform, and to pay growth incentives to verified individual people under a per-person cap. Much of it matches what we have argued for in our own work.

The more consequential change is underneath. The Polkadot Community Foundation (PCF) was founded in 2024 as "an unopinionated entity with no agenda, roadmap, or business purpose except to take actions directed to it via OpenGov referenda". In 2026 it operates the Polkadot App, holds the key that would attest new users onto the People chain if Referendum 1955 passes, publishes the code for a product platform, admits privately funded "units" by its directors' decision alone, and is the proposer of the strategy that names it as the right body for communications. Each step had some authorisation. Taken together they add up to a change of role that no single referendum asked voters to approve.

We find three places where the new design concentrates discretion: who counts as a person for incentive purposes, who decides what the PCF takes on, and who is accountable for work done under the PCF's name with money that never passed through OpenGov. In each case the DAO keeps a check, but a weaker one than the mandate's language suggests, because the two DOT-holder seats on the PCF board have been empty since 2024 and recent decisive votes have run on very low turnout. We end by setting the same questions against our own design at Birdbrain, where we face smaller versions of each.

## 1. The entities, and what each now does

The change is easiest to follow as a cast list. Five bodies matter, and the boundaries between them have moved.

| Entity | What it was | What it does now |
| --- | --- | --- |
| **DOT DAO (OpenGov)** | Token-holder governance over the treasury and runtime | Sets direction through Wish For Change referenda, and in 1954 would bind everyone it funds to a single strategy |
| **Technical Fellowship** | Ranked body that whitelists runtime changes | Still the technical gate (1955 needs [Fellowship referendum 639](https://collectives.subsquare.io/fellowship/referenda/639)), now also named in 1954 as an entity that must "support this mandate" as a condition of continuing funding |
| **Web3 Foundation** | Funder of research, design and early product work | Paid, directly or indirectly, for all of the Polkadot App's research, design, development and legal costs until 2025 ([1573](https://polkadot.subsquare.io/referenda/1573)), and asked by the DAO to run an agents programme ([1660](https://polkadot.subsquare.io/referenda/1660)) |
| **Parity Technologies** | Core developer of the protocol | Built Project Individuality, the proof-of-personhood system the Polkadot App integrates, over three years ([1783](https://polkadot.subsquare.io/referenda/1783)) |
| **Polkadot Community Foundation** | A Cayman Islands foundation company to carry out OpenGov decisions off-chain | Publishes and operates the Polkadot App, holds the user-onboarding attester key, proposes strategy and stablecoin referenda, and admits units |

Two smaller parties sit inside the PCF's activity. **Novasama** builds the Polkadot App under contract (72.7% of the $1.03m in [1573](https://polkadot.subsquare.io/referenda/1573) was for software development "allocated for Novasama and external PCF Contractors"). **Autonomous Projects**, a Cayman firm, is the PCF's administrator and the proponent named on most of its referenda.

## 2. How the PCF got here: the referendum trail

Read one at a time, the PCF referenda look like routine housekeeping. Read in order, they describe a body acquiring a product, a payments stack, a personhood role and a policy voice.

| Submitted | Ref | What passed | What it added |
| --- | --- | --- | --- |
| Apr 2024 | [730](https://polkadot.subsquare.io/referenda/730) | Found the PCF, about 88,000 DOT ($600,000) for year one | A legal wrapper to execute OpenGov decisions. Founding design: no deliverables or payments to third parties "unless they have been pre-approved by tokenholders", public transparency reports, two board seats for DOT holders |
| Aug 2024 | [1082](https://polkadot.subsquare.io/referenda/1082) | PCF owns the Polkadot App's IP and source code, $50,000 for store and legal set-up | The PCF becomes the publisher of a consumer product |
| Feb 2025 | [1416](https://polkadot.subsquare.io/referenda/1416) | PCF may sign formal contracts for the Marketing Bounty | The PCF becomes the contracting party for an ongoing programme |
| May 2025 | [1573](https://polkadot.subsquare.io/referenda/1573) | About $1.03m for six months of app development | The DAO funds the app directly through the PCF |
| Jun 2025 | [1591](https://polkadot.subsquare.io/referenda/1591) | $632,000 to renew the PCF for a year | Year-two goals: appoint the two DOT directors and build a transparency hub |
| Jun 2025 | [1608](https://polkadot.subsquare.io/referenda/1608) | PCF to set up a Polkadot-branded payment card with Baanx | Payments enter the PCF's remit |
| Jul 2025 | [1681](https://polkadot.subsquare.io/referenda/1681) | PCF to sign with Hong Kong's OASES and form a Hong Kong subsidiary | The PCF can hold subsidiaries |
| Sep 2025 | [1737](https://polkadot.subsquare.io/referenda/1737), [1749](https://polkadot.subsquare.io/referenda/1749) | **Both rejected:** two attempts to define and run the DOT-director election | The two seats meant to represent DOT holders stay empty |
| Nov 2025 | [1783](https://polkadot.subsquare.io/referenda/1783) | $3.0m for personhood-based incentives | Money for verified people, disbursed by on-chain logic |
| May 2026 | [1900](https://polkadot.subsquare.io/referenda/1900) | $1,500 for a website and tooling | Described as moving the PCF "from a reactive entity into a proactive ecosystem operator" and opening it to "externally funded units" |
| Sep 2026 | [1944](https://polkadot.subsquare.io/referenda/1944) | dotUSD, proposed by the PCF "in an administrative role" | A native stablecoin goes live |
| Oct 2026 | [1954](https://polkadot.subsquare.io/referenda/1954) | Deciding: the DOT DAO Strategy Mandate, proposed by the PCF | A single strategy that names the PCF as having "a well-aligned mandate" for communications |
| Oct 2026 | [1955](https://polkadot.subsquare.io/referenda/1955) | Deciding: onboarding parameters for the Polkadot App | Approving it "also confirms PCF as the operator of the onboarding service" |

Three things stand out.

**The biggest change of role rode on the smallest budget.** Referendum 1900 asked for $1,500. Its text is the only on-chain source for "PCF 2.0" and for units, and the PCF's new website now calls it "the PCF 2.0 mandate" on every page. Voters approved a website budget. The vote itself was decided by one account voting 5M DOT at six-times conviction, about 99% of the aye side. Counting DOT without conviction, the two sides were close to level, 5.09M for and 4.56M against. Eight accounts each abstaining with 8.45M DOT supplied 93% of the turnout. We do not suggest anything improper in that. It is how conviction voting works. But it is thin ground for a constitution.

**The checks written into the founding were never switched on.** The founding design promised two DOT-holder directors, transparency reports and no third-party commitments without token-holder approval. The director elections failed twice in September 2025. In November 2025 a forum brief on [the appointment of DOT directors](https://forum.polkadot.network/t/appointment-of-dot-directors/16006) found "no publicly available record indicating that the PCF has issued any report". In June 2026 a DOT holder's [public request](https://forum.polkadot.network/t/request-to-the-pcf-a-public-roadmap-and-a-full-accounting-of-community-funds-for-the-polkadot-app/17982) for a roadmap and an accounting of the app's funds said a week later that private approaches had drawn no response. With both DOT-holder seats empty, the board that admits units and backs the new direction is made up only of the professional directors appointed under the founding design.

**The PCF now proposes the referenda that define its own role.** It proposed 1944 and 1954 (both from the account `16kZ9e6L…uDMf`, which also proposed 1955). In 1954 the DAO's strategy is written by the body the strategy then recommends. A forum post titled [On the PCF situation](https://forum.polkadot.network/t/on-the-pcf-situation/18990) puts the question in one line: "Financial independence is not equivalent to governance authorization."

## 3. Units: what "bring their own funding" means

The PCF's [units page](https://pcf.network/units/) says: "A unit is a team that brings its own funding and works for the PCF." Teams with their own funding propose a unit, and "if a proposal fits the PCF's Bylaws and objectives, its directors approve it and the unit starts straight away as a pilot operator." Referendum 1900 adds that the website "serves as an official communication channel (via email) for receiving proposals to form a PCF unit using one's own funding resources", and that "approved units will launch immediately as pilot operators".

In plain terms, a unit is a team whose budget never goes through the treasury and never faces a referendum. It pays its own way, from a company, a foundation, investors or anyone else. In return it gets to work under the PCF's name and, through the PCF, with the legitimacy of the DOT DAO's own legal entity. The only gate is the PCF's directors, checking against bylaws and objectives that are broad by design.

There is one unit today, the [Human Web Initiative](https://pcf.network/human-web-initiative/). It is "independently funded" and "brings a renewed initiative with a clear direction for the PCF". Its funder is not named anywhere we could find. A forum participant [asked directly](https://forum.polkadot.network/t/on-the-pcf-situation/18990) whether Parity's work on the Polkadot App and its devnet releases sits inside this unit with its own external funding, or still under the app funding approved through OpenGov. As of 19 October the question is unanswered.

Units are not a bad idea. A DAO cannot vote on every hire, and outside money that wants to work for a public network is welcome. The difficulty is structural, and it would apply to anyone who ran a unit, including us.

- **Direction can be bought without a vote.** A unit "brings a renewed initiative with a clear direction for the PCF". If the PCF's direction can be set by whoever funds a unit, then the DOT DAO's influence over its own legal entity depends on who else is paying.
- **The DAO cannot withhold what it never gave.** The founding design made treasury funding the main lever: "DOT holders can choose to withhold future funding … if they are unhappy with the Foundation." A unit's money comes from elsewhere, so that lever does not reach it.
- **Credit and blame have nowhere to land.** When work ships under the PCF's name, holders cannot tell what the DAO authorised, what a unit decided and what the funder wanted. That is the accountability question the founding bylaws tried to answer with transparency reports.
- **It collides with the founding rule.** The founding design, as the [Polkadot Wiki](https://wiki.polkadot.com/general/pcf/) sets it out, forbids the PCF agreeing "to any deliverables, responsibilities, or payments to third parties unless they have been pre-approved by tokenholders". A unit that "works for the PCF" is a standing arrangement with a third party. Either units sit outside that rule, which needs explaining, or each one needs a referendum, which is not what the units page describes.

## 4. Money: what has changed

The money side moved in the same two years, mostly through Wish For Change referenda that set direction for the Fellowship to implement.

- **Supply is capped.** [Referendum 1710](https://polkadot.subsquare.io/referenda/1710) set a total supply of 2.1 billion DOT, with issuance stepping down every two years from 14 March 2026. The same proposer's figures in [1781](https://polkadot.subsquare.io/referenda/1781) put treasury income at about 18M DOT a year, falling to 8.3M at the first step.
- **The treasury stopped burning.** [Referendum 1781](https://polkadot.subsquare.io/referenda/1781) ended the burn of 1% of the treasury every 24 days, on the argument that a capped supply makes treasury funds scarcer.
- **Budgets moved into dollars.** The [Dynamic Allocation Pool](https://polkadot.subsquare.io/referenda/1827) collects fees and coretime revenue, and later staking parameters were set as budgets ([1909](https://polkadot.subsquare.io/referenda/1909)). The dotUSD announcement gives this as a reason a native dollar is needed.
- **A native dollar went live.** [Referendum 1944](https://polkadot.subsquare.io/referenda/1944) created dotUSD on 8 October, seeded with $2.5m of treasury USDT and $2.5m of DOT. Phase one, live now, mints dotUSD one for one against USDT up to a cap. Phase two adds DOT-collateralised vaults on a Liquity v2 design. It passed on the Root track with 1.87M DOT of support.
- **JAM economics are being settled in principle.** [Referendum 1926](https://polkadot.subsquare.io/referenda/1926) asked that all DOT the DAO receives from selling JAM state footprint be burned, and that none be given as grants. [1927](https://polkadot.subsquare.io/referenda/1927), a narrower version, was rejected.
- **The Fellowship is being repriced.** [Referendum 1931](https://polkadot.subsquare.io/referenda/1931) cut passive salaries for ranks 3 and above to a flat $10,000 a year. A request to fund the salary account with 4.8M DOT converted to HOLLAR ([1940](https://polkadot.subsquare.io/referenda/1940)) was cancelled.

Two observations for the mandate.

**The primacy of dotUSD is a claim about phase two.** Section 2 of 1954 backs dotUSD on the grounds that it runs on collateral logic rather than a third party who "holds, controls, and can potentially invest the underlying collateral". Today, in phase one, dotUSD's backing is USDT, a coin issued by exactly that kind of third party. The mandate is right that the destination differs from USDT. For now the coin in people's hands is a wrapper around it. We have an interest here, because dUSD is a custodial coin, so we say only that the distinction the mandate draws will be true when phase two ships, and is not yet.

**Primacy has a cost for builders already here.** Hollar is a sufficient asset on Hub ([1920](https://polkadot.subsquare.io/referenda/1920)). A native pUSD on the Honzon protocol was proposed and rejected ([1761](https://polkadot.subsquare.io/referenda/1761)). A mandate that requires funded entities to give one coin primacy decides between teams that competed in good faith. That may be the right call. As written, it is made as one clause in a six-part strategy, not as a decision of its own.

## 5. Design: personhood, and who decides who counts

The mandate's growth model depends on one design choice: pay incentives "into the hands of individual human users under some algorithmic per-person-limit". That needs a way to tell people apart. Here the design is good at one layer and loose at the next.

**At the protocol layer, discretion is designed out.** [Referendum 1783](https://polkadot.subsquare.io/referenda/1783) describes Project Individuality as requiring "no identity documents, phone numbers, email addresses, card details or bank payments", giving each user an unlinkable alias per application, and running its first two mechanisms, Proof-of-Ink and Proof-of-Video-Interaction, under Polkadot governance on the People chain. It says of the $3m incentive pot: "Neither Parity nor any other ecosystem entity has any role or authority in disbursement nor any operational function or privilege." That is a careful design.

**At the app layer, discretion comes back.** The Polkadot App's user terms, under which the PCF operates the app "in all respects", define verification as "Proof of Video Interaction (and/or any other 'Proof of' verification system introduced by the Company from time to time)". The governance-run mechanism is one option among any the operator chooses to add.

**At the onboarding layer, it is explicit.** Referendum 1955 lets an attester register up to one million "lite people" on the People chain and reserve a `.dot` name for each. Its own text says a lite person "shows that an account comes from an app installation the onboarding service has verified and attested, not that it belongs to a unique human". The attester signs with "the onboarding service key … held by the PCF". If that key were compromised, the holder "could register lite people and reserve names for accounts of their choice, up to the remaining allowance". The PCF states one trade-off plainly: the dotNS dispatcher it owns is upgradeable, and "if PCF upgraded that contract with an illegitimate version of the source, the new code could call other contracts that trust Root origin". It offers a public time delay "that a referendum can veto" as an interim guarantee.

This is unusually candid, and the PCF deserves credit for publishing the call data, dry runs and a fork rehearsal. But it shows where the incentive system's judgement lives. The thing that decides who receives money per person is two steps away from the autonomous logic in 1783: an app whose operator can add verification methods, and an attester whose key one organisation holds. Lite personhood is not personhood, and the mandate does not say which tier its per-person limit counts.

## 6. Governance: who actually decided

The new direction is being set by very few votes.

- **1954**, the strategy mandate, had 803,112 conviction-weighted DOT for and 210,570 against on 19 October, with support of 419,551 DOT. That is about 0.03% of issued DOT. Wish For Change thresholds fall as the decision period runs, so on these numbers it can pass near the close around 10 November.
- **1955**, the onboarding operator confirmation, had support of 346,806 DOT. It enacts no earlier than 22 October if it passes.
- **1944**, dotUSD on the Root track, passed with support of 1.87M DOT.
- **1900**, the "PCF 2.0 mandate", turned on one account and on abstentions, as set out in §2.

Low turnout is not new in OpenGov, and nobody should blame the people who turned up. It is a design property: thresholds that decay towards zero let a direction pass if nobody large objects in time. The consequence is that the DAO's authorisation for the most significant change of role in its history is real but shallow, and that matters more when the body being authorised is also the body proposing.

The PCF's board adds a second gate that holders cannot easily see. Under Article 6.4 of the bylaws, as [summarised on the forum](https://forum.polkadot.network/t/appointment-of-dot-directors/16006/3), directors can reject a token-holder-approved proposal within sixty days on legal and operational grounds. That is a reasonable protection for a legal entity. With both DOT-holder seats empty, it is exercised entirely by the professional directors approved as a slate at founding, none of whom holds a seat elected to represent DOT holders.

## 7. Incentives: who gains under each pillar

A direction is also a set of incentives. Reading 1954 for who benefits, not who is blamed:

| Pillar | Who it rewards | What could go wrong by design |
| --- | --- | --- |
| Users before ecosystem size | Teams that can show active people | Activity bought with the incentive pot looks like adoption, because the pot pays for being active |
| dotUSD primacy | The protocol, which keeps the float and fees | Phase-one backing is USDT, and competing native stablecoins lose funded integrations |
| One product platform | Whoever operates the platform | The platform's operator becomes the default gate for every product built on it |
| Per-person incentives | People who pass verification | Whoever sets verification sets the payroll, and lite personhood counts installs, not people |
| Freemium and personhood | New users | Free tiers subsidised by the DAO make the app operator the main buyer of network resources |
| Funded entities must comply | Coherence | The Fellowship's independence becomes conditional on agreeing with a strategy it did not write |

None of these is a case against the direction. Each marks a place where the outcome depends on who holds a role, more than on what the mandate says.

## 8. Reading it against ourselves

This piece is mostly for us. Birdbrain runs small versions of the same machinery on Kusama, and each of Polkadot's pressure points has a counterpart in our design. We record them here so we can check our own work against them, not to suggest Polkadot copy or avoid anything.

| Polkadot | Birdbrain's counterpart | What to watch in our own work |
| --- | --- | --- |
| The PCF's role grew through small referenda, each with some authorisation | Our collectives move from being run by an operator, to a trusted group, to their own governance, and we have written that a change of role is its own proposal | Whether a change of role ever arrives inside something smaller, such as a plugin, a budget or a release |
| The PCF holds the onboarding attester key | Birdbrain's operator key signs memberships in its Kreivo community | What that key could do if it were misused or lost, and whether members can see what it signs |
| Units: outside money working under the PCF's name, admitted by directors | Plugins and asks filed by members, decided by the collective's current stage | Whether anyone can bring money that sets direction without passing that stage |
| Individuality at the protocol, discretion at the app, attestation at onboarding | Passkey joining: a key the person holds, plus membership of the group | Our passkey proves a device and a membership, not a unique human, the same gap 1955 states for lite people |
| dotUSD's primacy rests on phase two, phase one is USDT | dUSD, whose reserves are held by a company | We sit where the mandate's line says the DAO will not go, and our descriptions of dUSD need to say so |
| Decisive votes on low turnout and high conviction | Kreivo ranks, proposed for our collectives | One large holder plus abstentions could carry small decisions when few people vote |
| Founding checks written down and never switched on | Our written promises: the contributor promise, the door kit, objection windows | Which of ours exist only on paper, and who would notice |

## 9. Why this matters beyond Polkadot

Every network that moves from protocol to product meets the same problem. A DAO is good at setting direction and bad at running a product. A legal entity is good at running a product and hard for a DAO to steer. The PCF is one of the most serious attempts yet to join the two, and its founding documents are better than most. 

What 2026 shows is that the joint fails quietly. It does not fail when someone seizes control. It fails when the checks are designed in and never switched on, while the role grows one small, reasonable referendum at a time.

We face the same problem at our own scale. Reading Polkadot's last two years has made us more sure that a change of role should be its own decision, and less sure that writing that down is enough.

## Appendix A | the referendum register

Conviction-weighted ayes and nays, and support in DOT without conviction, read from the Subsquare API on 19 October 2026. The full register, with tracks and calls, is in [`file data/referenda.json`](data/referenda.json).

| Ref | Subject | Outcome | Ayes | Nays | Support |
| --- | --- | --- | --- | --- | --- |
| [730](https://polkadot.subsquare.io/referenda/730) | Found the PCF | Executed | 57.4M | 0.66M | 20.8M |
| [1082](https://polkadot.subsquare.io/referenda/1082) | PCF owns the Polkadot App | Executed | 54.1M | 0.02M | 15.0M |
| [1416](https://polkadot.subsquare.io/referenda/1416) | PCF contracts for the Marketing Bounty | Executed | 37.7M | 0.04M | 9.2M |
| [1573](https://polkadot.subsquare.io/referenda/1573) | Polkadot App funding #01 | Executed | 41.8M | 20.0M | 11.4M |
| [1591](https://polkadot.subsquare.io/referenda/1591) | PCF renewal, year two | Executed | 45.4M | 26.7M | 14.1M |
| [1608](https://polkadot.subsquare.io/referenda/1608) | Polkadot payment card | Executed | 46.9M | 0.07M | 10.0M |
| [1681](https://polkadot.subsquare.io/referenda/1681) | Hong Kong agreement and subsidiary | Executed | 32.6M | 14.7M | 7.3M |
| [1710](https://polkadot.subsquare.io/referenda/1710) | 2.1B DOT supply cap | Executed | 23.9M | 5.6M | 10.8M |
| [1737](https://polkadot.subsquare.io/referenda/1737) | DOT-director election process | Rejected | 14.1M | 17.3M | 4.6M |
| [1749](https://polkadot.subsquare.io/referenda/1749) | DOT-director appointment | Rejected | 3.7M | 10.3M | 1.4M |
| [1761](https://polkadot.subsquare.io/referenda/1761) | Native pUSD on Honzon | Rejected | 5.6M | 24.7M | 1.7M |
| [1781](https://polkadot.subsquare.io/referenda/1781) | End the treasury burn | Executed | 146.0M | 10.9M | 48.1M |
| [1783](https://polkadot.subsquare.io/referenda/1783) | Personhood incentives, $3.0m | Executed | 160.9M | 22.6M | 55.1M |
| [1827](https://polkadot.subsquare.io/referenda/1827) | Dynamic Allocation Pool, phase 1 | Executed | 14.7M | 0 | 4.8M |
| [1900](https://polkadot.subsquare.io/referenda/1900) | PCF website and tooling ("PCF 2.0") | Executed | 30.3M | 14.0M | 71.8M |
| [1926](https://polkadot.subsquare.io/referenda/1926) | Burn all DOT from JAMKB sales | Executed | 129.5M | 0.01M | 128.8M |
| [1927](https://polkadot.subsquare.io/referenda/1927) | Settle JAM footprint releases in DOT | Rejected | 0.43M | 141.0M | 0.25M |
| [1931](https://polkadot.subsquare.io/referenda/1931) | Fellowship passive salaries | Executed | 26.8M | 0 | 131.9M |
| [1940](https://polkadot.subsquare.io/referenda/1940) | Fellowship salaries in HOLLAR | Cancelled | 0.07M | 13.2M | 0.02M |
| [1944](https://polkadot.subsquare.io/referenda/1944) | dotUSD | Executed | 4.63M | 0.07M | 1.87M |
| [1954](https://polkadot.subsquare.io/referenda/1954) | DOT DAO Strategy Mandate | Deciding | 0.80M | 0.21M | 0.42M |
| [1955](https://polkadot.subsquare.io/referenda/1955) | Polkadot App onboarding, PCF as operator | Deciding | 0.72M | 0.16M | 0.35M |

## Appendix B | questions we could not answer

1. Who funds the Human Web Initiative, and is any Polkadot App or devnet work paid for through it rather than through 1082 and 1573?
2. Have any units other than the Human Web Initiative been proposed, and were any declined?
3. Has the PCF published any of the transparency reports its founding design requires, and where?
4. Does the per-person limit in 1954 count lite people, verified individuals, or both?
5. Which verification methods, beyond Proof-of-Video-Interaction, has the Polkadot App's operator added or planned under its user terms?
6. Who holds the accounts that decided 1900? The identity service we used was unavailable when we checked.