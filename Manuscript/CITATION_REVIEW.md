# Citation review — Digital Organizational Resilience manuscript

Inventory taken from `Manuscript/sections/*.tex` + `Manuscript/main.tex`.
**722 citation instances, 155 unique keys.** Target: 70–80 unique keys → cut ~75–85.

| Section | Unique refs | Instances |
|---|---:|---:|
| 1_introduction | 21 | 27 |
| 2_background | 87 | 174 |
| 3_research_gaps | 47 | 88 |
| 4_enactment-scope | 41 | 79 |
| 5_research_directions | 73 | 208 |
| 6_implications | 42 | 62 |
| 7_conclusion | 5 | 5 |
| 12_appendices | 59 | 79 |

Top-15 most-cited keys:

| count | key |
|---:|---|
| 31 | rota2024 |
| 30 | duchek2019organizational |
| 20 | gillard2023efficient |
| 19 | skopik2016problem |
| 17 | bcbs2021operational |
| 17 | boin2013resilient |
| 17 | woods2015four |
| 17 | francis2014metric |
| 15 | bhamra2011resilience |
| 15 | linkov2013resilience |
| 14 | weick2011managing |
| 13 | european2022regulation |
| 13 | kuypers2018designing |
| 12 | calder2021iso |
| 12 | ecb2018tiber |

Distribution: 52 refs cited once, 28 cited twice, 15 cited three times — the long tail is large.

---

## 1. Citation positioning issues (claim vs. source mismatch)

Ordered roughly by severity. File:line points to the location of the `\autocite`.

### 1.1 — Likely mispositioned

| # | Location | Claim being supported | Cited key(s) | Problem | Suggested fix |
|---|---|---|---|---|---|
| A1 | [1_introduction.tex:9](sections/1_introduction.tex#L9) | "resilience has become a central regulatory priority" | `heinimann2017infrastructure` | The cited chapter is about infrastructure resilience assessment; it does not establish the regulatory-priority claim. | Use `bcbs2021operational` or `european2022regulation` (already in bib) — they *are* the regulatory record. |
| A2 | [1_introduction.tex:5](sections/1_introduction.tex#L5) | "the threat environment has continued to accelerate dramatically" | `arif2024overview` | Arif et al. is a generic AI-cyberthreat overview — a thin anchor for an "acceleration" claim. | Either cut the citation (the journalistic `smith2026mythos` already covers it three sentences earlier) or pair with `hausken2020cyber`/`falco2019cyber`. |
| A3 | [5_research_directions.tex:16](sections/5_research_directions.tex#L16) | "cross-jurisdictional reporting converges" (macro institutional indicators) | `meerow2016defining`, `allen2018quantifying` (urban + ecological) | Both are about non-organizational, non-regulatory domains. They don't speak to cross-jurisdictional regulatory reporting. | Drop both from this cluster; `nist2024csf`, `bcbs2021operational`, `european2022regulation` alone do the work. |
| A4 | [5_research_directions.tex:26](sections/5_research_directions.tex#L26) | "ISAC membership, shared standards, or platform interoperability translate into cooperative response" | `mahajan2022participatory` | Mahajan et al. is about *participatory urban resilience planning*, not ISACs or cyber info-sharing. | Replace with `arnold2004informationsharing` or `lostri2022shared` (already in bib). |
| A5 | [5_research_directions.tex:50](sections/5_research_directions.tex#L50) | "warning systems and incentive structures … for cross-firm cooperation" | `brauer2008compartmental` | Brauer is a chapter on compartmental SIR epidemic models — irrelevant to cyber sharing incentives. | Drop; the same line already cites `maillart2017bugbounty`, `arnold2004informationsharing`, `mermoud2019share`. |
| A6 | [5_research_directions.tex:30](sections/5_research_directions.tex#L30) | "ML pipelines embedded in explainable AI (XAI) … rationalizing high-dimensional trace data" | `rane2024artificial` | Rane et al. is a high-level AI-for-resilience overview, not an XAI-for-security source. | Drop `rane2024artificial` (singleton elsewhere); `gillard2023efficient` already anchors the cyber-ML claim. |
| A7 | [6_implications_for_research.tex:11](sections/6_implications_for_research.tex#L11) | indicators: "coordination speed, stakeholder support, community ties, capacity to reconfigure infrastructures, variation in response under stress" | `mayer2021putting` | Mayer & Roche is about purpose/mutuality economics; the indicators listed don't come from it. | Drop; `paries2017resilience` + `gillard2023efficient` already cover the indicator catalogue. |
| A8 | [6_implications_for_research.tex:17](sections/6_implications_for_research.tex#L17) | "design principles, benchmarks, early-warning systems, and governance mechanisms" | `lengnick2011developing` | Lengnick-Hall et al. is HR-focused "capacity for resilience" — light on benchmarks/EWS. | Drop here (Lengnick already cited ~6× elsewhere); `calder2021iso`, `bcbs2021operational`, `finma2023operational`, `nist2024csf` are the right anchors. |
| A9 | [5_research_directions.tex:54](sections/5_research_directions.tex#L54) | "closing the gap between articulated commitment and observable adaptive performance under persistent uncertainty" | `kalisch2024neurobiology` | Kalisch is a *neurobiology of stress* review — only loosely related to organizational measurement. | Drop; `aerts2018integrating`/`gillard2023efficient` carry the claim. |
| A10 | [2_background.tex:27](sections/2_background.tex#L27) | "disruptions frequently cascade across spatial, temporal, and governance levels" | `moreno2018womens` | Moreno et al. is on women's vulnerability in disasters — not the cited cross-scale cascade claim. | Replace with `aerts2018integrating` or simply drop; `liu2022network` (cited nearby) carries the cascade point. |

### 1.2 — Less severe, but worth tightening

| # | Location | Issue |
|---|---|---|
| B1 | [1_introduction.tex:11](sections/1_introduction.tex#L11) | `rota2024` cited *twice* inside the same six-theme list. Only the introductory mention is needed. |
| B2 | [3_research_gaps.tex:13](sections/3_research_gaps.tex#L13) | `duchek2019organizational` cited for "definitional drift" — the broader argument is already established. Could swap with `hillmann2021organizational` (which is *about* definitional pluralism) to vary the workload. |
| B3 | [2_background.tex:46](sections/2_background.tex#L46) | "Decentralized structures … quicker local responses" anchored only with `boin2013resilient`. Pair with `bhamra2011resilience` (already cited heavily) so the load distributes; or rely on `galbraith1973designing` (cited L46 of section 5 only once — under-used). |
| B4 | [4_enactment–scope.tex:26](sections/4_enactment–scope.tex#L26) | Three back-to-back nine-cell cite clusters total ~30 cite-instances. Each cell ends in a "concrete-evidence" cluster; some inputs (`mahajan2022participatory`, `ibnehossain2020modeling`) are weak fits — see §3 below. |
| B5 | [5_research_directions.tex:38](sections/5_research_directions.tex#L38) | Long simulation paragraph cites `folke2004regime`, `walker2004resilience`, `holling1973resilience` repeatedly in a non-ecological context. They are correct sources for "regime shift" framing but the section is about cyber/SOC modelling — risks reading as theory-shopping. Consider keeping one (e.g. `walker2004resilience`) and dropping the other two from this paragraph. |

---

## 2. Over-cited references — rebalancing proposals

For each, the proposal lists **existing** bib substitutes first; new-ref suggestions appear only where the existing pool is thin.

### 2.1 — `rota2024` (31 instances)

Used both for the field-study evidence (correct) and as a *referent* to the appendix (often redundant). The thesis is the same source whether you cite it once per section or once per claim.

**Recommendation:** keep ≤ 12 uses. Concrete cuts:
- Drop the second occurrence in [1_introduction.tex:11](sections/1_introduction.tex#L11) (already cited once in the same sentence).
- In `5_research_directions.tex` it appears 6× — keep one per subsection (theory / measurement / governance), drop the rest.
- In `3_research_gaps.tex` it appears 4× — keep one anchoring citation; the appendix already records the field study.

No substitute needed — the goal is fewer self-references to the same source.

### 2.2 — `duchek2019organizational` (30 instances)

Used for: (i) dynamic-capability framing, (ii) sense–reconfigure language, (iii) generic "preparedness ≠ adaptation" claims, (iv) "definitional drift".

**Proposed rotation using existing bib:**

| context | currently | alternative already in bib |
|---|---|---|
| sense / reconfigure | `teece2007explicating, duchek2019organizational` | `teece2007explicating` + `lengnick2011developing` |
| preparedness vs. adaptation | `duchek2019organizational, woods2015four` | `woods2015four` alone, or `hillmann2021organizational` |
| definitional drift | `duchek2019organizational` | `hillmann2021organizational` (specifically *about* this) |
| HRO/mindfulness | `duchek2019organizational, weick2011managing` | `weick2011managing, vogus2007organizational` |

Target: keep ≤ 12 uses.

### 2.3 — `gillard2023efficient` (20 instances)

Self-citation, often used as a generic anchor at the end of clusters. Several uses are placeholders rather than evidence (e.g. closing a paragraph on indicators with "…and `gillard2023efficient`").

**Recommendation:** keep ≤ 8 uses where it specifically anchors *cooperative cyber-defence quantification*. Cuts:
- [5_research_directions.tex:30](sections/5_research_directions.tex#L30) (XAI claim — drop, see A6)
- [5_research_directions.tex:48](sections/5_research_directions.tex#L48) (end of governance cluster — drop)
- [5_research_directions.tex:54](sections/5_research_directions.tex#L54) (closing line — drop)
- [6_implications_for_research.tex:5](sections/6_implications_for_research.tex#L5) and [6_implications_for_research.tex:17](sections/6_implications_for_research.tex#L17): keep one.

No substitute needed (drops, not swaps).

### 2.4 — `skopik2016problem` (19 instances) and `francis2014metric` (17 instances)

Both reasonable anchors but appearing as "and finally…" tail-end citations in long clusters. Trim by removing tail occurrences where the lead citation already covers the claim. Target: each ≤ 10.

### 2.5 — `woods2015four` (17 instances)

Central to the "preparedness ≠ adaptation" thread, which is *the* paper's argument — this density is defensible. Keep ~10–12.

### 2.6 — `bcbs2021operational` (17×), `boin2013resilient` (17×), `bhamra2011resilience` (15×), `linkov2013resilience` (15×), `weick2011managing` (14×)

All appropriately central to the field. Trim only where they're part of 4+ citation clusters that overlap (see §3).

---

## 3. Dense citation clusters (≥ 4 keys at one site)

These clusters dilute the support for each claim and inflate the count without strengthening the argument. Each row proposes a trimmed version.

| Location | Current (count) | Proposed keep | Drop reason |
|---|---|---|---|
| [2_background.tex:5](sections/2_background.tex#L5) | `hillmann2021organizational, woods2015four` (2) | both | OK as-is |
| [2_background.tex:12](sections/2_background.tex#L12) | `rankine1858manual, panteli2017metrics, wiener1948cybernetics` (3) | `rankine1858manual, wiener1948cybernetics` | `panteli2017metrics` is a 2017 power-grid metrics paper — wrong era for "earliest foundations". Move it to where it actually applies (used 4× elsewhere correctly). |
| [2_background.tex:15](sections/2_background.tex#L15) | `walker2004resilience, folke2004regime, folke2010resilience` (3) | `folke2010resilience` alone (already covers the panarchy/regime synthesis) | Two of three are tightly overlapping. |
| [2_background.tex:21](sections/2_background.tex#L21) | `masten2010disasters, feder2019biology, mcewen2004protection` (3) | `feder2019biology` | Reviews same neurobiological mechanisms; one is enough at this level of generality. |
| [2_background.tex:27](sections/2_background.tex#L27) | 14 keys across one paragraph | keep `levin1998ecosystems, gao2016universal, albert2000error, berkes1998linking, adger2005socialecological` (5) | Drop `sornette2014how, maillart2019aristotle, krakovska2023resilience, klein2015wikipedia, bodin2009role, moreno2018womens, sornette2013exploring, aase2020resilience, leichenko2024climate` from this site. Most reappear elsewhere or are singletons that decorate without anchoring. |
| [2_background.tex:40](sections/2_background.tex#L40) | cites `bhamra2011resilience, weick2011managing` then again `teece2007explicating, duchek2019organizational` then `calder2021iso, european2022regulation, linkov2013resilience` (7) | structure as three short citations (one per claim) rather than three triples |
| [2_background.tex:62](sections/2_background.tex#L62) | 6 keys for cyber-resilience generalities | keep `dupont2019cyberresilience, bjorck2015cyber` | Drop `maillart2010heavy, wheatley2016extreme` (cited only here); fold `kuypers2018designing` use into next paragraph. |
| [3_research_gaps.tex:19](sections/3_research_gaps.tex#L19) | `bruneau2003framework, francis2014metric, cutter2010disaster, kruk2017building, gao2016universal, panteli2017metrics` (6) | `bruneau2003framework, kruk2017building, gao2016universal` | Three cover engineering / health / complex-systems; the other three appear in adjacent sentences anyway. |
| [4_enactment–scope.tex:26](sections/4_enactment–scope.tex#L26) | Nine cells × 3–4 cites each = ~30 instances | aim for ≤ 2 cites per cell; drop `ibnehossain2020modeling` (singleton), `mahajan2022participatory` (mispositioned, A4), `finma2023operational` from infrastructural-managerial cell (already cited in §6 backbone) |
| [5_research_directions.tex:16](sections/5_research_directions.tex#L16) | 5 keys for macro institutions | `nist2024csf, bcbs2021operational, european2022regulation` | Drop `meerow2016defining, allen2018quantifying` (A3) |
| [5_research_directions.tex:36](sections/5_research_directions.tex#L36) | Long cluster for CCRC Chain + DORA | trim to `ccrc2024chain, ecb2018tiber, european2022regulation` |
| [5_research_directions.tex:50](sections/5_research_directions.tex#L50) | 6 keys for ecosystem governance | `arnold2004informationsharing, lostri2022shared, mermoud2019share, gillard2023efficient` | Drop `brauer2008compartmental` (A5), `maillart2017bugbounty` (keep only one of self-cites, see §2.3) |
| [6_implications_for_research.tex:17](sections/6_implications_for_research.tex#L17) | 6 keys for backbone | `calder2021iso, bcbs2021operational, finma2023operational, nist2024csf` | Drop `lengnick2011developing` (A8), `weick2011managing` (cited in next clause anyway) |

---

## 4. Removable references — path to 70–80 unique keys

### 4.1 — Appendix-only singletons (25 refs, 27 instances)

These keys are cited *exclusively* in `12_appendices.tex` and almost all serve as decoration for the historical/mathematical narrative. The appendix can keep its expository quality with substantially fewer citations.

**Strong candidates for removal (the equations/concepts don't need attribution):**

| key | role | proposal |
|---|---|---|
| `walpole1998probability` | introduces survival function $S(t)$ | textbook fact — drop citation |
| `marconi2008fluctuation` | thermodynamics stability inequality | drop citation |
| `pelorosso2017low` | thermodynamics exponential decay | drop citation |
| `almassalkhi2015modelpredictive` | model-predictive control example | drop or replace with `astrom2008feedback` (also appendix-only — pick one) |
| `astrom2008feedback` | textbook ref for control theory | keep, drop `almassalkhi2015modelpredictive` |
| `newman2018networks` | textbook ref for giant component | drop — standard fact |
| `strogatz2018nonlinear` | textbook ref for ODE equilibrium | drop — standard fact |
| `callister2020materials` | modulus-of-resilience formula | drop (and the DOI is wrong anyway, per prior review) |
| `rakesh2019resilience`, `manikis2019computational`, `kleitman2022applying`, `rutter1987psychosocial`, `werner1995resilience`, `walsh1996concept`, `antonovsky1971twentyfive`, `hill1949families`, `alexander2013resilience` | decorative psychology/history refs in the resilience-history appendix | keep at most 2 (`luthar2000construct` and `ungar2021modeling` already cover the construct) |
| `peng2015invulnerability`, `wangersky1978lotka`, `zhu2015game` | one-line appendix mentions | drop |
| `braun2019thematic` | method ref in Rota appendix | keep (correct methodological anchor) |
| `vomBrocke2009` | one of two Vom Brocke method refs | drop, keep `vombrocke2015standing` (newer) |
| `webster2002analyzing` | review-method anchor | keep |
| `aldrich2014social` | community social capital | keep |

**Net cut from appendix-only: ~18 refs.**

### 4.2 — Main-body singletons that add little (subjective; review needed)

| key | uses | proposal |
|---|---:|---|
| `ibnehossain2020modeling` | 3× but always in clusters of 4–5 | drop — never load-bearing |
| `mahajan2022participatory` | 3× — urban planning context | drop (see A4) |
| `rane2024artificial` | 2× | drop (see A6) |
| `mayer2021putting` | 1× | drop (see A7) |
| `kalisch2024neurobiology` | 2× | drop (see A9; the cybersecurity neuroscience hook is weak) |
| `moreno2018womens` | 1× | drop (see A10) |
| `lanzara1999transient` | 2× | the "transient organizing" claim could collapse with `weick2011managing` |
| `klein2008performing` | 2× | could collapse with `weick2011managing` |
| `klein2015wikipedia` | 1× | drop — appears in one cluster only |
| `vogus2007organizational` | 6× | KEEP — HRO anchor; load-bearing |
| `myerson2013game` | 1× | drop — appendix singleton only |
| `aase2020resilience` | 1× | drop |
| `sornette2013exploring` | 1× | drop |
| `sornette2014how` | 1× | drop |
| `maillart2010heavy` | 1× | drop (cyber-extreme-distribution claim already in `wheatley2016extreme`) |
| `wheatley2016extreme` | 1× | drop OR keep one of (maillart2010, wheatley2016) |
| `pumpuni2017resilience` | 2× | drop (IT-failure-as-example claim can stand without citation) |
| `bilge2012before` | 2× | KEEP — anchor for "long dwell time" claim |
| `roumani2022detection` | 2× | could collapse with `bilge2012before` |
| `arif2024overview` | 1× | drop (see A2) |
| `arora2025understanding` | 1× | this is the SSRN AI-security paper; weak ground for the intro claim. Drop unless central to the AI-resilience story. |
| `falco2019cyber` | 4× | KEEP — generic cyber-resilience anchor |
| `hausken2020cyber` | 3× | KEEP |
| `feder2019biology` | 1× | keep (neuropsych anchor) — but trim cluster (background:21) so it's load-bearing |
| `mcewen2004protection` | 2× | drop — overlap with `feder2019biology` and `kalisch2024neurobiology` |
| `kruk2017building` | 4× | KEEP — health-systems anchor |
| `norris2007community` | 2× | could collapse with `kruk2017building` |
| `helbing2012agent` | 2× | KEEP — ABM anchor |
| `dawson2011agentbased` | 4× | KEEP |
| `kwakkel2016comparing`, `haasnoot2013dynamic`, `lempert2019robust` | 2–3× each, all in deep-uncertainty paragraph | keep one (`kwakkel2016comparing`), drop the other two — they cluster identically in two places |
| `panteli2017metrics` | 6× | KEEP — but mispositioned in background:12, see §3 |
| `nelson2007adaptation` | 1× | drop — overlaps with `walker2004resilience` |
| `ivanov2022viable` | 2× | KEEP — supply-chain dynamic-capabilities anchor |
| `taleb2012antifragile` | 4× | KEEP |
| `henfridsson2013generative` | 4× | KEEP |
| `liu2022network` | 3× | KEEP |
| `boh2023building` | 8× | KEEP (but DOI is broken — see prior reference review) |
| `aerts2018integrating` | 3× | KEEP — bridging anchor for transferability claim |
| `linkov2019fundamental` | 2× | KEEP — frames the standards landscape |
| `jacobs2017applying`, `aydin2018integration`, `luke2012systems` | 1–2× each, all in transferable-methods paragraph (research gaps:23–25) | keep `luke2012systems` (PH network analogue) as the strongest fit; drop the other two |
| `simon1997administrative`, `march1993organizations` | 1× each | KEEP — load-bearing for bounded-rationality framing |
| `galbraith1973designing` | 2× | KEEP — coordination-design anchor |
| `holling1996engineering` | 2× | KEEP (book-level DOI noted in prior review) |
| `power1999audit` | 3× | KEEP |
| `aldrich2014social` | 1× (appendix) | KEEP (social-capital anchor) |
| `schumpeter1942capitalism` | 1× | drop unless creative-destruction passage is rewritten; the metaphor is decorative |
| `taleb2012antifragile` | 4× | KEEP |
| `kleitman2022applying` | 1× (appendix) | drop |

**Net cut from main body: ~25–30 refs** when combined with the cluster trims in §3.

### 4.3 — Summary count

| Action | Refs removed |
|---|---:|
| Appendix-only decoration | ~18 |
| Main-body singletons (positioning fixes + dispensable) | ~25 |
| Tail of dense clusters (without dropping the key elsewhere) | ~30 instances (no unique-key reduction; just trims the count) |
| **Net unique-key reduction** | **~43** |

That brings 155 → **~112**. To hit 70–80, additional cuts are needed:

- Consolidate the **regulatory backbone** to 3 keys (`bcbs2021operational`, `european2022regulation`, `nist2024csf`) and drop the rest (`finma2023operational`, `european2022nis2`, `boe2021cbest`, `enisa2024cybereurope`) — each appears 1–3× and could be merged into a single regulatory-landscape footnote or the backbone enumeration in §6. **−4 keys**
- Consolidate the **ecological-resilience canon** in background §27 + appendix: keep `folke2010resilience`, `walker2004resilience`, drop `folke2004regime`, `anderies2004framework`, `adger2005socialecological`, `berkes1998linking`, `lebel2006governance`, `nelson2007adaptation`. **−6 keys** (verify each isn't load-bearing in a unique site; `ostrom1990governing` should stay).
- **Trim psychology/neuroscience traditions** to 2 keys (`luthar2000construct` for psychology, `feder2019biology` for neuroscience) — drop `kalisch2024neurobiology`, `mcewen2004protection`, `masten2010disasters`, `feder2019biology`-overlap, `rakesh2019resilience` (already in 4.1). **−4 keys**
- **Drop redundant ISMS/standards refs**: between `calder2021iso` (ISO 22301) and `linkov2019fundamental` (standards landscape), one is enough in implications. **−1 key**
- **Self-citation hygiene**: of `gillard2023efficient`, `maillart2008zipf`, `maillart2017bugbounty`, `maillart2019aristotle`, `maillart2024computational`, `maillart2010heavy`, `mermoud2019share` — keep `gillard2023efficient` (load-bearing) and `mermoud2019share` (load-bearing for ISAC behavioural claim), drop the rest unless they are uniquely supporting a claim no other ref can. **−4 keys**

Combined: **~155 → ~93**, then with the cluster pruning headroom **→ 75–80**. Achievable without rewriting whole paragraphs.

---

## 5. Recommended decision sequence

1. **Apply positioning fixes (§1)** — these don't require trade-offs, just substitute or delete.
2. **Decide on the appendix budget** — if the historical appendix is meant as a self-contained primer for non-experts, the textbook-fact citations (Strogatz, Newman, Walpole, Marconi, Pelorosso) can simply be removed without weakening the prose.
3. **Apply the over-citation rotation (§2.1–2.6)** — gives ~30 instance reduction with no key change yet; reveals which keys then become singletons.
4. **Apply singleton drops (§4.2)** — biggest unique-key reduction.
5. **Apply backbone/canon consolidation (§4.3)** — the final push to 75–80 if needed.

---

## 6. Out-of-scope items noted in passing

- **Prior reference-validation issues** (handled in earlier review, not re-listed here): `boh2023building` DOI 404; `enisa2017isacs` malformed DOI; `callister2020materials` wrong DOI; `vomBrocke2009` URL 403; `SOCI2018` URL too generic; `bilge2012before` and `mermoud2019share` missing diacritics. These remain to fix regardless of which entries survive the trim.
- **`european2022regulation` author rendering** fixed earlier this session ([references.bib:2519](references.bib#L2519)).
