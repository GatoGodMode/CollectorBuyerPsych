---
title: The Neuro-Economic Architecture of Modern Collectibles
generated: 2026-06-13
source: research.html
---

# The Neuro-Economic Architecture of Modern Collectibles

A comparative psychological and market-structure analysis of physical TCG ecosystems, NFT/crypto markets, livestream “rip-and-ship” economies, and gacha-style digital monetization.

**Evidence tiers.** Empirical claims below cite peer-reviewed research, official regulator reports, or established news outlets. Where we cite **trade press, entertainment news, Reddit, or X**, we treat them as documentary / real-time signals and label user-generated content (UGC) accordingly. The WXYZ table is an **organizing scaffold** that labels themes for this essay; scored policy or clinical work needs its own instruments. Where we describe resale tactics, we separate **corroborated** incidents from **anecdotal** accounts.

Cited patterns on this page include highly skewed NFT trader activity (the most active decile of traders accounts for a dominant share of transactions in a large on-chain sample)[1]; anticipatory arousal before randomized “loot box” reveals in controlled experiments[2]; heavy-tailed resale prices for Pokémon cards on eBay in a prospective listing study[3]; and survey-based evidence that NFT-linked art can be perceived as less “permanent” than physical art despite blockchain persistence[4]. Cryptocurrency ownership correlates with psychological and social variables in large-sample work[5], and NFT markets exhibit systematic rug-pull fraud in security measurement research[6].

## 1) WXYZ Framework for Market Psychology

We use the WXYZ model for side-by-side comparison:

| Axis | Dimension | Low-Risk Profile | High-Risk Profile |
| --- | --- | --- | --- |
| X | Temporal maturity | Decades-long market memory (e.g., TCG since 1996) | Young/high-volatility cycles |
| W | Asset medium | Physical ownership with friction (storage, grading) | Digital abstraction with high liquidity |
| Y | Greed vs. output | Cultural/play utility and community output | ROI-maximization and extraction-first behavior |
| Z | Moral alignment | Balanced participation | Manipulative/speculative participation |

The cited Pokémon resale study documents market structure: liquidity, skew, and rarity premia.[3] NFT trader networks show concentration of activity consistent with a small set of accounts dominating turnover.[1]

## 2) Reinforcement Psychology: Reveal-Driven Dopamine Loops

Randomized monetization in games is empirically tied to gambling-like reward reactivity. In controlled experiments, rarer loot-box outcomes produce stronger arousal and urge to re-engage, with **anticipatory** arousal rising before the outcome is revealed.[2] Problem-gambling risk among young adults who play gacha-style games is analyzed in dedicated clinical-samples work.[7] Booster packs and loot-box lab tasks differ in medium and context; both still hinge on randomized reveal, while legal and diagnostic claims need their own evidence.

At a **population** level, systematic reviews in gambling studies summarize links between gambling disorder and income-generating offending in the papers they synthesize—forensic context that does **not** license equating casual gacha spend with crime.[53]

1.  **Anticipation:** acquisition of randomized exposure.
2.  **Activation:** reveal event drives acute arousal.
3.  **Resolution:** win reinforces repetition; dud encourages immediate retry.

### 2.1 Etymology, kompu gacha, and early Japanese policy

**Gacha** (ガチャ) takes its name from Japanese capsule-toy vending (_gashapon_): pay a fixed price, receive a random figurine. Free-to-play mobile games ported that **stochastic reward** template into currency-gated economies. **Complete / “kompu” gacha** pushed harder: buyers had to assemble specific randomly awarded parts to unlock a top prize, which created a combinatorial spend target. Japan’s Consumer Affairs Agency publishes official Q&A on internet transactions and “card matching” (カード合わせ) under the Act against Unjustifiable Premiums and Misleading Representations. That administrative spine treated kompu-style schemes as a **consumer-fairness issue** years before many Western debates framed loot boxes mainly as gambling law.[38]

### 2.2 Disclosure compliance, cross-regional RRM design, and pity economics

Empirical work now tests whether storefronts match their transparency promises. A PLOS ONE audit of top-grossing UK iPhone games reported substantial **non-compliance** with industry self-regulation on loot-box probability disclosure, which is evidence that “voluntary odds posting” is uneven in practice.[39] Entertainment Computing scholarship taxonomizes **random reward mechanisms** (RRMs) across China, the EU, Japan, and the U.S., coding hundreds of in-game implementations and showing both shared design templates and region-dependent packaging of pulls, currencies, and guarantees.[40] A randomized controlled trial on gacha monetization isolates a **behavioral triad** (unit price, pity (guaranteed-rare) systems, and luck beliefs) that jointly shapes payment intention; pity can reduce perceived risk while still elongating spend horizons.[41]

### 2.3 How gacha is programmed (open-source illustrations)

Live game servers are proprietary, but public codebases show the usual **engineering skeleton**: maintain a table of rewards with integer weights or rarity buckets; draw a uniform random variable; map it to a bucket; optionally increment **pity counters** on failure and force a high tier after a threshold. The TypeScript module `garug/gacha` implements configurable pools, rarity tiers, user inventory hooks, and pity-aware pulls, a compact illustration of how declared parameters shape pull distributions.[42] The `allemandi/gacha-engine` toolkit foregrounds **Monte Carlo** simulation: replay the same declared table thousands of times to estimate cumulative odds and pity breakpoints, making explicit that “fairness” is a design choice encoded in data structures.[43] Both repos document _mechanism types_ engineers reuse; commercial tuning stays outside the repos.

## 3) Utility Anchor Gap: Playability vs Programmed Scarcity

This section names a structural tension: **designed play utility** (what publishers and regulators can describe in rulebooks and terms) versus **speculative and aftermarket utility** (what markets price once scarcity, nostalgia, and social proof attach). The gap matters for psychology because the _same object_ can simultaneously be a game piece, a display collectible, and a liquid asset, with different mental accounts and time horizons depending on context.

### 3.1 Physical TCG: official “use” is play-shaped; markets add a second layer

The Pokémon Company publishes the TCG as a **rule-governed game**: the public rules hub defines how cards function in play, deck construction, and win conditions, and is the canonical entry point for sanctioned competitive formats.[36] Organized **Play! Pokémon** resources further specify which products and promos count as tournament-legal over time. That is a form of **administrative scarcity** distinct from print-run economics (bans, rotation, promo legality lists).[37] A separate Play! Pokémon terms layer governs participant conduct and program participation expectations.[35]

Official docs center play, programs, and IP rules. Independent market research treats Pokémon cards on eBay as a **secondary market** with heavy-tailed prices, strong liquidity for many SKUs, and rarity-linked premia in line with collectible-finance listing dynamics in that sample.[3] The utility anchor therefore **splits**: official channels anchor _legitimate competitive use_, while listing platforms anchor _clearing prices_. Friction (grading, shipping, authentication risk) is physical and procedural; resale usually leaves a usable object, while many tokenized projects lose utility when contracts or communities collapse.[6]

### 3.2 Digital objects, NFTs, and perceived permanence

Where the physical card remains a manipulable token with socially legible scarcity (print era, condition, grade), many NFT-linked artworks live inside a different psychology: consumers can perceive digital identity and value as **more fragile** than physical art despite on-chain persistence.[4] Security measurement work documents systemic **rug-pull** patterns: failures of the promised utility / governance layer that can strand holders even when a token technically still exists.[6] The “utility anchor” for digital collectibles is often **thinner**: provenance may be sharp, but the durable consumption experience (display, play, community) may be vendor- and platform-dependent.

Peer-reviewed work applies the **fraud triangle** (pressure, opportunity, rationalization) to NFT marketplace risk, situating rug-pull incentives in a psychology-of-fraud frame that complements—but does not replace—empirical counts of exploitative contracts and rug-pull projects.[54][6] Federal prosecutors charged OpenSea “insider” NFT trading as wire fraud; the Second Circuit **vacated** the conviction and remanded after finding erroneous jury instructions on what counts as wire fraud “property,” a boundary-setting appellate outcome rather than a moral verdict on every NFT trade.[55]

A contrasting **vendor narrative** targets collectors exhausted by retail queues, shipping friction, and authentication anxiety: **vault-and-mint** platforms take physical graded Pokémon cards into custody, issue cryptographically linked NFT receipts, and advertise insured storage plus programmatic redemption for the underlying slab.[45] Ecosystem blogging from a chain sponsor explicitly markets putting analog Pokémon inventory onchain as a modernization play.[44] That stack can feel **psychologically “safer” or cleaner** than camping big-box endcaps: ownership is legible in a wallet, transfers avoid postal risk each trade, and marketing stresses tamper-evident linkage over informal handoffs. Structural caveats remain: custodial concentration, smart-contract and bridge risk, and issuer solvency under vault branding; large-sample NFT security work on rug pulls and exploitative contracts remains salient even when the JPEG points at cardboard in a warehouse.[6] Consumer research likewise separates _blockchain persistence_ from _felt permanence_ of digital identity and value.[4] §8 summarizes the JACR experiments on essentialism and on preference when physical destruction is made salient.[4]

### 3.3 Randomized acquisition: parallel psychology, different regulatory frames

Booster-based TCG distribution shares a **family resemblance** with loot boxes and gacha: buyers pay for uncertain contents, and lab work ties rarer randomized outcomes to stronger anticipatory arousal and urge.[2] Clinical-samples research on gacha further motivates treating heavy engagement as a potential problem-gambling risk vector for vulnerable users in those clinical samples.[7] Regulators have interrogated loot-box-like designs as potential **games of chance** in specific jurisdictions; Belgium’s Gambling Commission published an influential analysis in that legal frame (English PDF).[11] Physical TCG packs share retail culture with digital loot products while following separate compliance rules. Here **programmed randomness** is a design fact with policy hooks. Section 2.2 adds **disclosure audits**, cross-regional RRM taxonomies, and pity economics on the quantitative side.[39][40][41] Section 2.1 notes Japan’s earlier administrative framing of exploitative complete-gacha schemes.[38]

### 3.4 What corporate “official” channels actually commit to

Official disclosures frame the collectible economy from a governance angle. The Pokémon Company’s published **Terms of Use** for Pokémon.com, apps, and related services (including Pokémon TCG Live) center intellectual-property control, acceptable use, and the limits of user claims on service content for digital participation.[34] The company’s **social impact** reporting supplies a complementary, voluntary narrative frame on corporate citizenship and programs.[15]

**Synthesis.** Official rules and terms describe _how to play and what licensors permit_; peer-reviewed work describes _how people respond to randomness and how markets clear_; regulator reports describe _where lawmakers see gambling-adjacent risk_. The “utility anchor gap” is the systematic mismatch between those layers. Collectors may price scarcity and status while rulebooks price match equity and card legality.[3][4][6][11][34][35][36][37]

## 4) Physical Market Pathologies: Scalping and Retail Friction

Major U.S. retail reporting documents acute friction around trading-card restocks: purchase limits, overnight camping, and in May 2021 a temporary halt to in-store sales at Target following safety incidents linked to demand for Pokémon and sports cards.[8] Business-news reporting from the same window ties one escalation to a Wisconsin parking-lot dispute (with a firearm drawn, no shots fired) and reproduces Target’s rationale for pulling cards from shelves.[17] That episode supports the claim that **early access** to shelf inventory became a contested resource; national scalping rates would need broader measurement.

Separately from lawful resale arbitrage, local reporting describes **retail theft** and **felony shoplifting charges** after alleged Pokémon card theft—documented enforcement at the property-crime layer, not proof that “flipping” is itself a crime.[59]

### Sealed packs: resealing, weighing, and secondary-market scams

Tampering does not require stealing inventory off the shelf: sellers can break factory seals, swap hits, and reclose blister or foil so buyers face **information asymmetry** about whether “sealed” still means factory-sealed. Reddit threads collect **informal visual tells** (crimp ridges vs flattened “melted” plastic, adhesive residue, alignment of back graphics)—useful community heuristics, not certification-grade authentication.[61] Hobby commerce writing similarly warns buyers to inspect seller photos and treat loose secondary-market packs as higher-risk than intact retail assortments.[64]

**Pack weighing** creates selection incentives: holographic cards can weigh slightly more than commons in hobby measurements,[62] and a single-author weighing experiment on Scarlet/Violet products reports that the heaviest packs in sampled boxes correlated with better pulls—non-peer-reviewed, but explicit about methodology limits.[63] That sits in tension with journalism arguing modern code-card counterweights make retail weighing unreliable,[62] and with above-board shelf purchasing where coverage already showed crowds competing for MSRP restocks rather than hidden chain-of-custody defects.[8][17]

Entertainment news documented a concrete **livestream controversy**: alleged resealed Pokémon packs sold on Whatnot, with coverage summarizing viewer accusations and on-camera reactions rather than a criminal verdict.[68] Separately, creator Shorts illustrate how foil can be reworked for reclosure—media about technique, not proof any listing you see is sound.[66][67] A long-form guide collates authentication cues for sealed items and singles for collectors evaluating listings.[65]

### Trade press, retailer social media, and user-generated corroboration (2021–2025)

Later coverage shows the problem persisting into premium-set rollouts: Polygon synthesizes GameStop employees’ photos and Reddit threads describing multi-day camping before high-demand Pokémon TCG SKUs, and points to an official GameStop post on X that presents long lines as part of store culture.[16][20][21] These sources follow trade-press and social rules: Reddit and X embeds are user- or brand-controlled narratives that outlets curate for story value. They still show how restocks feel on the ground in real time.

Games-media reporting also documents retailer experiments aimed at scalpers (for example, some Pokémon Center locations removing outer seals at purchase so “sealed box” resale is harder), while noting geographic limits to that tactic.[18] Entertainment-news pieces in 2025 summarized viral TikTok / X footage of a shoving match during a vending-machine restock, including participant comments about police contact; treat such pieces as **secondary journalism over UGC**.[19]

In early May 2026, trade reporting describes The Pokémon Company **scaling back** Pokémon TCG vending kiosks at some third-party retail locations. Polygon reproduces the gist of customer-facing notices (also collected in a Pokémon TCG subreddit megathread): kiosks are “gradually being removed from select retail locations” with aims to improve stock consistency and reliability for players.[22][24] The same article stresses that those notices **cite supply consistency**, while still cataloguing community reports of crowding, theft, fights, limit workarounds, and stores citing safety when pulling machines. Press and forums discuss those drivers even when notice text stays silent on them.[22] GoNintendo’s write-up parallels the official supply narrative and explicitly contrasts it with collector-side explanations emphasizing scalpers and unsafe scenes around kiosks.[23] Social screenshots of support emails may circulate faster than primary filings; treat them as **unverified unless matched** to publisher channels or reporting that independently confirms wording.

### Social signals: Target promo pins and parallel X discourse (May 2026)

A separate cluster of **user-generated signals** coalesced in early May 2026 around Target-issued Pokémon promotional pins (community-framed as in-store or campaign giveaways) appearing almost immediately on resale channels. Low-friction promos are often arbitraged; here the evidentiary value is **documentary**: listings and posts show asking prices and seller positioning; chains of custody and MSRP rules stay uneven across regions.

One seller-branded X account links to an eBay listing near **~$15** for a Target × Pokémon Squirtle pin SKU while packaging text visible in screenshots references a later online shop date: a concrete example of promo inventory being marketed on a secondary marketplace; unit-level sourcing stays unknown in the screenshots.[27][28] Another X post circulates screenshots implying **much higher** asks (e.g., $50+) for the same broad item class; the thread documents _ask dispersion and reactive memes_ around the drop.[33] Additional posts in the same timeline capture **opinion and venting** about reseller behavior around the drop.[29][30][31]

Adjacent **community-governance** friction also surfaces in the same window: long-time participants describe collector-oriented Discord or Facebook-adjacent spaces feeling dominated by resellers, while replies document members leaving over perceived toxicity. Treat the thread as sentiment and identity talk from participants.[26][25] Separately, a vending-focused X post alleges machine exploitation; it lacks retailer or legal primary sources in this map.[32] (Screenshots of Facebook groups charging for “skip approval” posting illustrate the same theme (monetized queue access), but we omit them here until permalinked primary URLs are added to the reference map.)

NFT rug pulls can strand holders after funds move and teams vanish.[6] Physical cards usually keep object-level value through resale churn; friction then concentrates in access and price.

### Scalping methodologies observed in the current cycle

The following table mixes (A) tactics consistent with wire-style and business reporting around Target’s 2021 pullback[8][17], (B) recurring camping/line narratives in games trade press and Reddit/X chains[16][20][21], and (C) vending-machine conflict described via entertainment news over viral video.[19], and (D) reported **kiosk phase-outs** in 2026 trade coverage with explicit separation of official messaging vs community safety/scalper narratives.[22][23][24], and (E) May 2026 **Target pin / resale** and related X threads as documentary social signals (listings plus opinion with unverified sourcing).[25][26][27][28][29][30][31][32][33] The stack grounds the case study in publicly accessible, citable URLs ahead of any peer-reviewed prevalence work. Rows marked _anecdotal_ remain hypotheses where only informal reports exist.

| Methodology | Operational tactic | Primary market effect |
| --- | --- | --- |
| Restock interception | Queueing/camping before open, first-to-shelf races, rapid cart clearing at release windows | Shelf depletion at MSRP before normal buyers can access product |
| Inventory intelligence networks | Group chats, tip-offs, and route-tracking of merchandiser schedules | Predictive capture of supply before public availability |
| Purchase-limit circumvention | Multi-person proxy buying, repeated checkout loops, and split-transaction behavior | De facto nullification of anti-hoarding controls |
| Vending kiosks _(conflict + reported phase-out)_ | Race to limited restocks; UGC and trade summaries of disputes;[19] plus 2026 reporting on gradual removal of select Pokémon TCG vending machines with supply/consistency rationale in notices and scalping/safety context in adjacent coverage.[22][23][24] | Fewer fixed retail touchpoints for MSRP-adjacent buying; continued reliance on online and other channels |
| Retail-to-secondary arbitrage | Immediate relisting at large markups across marketplaces and live-stream channels | Price floor inflation and reduced entry accessibility for hobby-first participants |

If marginal buyers face resale markups, total cost of participation rises even when cards stay available on secondary markets. The eBay Pokémon study quantifies heavy-tailed prices and fast turnover for certain sets,[3] with scarcity-driven premia; the listing metadata omit scalper self-labels.

### Countermeasure matrix for scalping control

**Design note.** This matrix lists practical controls from retail and marketplace policy debates; cite a specific evaluation whenever you claim results from a randomized trial.

| Scalping method | Retailer controls | Platform/marketplace controls | Policy and enforcement controls |
| --- | --- | --- | --- |
| Restock interception | Randomized release windows, ticketed queue systems, and per-customer daily hard caps | Time-delayed listing for freshly released SKU classes and repeated SKU-velocity flags | Store-level anti-harassment enforcement and incident-report escalation protocols |
| Inventory intelligence networks | Route obfuscation for restocks, confidential logistics windows, and internal access logging | Risk scoring for coordinated seller clusters with synchronized listing behavior | Employer sanctions for paid tip-offs and conflict-of-interest retail policies |
| Purchase-limit circumvention | Identity-linked limits (phone/payment/loyalty), cooldown windows, and duplicate transaction detection | Cross-account linkage checks for near-identical listing metadata and payout destinations | Consumer-protection audits of anti-hoarding compliance for large retail chains |
| Vending-channel exploitation | Tamper-resistant interfaces, signed firmware, and remote anomaly alerts on velocity spikes | Flag-and-hold workflows when inventory drains map to immediate high-volume relists | Computer misuse referral paths where exploit behavior breaches device-access laws |
| Retail-to-secondary arbitrage | MSRP-protected bundle allocation for local buyers and verified hobby loyalty tiers | Markup transparency labels and repeat markup-abuse monitoring for high-frequency sellers | Targeted unfair-trade enforcement for deceptive scarcity claims and collusive resale conduct |

The intervention logic is layered: retailer controls reduce first-capture probability, marketplace controls reduce immediate monetization efficiency, and policy controls raise the expected cost of organized abuse. Whether a given lever works in practice is context-specific and should be evaluated with operational data.

## 5) Digital Pathologies: Rug Pulls, Whale Concentration, and Casino Dynamics

In a large trader-network study of early NFT markets, the authors report that the top 10% of traders perform about 85% of all transactions and touch the vast majority of assets at least once.[1] Independent security measurement work identifies thousands of NFT rug-pull projects and reports that a large majority of analyzed rug-pull contracts exhibit exploitative contract patterns (e.g., privileged “backdoor”-style logic).[6] These findings describe on-chain fraud and concentration in the cited NFT samples. Agency announcements add the enforcement layer: IRS Criminal Investigation publicized federal **charges** in the Frosties NFT matter,[56] and ICE announced a federal **indictment** in the Undead Apes / Undead Tombstone Solana NFT scheme (charging documents state **allegations** until proven otherwise).[57] Appellate law on wire fraud “property” in NFT-market prosecutions remains salient after the Second Circuit **vacated** convictions in _United States v. Chastain_ and remanded for a new trial on that theory.[55]

| Market | Inequality Pattern | Resilience Implication |
| --- | --- | --- |
| Pokémon TCG (eBay resale study) | Heavy-tailed prices (mean above median); high listing success rate; rarity commands multiplicative premia[3] | Broad liquidity for listings in sample; global holder-wealth inequality is outside the design |
| NFTs (on-chain trader network, 2017–2021 window) | Extreme concentration of _transaction activity_ among top-decile traders[1] | Market depth can be sensitive to activity of highly active accounts |

## 6) Psychographic Segmentation and Dark-Trait Correlates

Labels like **hobbyist**, **flipper**, or **hybrid participant** are _heuristic personas_ for discussion here. **Cryptocurrency panels** (§6.1–6.3) sit next to **literature on physical collectibles, CCG booster spending, and speculator–collector communities** (§6.4), which tracks TCG economies more closely. Flipper-adjacent claims draw on **investment-motivated collectors**, **community studies of speculators**, and §4’s documentary social posts as context. Cross-market links stay **hypothesis-generating** until Pokémon-stratified psychometrics land.

### 6.1 National U.S. survey: who has owned cryptocurrency? [5]

Littrell, Klofstad, and Uscinski report a demographically weighted Qualtrics panel of **2,001 U.S. adults** (May–June 2022) in which **29.8%** answered yes to ever owning cryptocurrency. The authors stress **cross-sectional associations** only. At the bivariate level, ownership correlates with higher conspiracy-style thinking and endorsement counts, higher scores on narcissism, Machiavellianism, psychopathy, and sadism scales, greater use of alternative social media for political news, and a mix of other political and behavioral measures they visualize at length. In a comprehensive multivariate logistic model, the strongest positive predictor of ownership is **reliance on alternative/fringe social media** for news about politics and public issues. **Male respondents** show substantially higher odds of reporting ownership than female respondents after the authors include the selected covariates. Ownership is also predicted positively by **argumentativeness**, **higher income**, and **religiosity**, and **negatively** by both **right- and left-wing authoritarianism scales** in that full specification. Conspiracy belief count is only a marginal predictor once other covariates enter. “Crypto owner” in Littrell et al. means **ever-ownership in 2022**; trading intensity, wallet size, and Pokémon behavior fall outside that item.[5]

### 6.2 Mechanistic survey: Dark Tetrad pathways to attitudes and buying intention [9]

Martin and colleagues analyze a **pre-registered** sample of **N = 566** respondents with **stated interest in cryptocurrency**, a different recruitment frame from the national ever-ownership study in §6.1. Structural-equation models link Dark Tetrad traits to cryptocurrency **attitudes** and **buying intention** through three mediators: **conspiracy beliefs**, **FoMO**, and **positivity**. The paper emphasizes **trait-specific pathways** (e.g., narcissism vs Machiavellianism vs psychopathy vs sadism). Outcomes are **self-reported intentions**. The authors caution against stereotyping all cryptocurrency users; we repeat that caution here.

### 6.3 Early adopters: overconfidence and self-control [10]

Sudzina, Dobes, and Pavlicek model **cryptocurrency use** with **binary logistic regression** on an early-adopter-framed sample. They discuss **overconfidence** in relation to Big Five patterns, specifically **higher extraversion and lower agreeableness**, consistent with literature linking those traits to overconfidence biases. For **self-control**, they depart from standard impulse-control scales and instead use a **proxy tied to respondents’ self-reported experience with categories of cybercrime victimization**, interpreting the pattern within their framework as evidence about self-regulation. **Men** in their models report substantially higher odds of cryptocurrency use than women (on the order of **three times** the odds in their published specification). These design choices mean the self-control result tracks the paper’s cybercrime-victimization proxy; clinical compulsivity batteries use different instruments.

### 6.4 Physical collectibles & CCGs: verifiable “flipper-adjacent” psychology

The **methods and psychologies** in journal work on physical collectibles diverge from the crypto surveys above: fewer political-fringe-media batteries; more emphasis on **investment vs consumption motives**, **community-level conflict with resellers**, and **gambling-symptom links to randomized packs** tested with player-reported spend.

**Booster spend and problem gambling.** Zendle and colleagues surveyed **726 collectible card game players**, testing whether people with stronger problem-gambling symptoms spend more on sealed booster packs. They report **no statistically significant** association for in-store physical booster spending and problem gambling, and only a **trivial-magnitude** link for online booster spending, with equivalence tests arguing effects sit below practical importance at pre-registered thresholds. For **policy analogies to loot boxes**, the CCG evidence is **softer** than typical loot-box harm studies, so blunt “TCG flippers = gambling addicts” mappings lack support here.[48]

**Investor-oriented collectors vs pure hobbyists.** Kleine, Peschke, and Wagner partition self-identified collectors into consumption-, investment-, and “pure” collecting motives in a large European survey (**n ≈ 4,042**, including **1,601** collectible owners). “Investor” collectors score lower on **Agreeableness** and **Conscientiousness**, framed as a more competitive, spontaneous profile, whereas “pure” collectors show **higher Conscientiousness** and more systematic goal pursuit. Consumption-oriented collectors largely resemble non-collectors except for higher Openness. This is the closest peer-reviewed analogue on this page to a **profit-oriented resale identity** through Big Five motives; Dark Tetrad batteries and Pokémon SKU revenue fields sit outside that survey.[49]

**Speculators inside collector brand communities.** Hass and colleagues use mixed methods (survey + Reddit content analysis) in a **Squishmallow** collector community to theorize how **third-party speculators** inflate prices, gatekeep primary supply, and generate emotional pain, while paradoxically fueling continued community engagement as members reinterpret frustration as shared struggle. The introduction cites **Pokémon card** resale conflicts; the empirical work stays in a **Squishmallow** community as a **meso-level model of collector–speculator tension**.[50]

**Self-reported “addiction” and subclinical scores.** Calvo and colleagues study players of Star Wars universe collectible card games, miniatures, and dice (**n = 218**). Dissociation-oriented motives and lower self-esteem predict variance on a short internet-gaming-disorder screen, yet **no respondent exceeded the authors’ tentative clinical cut-off**; many describe economic or family strain while still falling below the authors’ tentative clinical cut-off, keeping most scores in a subclinical band.[51]

**Evidence stack (crypto vs TCG-adjacent).** Littrell et al. tie ever owning tokens to **fringe information diets, conspiracy receptivity, and elevated dark-trait scales** in a 2022 U.S. panel.[5] Martin et al. route Dark Tetrad traits into crypto **intention** through FoMO, conspiracy beliefs, and positivity in a niche sample.[9] Collectible-economy papers add **Big-Five investment profiles**,[49] **muted booster–problem-gambling links in Zendle et al. relative to loot-box literatures**,[48] and **community-level pain from speculators** in Hass et al.[50] FoMO also shows up in compulsive retail behaviors,[46][47] so scarcity hype can echo across both stacks while the citations stay separate.

### 6.5 FoMO, compulsive buying, and conceptual links to scarcity retail

Independent of crypto, marketing and consumer research ties **FoMO** to **compulsive buying behaviors**, including pathways through mood and materialism in a 569-adult SEM sample.[46] A systematic review maps how FoMO connects to conformity-, bandwagon-, and conspicuous-consumption patterns in marketing contexts.[47] Together with FoMO’s role as a mediator in the Dark Tetrad / cryptocurrency intention study,[9] the same FoMO construct lines up with reactions to time-boxed retail drops and “must buy now” social feeds. This map lacks FoMO surveys tied to Target lines or vending queues. Clinical-samples work on **gacha** engagement and problem-gambling risk supplies a parallel vulnerability literature for digital random rewards among sampled gacha players.[7]

### 6.6 Evidence gaps and ethics of inference

Even after adding CCG and collectible-investor sources, the map still lacks: representative psychometrics of **self-identified Pokémon TCG scalpers**; longitudinal links from personality to **observed flipper revenue**; and field experiments on how purchase limits or queue designs change behavior. Aggregated associations, whether from crypto panels[5][9] or investor-motivated collector surveys,[49] support group summaries only; extending them to named individuals requires an **ecological fallacy** check. Policy and moderation can track **population-level risk factors** while avoiding blanket blame on individuals.

### 6.7 Toward psychometrics of self-identified Pokémon TCG resellers

This subsection is a protocol sketch for closing the §6.6 gap with auditable methods. Recent Pokémon-specific marketplace work tracks listing survival and revenue on eBay without measuring seller traits or motives, which shows the split between **transaction physics** and **participant psychology**.[52]

**Eligibility and strata.** Recruit adults who report past-90-day Pokémon TCG resale activity on at least one platform (eBay, Mercari, in-person, etc.). Use a two-step identity item: (1) “Do you sell Pokémon cards mainly to fund the hobby, mainly for profit, or about equally?” (2) optional checkbox **self-label** (“reseller / flipper / scalper” language varies by community; capture exact wording and discomfort with the label). Compare against a **hobby-primary control** arm matched on age/region with negligible resale revenue. Pre-register exclusion rules (e.g., professional shop employees) before data collection.

**Core construct battery (map to existing literature on this page).** Administer short, validated scales where possible: **Big Five** (to test whether “investor” low Agreeableness / Conscientiousness patterns replicate Kleine et al. within a Pokémon-only resale stratum)[49]; **FoMO** and **compulsive buying** screens tied to scarcity retail theory[46][47]; optional **Dark Tetrad** short form for symmetry with crypto intention work (interpret cautiously; avoid stigmatizing reporting)[9]; **problem-gambling symptomology** (e.g., PGSI) to relate resale intensity to the CCG booster findings in Zendle et al.[48] Add behavioral covariates: estimated monthly resale gross, hours spent sourcing, use of inventory bots/trackers, and participation in Discord/X tip networks as covariates alongside trait scores.

**Design choices.** Prefer **between-subjects contrasts** (profit-primary vs hobby-primary) plus latent-profile mixture models over a single “scalper score.” Report measurement invariance across gender and region. Link self-report to **platform metrics** where API or screenshot consent allows (e.g., seller rating counts) to reduce social-desirability bias on profit motives.

**Ethics.** Communities already moralize resellers; debrief participants, allow withdrawal, and aggregate findings so individuals cannot be doxxed. Use neutral wording in instruments (“profit-primary seller” vs pejoratives). Pre-registration (OSF/AsPredicted) should lock hypotheses before recruitment to prevent post-hoc pathologizing.

**Interim use of this page.** Until such a study exists, treat §6.1–6.5 as a **stack of proxies**: crypto panels for digital-asset psychology[5][9][10], general FoMO/compulsive buying[46][47], CCG booster–gambling links[48], investor Big Five in broad collectibles,[49] and speculator–community dynamics in adjacent toy markets.[50] A Pokémon-stratified psychometric battery would still add precision beyond that stack.

**Construct routing (selected).** The table ties each psychological theme to where it is measured in this bibliography and how it relates to physical-collectible discourse on this page.

| Construct / theme | Where measured (this page) | Relevance to collectibles narrative |
| --- | --- | --- |
| Ever cryptocurrency ownership (U.S. national) | Littrell et al. survey, 2022 fielding[5] | **Analog** U.S. panel for anti-establishment media use, conspiracy receptivity, and dark-trait scales; Pokémon strata absent. |
| Dark Tetrad → intention (FoMO, conspiracy, positivity) | Martin et al. crypto-interested SEM[9] | **Analog** mechanism for how scarcity hype and ideology might route into pay intention via survey items only. |
| Overconfidence / self-control proxies | Sudzina et al. logistic models[10] | **Analog** early-user profile; self-control operationalization is nonstandard; see §6.3. |
| FoMO → compulsive buying; FoMO in marketing SLR | Hussain et al.; Alfina et al.[46][47] | **Direct** consumer-psychology foundation for scarcity/FoMO language around drops in general-adult samples. |
| Problem-gambling risk in gacha contexts | Clinical-samples framing[7] | **Partial parallel** for digital random-reward harm reduction among gacha clinical samples. |
| CCG booster spend vs problem gambling symptoms | Zendle et al., CCG player survey[48] | **Direct** to sealed-pack economies; null/trivial links under the paper’s tests. |
| Investor- vs consumption-oriented collector Big Five | Kleine et al.[49] | **Direct** to resale/investment motive in a broad European collector panel; flipper-adjacent Big Five read. |
| Collector–speculator community pain / paradox | Hass et al. (collectible toy community)[50] | **Analog** meso dynamics from a Squishmallow community with Pokémon cited only in framing. |
| CCG hobby “addiction” self-concept vs clinical cut-offs | Calvo et al. (Star Wars universe tabletop/CCG)[51] | **Direct** to tabletop CCG culture; subclinical pattern cautions against over-pathologizing. |
| Empirical “scalper psychology” profile | Not yet measured (§6.7 protocol) | **Gap**: stratified psychometrics still in protocol form (§6.7); §4 social signals stay documentary for now. |
| Pokémon listing survival / revenue (no seller psych) | Heck et al., eBay field study Germany[52] | **Market layer only**; Pokémon listing survival and revenue; personality covariates still open. |

## 7) Gacha, Rip-and-Ship, and the “Unregulated Casino” Problem

Loot boxes and gacha monetization parallel gambling-like reward structures in experimental psychophysiology work on anticipation and arousal.[2] Clinical-samples research discusses problem-gambling risk among young adults engaged with gacha games.[7] On policy, Belgium’s Gambling Commission has published analysis concluding that certain paid loot-box models meet legal elements of games of chance under Belgian law; other jurisdictions need their own legal read.[11] News reporting describes renewed legislative attention to gacha regulation in South Korea.[12] Japan’s Consumer Affairs Agency materials on **card-matching** monetization anchor an earlier regulatory chapter that is easy to overlook in Anglophone loot-box debates.[38]

The same gambling-adjacent design conversation sits beside **population-level** reviews linking gambling disorder to offending patterns in synthesized studies—not a claim that every gacha player offends.[53] Belgian **civil** litigation has produced a CJEU referral on loot boxes and app-store liability, parallel to administrative gambling-commission analysis but distinct from a U.S. criminal trial.[58][11] Federal **indictments** in alleged Solana NFT rug-pull schemes illustrate how prosecutors frame quick-exit liquidity narratives; those filings allege facts for court, not proof for this essay’s psychology claims.[57]

Storefront odds claims still miss often: empirical audits find uneven compliance with probability-disclosure norms,[39] while comparative scholarship maps how studios encode random reward mechanisms differently by region.[40] Behavioral experiments show pity systems and pricing jointly steer spend, complicating simple “guarantees protect players” stories.[41] Open repositories such as `garug/gacha` and `allemandi/gacha-engine` make the implementation pattern (weighted tables, RNG draws, pity counters) inspectable for pedagogy only.[42][43]

Live-stream **rip-and-ship** and vaulted **phygital** rails sit adjacent to this psychology: both convert cardboard variance into spectator or wallet-native liquidity. Commentary on opening Pokémon packs onchain sketches that business model.[13] Vault platforms and chain blogs pitch NFT receipts as a frictionless alternative to physical arbitrage for graded Pokémon inventory, which can feel safer than door-crashing retail, though custody and contract risk remain.[45][44][6][4]

## 8) Art Psychology: Essentialism and Permanence Threat

The studies cited here are lab work on how people judge **one-of-a-kind art** on canvas versus NFT-linked forms.[4] Scope covers art-judgment tasks; Pokémon listings and graded-card markets need other instruments.

### 8.1 Essentialism, permanence, and artistic identity

**Psychological essentialism** in this context means treating a work as if it holds something fixed about the maker. People read **artistic identity** off the object. Finken et al. argue that how **enduring** the **carrier** seems (canvas versus NFT-linked uniqueness) feeds that reading.[4]

### 8.2 Baseline: NFT-linked art seen as less permanent, canvas preferred

In **four experiments** and **three replications**, one-of-a-kind NFT-linked works were often rated **less permanent** than on-canvas work. Lower permanence went together with a **weaker sense** that the piece carried the artist’s essential identity, matching stronger baseline **preference for canvas over NFT** in their designs.[4] The outcomes are controlled ratings and choices inside those designs.

### 8.3 Threatened permanence: when digital preservation reframes value

When the materials stressed that the physical work could be ruined on purpose or by accident, respondents could see NFT-linked forms as **better at preserving value** and **tilt preference** toward the digital option versus the baseline.[4] The stimuli are fine-art vignettes; _fragility_ in the story shifts which carrier feels tied to identity.

### 8.4 Collectibles context and limits

Slabs, wallet receipts, and gallery pieces differ in tangibility, who holds custody (vault, bridge, issuer), and what signals “real.” §3.2 sets NFT permanence beliefs next to rug pulls and platform failure;[6] §7 notes vault and phygital pitches that stress convenience over door-crashing retail.[44][45] Art-stimulus results[4] stop at perception; Pokémon **hold times**, **price levels**, and **liquidity** need trade-level and category-specific studies.

## 9) Strategic Generosity and Reputation Penalties

Peer-reviewed information-systems work reports reputational and pricing consequences when NFT charity fundraisers are perceived as strategically relisting donated items for profit (including a reported portfolio-level price penalty in their empirical setting).[14] Separately, The Pokémon Company’s public social-impact reporting documents corporate giving and governance structures. On-chain “strategic generosity” penalties sit outside that disclosure set.[15]

As a **distant enforcement analog** only: federal mail- and wire-fraud **indictments** in a veterans nonprofit matter (per contemporaneous news on the charging instrument) show how misrepresented charitable use of funds can trigger criminal process—without implying that participants in the NFT charity relisting study were prosecuted or that the schemes are legally equivalent.[14][60]

## Conclusion

In short: physical resale markets can remain liquid while exhibiting rarity-driven heavy tails[3]; NFT markets can simultaneously concentrate trading activity[1] and facilitate large-scale contract-based fraud patterns[6]; randomized digital monetization engages anticipatory reward processes similar to those studied in loot-box experiments[2]; and crypto participation correlates with measurable psychological constructs in survey research[5][9][10][46][47]; complementary CCG and physical-collectible studies document different effect sizes for booster spend vs gambling symptoms, Big-Five splits between investor- and hobby-oriented collectors, and meso-level speculator conflicts in communities.[48][49][50][51] Pokémon listing dynamics on eBay are now described prospectively in one national field study; seller psychometrics are still absent there, which §6.7-style protocols target.[52] Tampered sealed inventory illustrates the same **promise-vs-delivery** gap measured for exploitative NFT contracts in large-sample security work.[6] Policy and design can ground consumer protection (e.g., transparency, harm minimization) in cited evidence while judging individual conduct on its own facts. Gacha and loot economies increasingly face **empirical scrutiny** on disclosure and mechanism design,[39][40][41] while tokenized vault narratives emphasize perceived safety even though contract and custody risk remain.[44][45][6]

**Limitations.** This page cites primary sources in narrative form; preregistered meta-analysis standards apply only when we cite a study that used them. Claims point to the closest matching citation we name, with weak or anecdotal evidence labeled when it appears.

\## References and source credits See \[references.json\](../references/references.json) for the canonical bibliography (68 sources).