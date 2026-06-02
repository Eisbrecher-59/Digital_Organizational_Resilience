# Manuscript streamlining review — redundancies and citation density

Scope: identify opportunities to compress prose without information loss, and benchmark current citation density against MISQ norms. **No text changes at this stage** — proposals only.

---

## 1. Current citation density

| metric | value |
|---|---:|
| Unique refs in main bib | 91 |
| Total citation instances | 572 |
| Average instances per ref | 6.29 |
| Prose word count (sections 1–7) | ~10,000 |
| Citation instances per 1,000 words | 54.5 |
| Citation instances per double-spaced MS page (300 wpm) | 16.3 |

**Distribution of citations per ref:**
- 1–2× (singletons + doubles): 26 refs (29%)
- 3–6×: 27 refs (30%)
- 7–10×: 18 refs (20%)
- 11–18×: 20 refs (22%)

The mass is in the long, heavy tail — 20 refs cited 11+ times account for nearly half the instances. A small number of "structural" refs is doing most of the work.

**Density by section:**

| Section | words | cites | per 1,000 words |
|---|---:|---:|---:|
| §1 Introduction | 1,069 | 22 | **21** |
| §2 Background | 2,264 | 140 | **62** |
| §3 Research Gaps | 1,319 | 66 | **50** |
| §4 Enactment-Scope | 887 | 63 | **71** ← densest |
| §5 Research Directions | 2,698 | 150 | **56** |
| §6 Implications | 1,530 | 47 | **31** |
| §7 Conclusion | 267 | 5 | **19** |

§4 and §2 are the densest. §1, §6, §7 are at a more readable density. The middle sections (§2–§5) carry the citation weight.

## 2. MISQ baseline comparison

**Bottom line: the citation worry is largely misdirected. The manuscript is below MISQ ref-count norms, not above them.**

Reference counts in well-known MISQ reviews/theory pieces (CrossRef + Semantic Scholar):

| Article | Year | Refs | Pages |
|---|---|---:|---:|
| Leidner & Kayworth, IT culture review | 2006 | **198** | 42 |
| Sarker et al., sociotechnical commentary | 2019 | **192** | 24 |
| Baird & Maruping, IS-use delegation | 2021 | **176** | ~25 |
| Berente et al., Managing AI | 2021 | **157** | 17 |
| Gregor, Nature of Theory | 2006 | **134** | 31 |
| Sambamurthy et al., Digital options/agility | 2003 | **109** | 26 |
| Grover & Lyytinen, New State of Play | 2015 | **99–120** | 25 |
| Venkatesh et al., UTAUT2 | 2012 | **96** | 21 |
| Chen et al., BI&A | 2012 | **86** | — |
| Gregor & Hevner, DSR | 2013 | **80** | 18 |
| **This manuscript** | — | **91** | ~10 |

- **Typical band for MISQ reviews: ~130–200 refs**; theory/commentary pieces cluster **~80–160**. At 91, the manuscript is at the **low end** — closer to a focused theory piece than a comprehensive review.
- **Reuse ratio (~6.3×)** is plausibly normal-to-slightly-high but defensible. MISQ doesn't publish in-text instance counts so this can't be benchmarked directly, but [Webster & Watson 2002](https://misq.umn.edu/misq/article/26/2/xiii/1323) and [Rai 2016 "Writing a Virtuous Review"](https://aisel.aisnet.org/misq/vol40/iss3/2/) explicitly push **concept-centric synthesis** — i.e. a small anchor set of canonical references recurring across sections is the recommended pattern, not a flaw. No MISQ editorial guidance was found that warns against over-citation per se.
- **~57 instances per manuscript page** is dense prose but not anomalous for theory-development MISQ work, where most claims carry provenance.

### What this means for the streamlining decision

- The case for **citation cuts to reduce density** is weak. If anything, a reviewer might ask for *more* breadth in the reference set (e.g. additional MISQ self-cites to anchor the IS-research framing).
- The case for **prose redundancy cuts** stands independently. Removing repeated claims tightens the argument whether or not the bibliography changes.
- The Tier C "citation density" recommendations below (§6) should be downgraded — they're now closer to copy-edit hygiene than a structural priority. Tier A and B redundancy cuts remain valuable.

If the author is set on lowering perceived citation weight, the better lever than dropping references is to **reduce the visible cluster sizes** (3-ref clusters read lighter than 5-ref clusters even if the bibliography is unchanged) — but this is presentation, not substance.

---

## 3. Prose redundancies — claims restated across the manuscript

These are the same claim said in different words, with progressively more refs piled on each time.

### R1 — "Compliance ≠ adaptation" (restated 7+ times)

The paper's central pivot, but stated very many times:

| location | wording (paraphrased) |
|---|---|
| [§1:9](sections/1_introduction.tex#L9) | "audit-driven compliance and control frameworks tend to emphasize documentation and formal assurance at a point in time" |
| [§3:13](sections/3_research_gaps.tex#L13) | "compliance investment is approved more readily than operational adaptation" |
| [§3:15](sections/3_research_gaps.tex#L15) | "they certify documented readiness more readily than reconfiguration, improvisation, or learning" |
| [§3:17](sections/3_research_gaps.tex#L17) | "What they still validate weakly is behavior when disruption departs from script" |
| [§3:25](sections/3_research_gaps.tex#L25) | "the same instruments that certify preparedness without observing adaptation" |
| [§4:9](sections/4_enactment–scope.tex#L9) | "compliance substitutes for adaptation, and exercises rarely change operational routines" |
| [§6:5](sections/6_implications_for_research.tex#L5) | "still struggle to show boards how any of it evidences adaptive performance when disruption departs from script" |
| [§7:6](sections/7_conclusion.tex#L6) | "adaptive performance under disruption, and improvement across successive events, often remains harder to evidence than compliance itself" |

**Recommendation:** keep the §1 and §6 statements (frame the argument and recap it), use §3 to make it once with field-interview evidence, drop the §3 echoes inside the same section (§3:15, §3:17, §3:25 each restate it), and let §4 / §7 cross-reference back to §1's framing rather than re-stating.

### R2 — "Three deficits" enumerated 4 times in §3 alone

- [§3:9](sections/3_research_gaps.tex#L9) lists the three with one-line summaries
- [§3:11, §3:15, §3:23](sections/3_research_gaps.tex#L11) each is a bold-header paragraph on one deficit
- [§3:27](sections/3_research_gaps.tex#L27) recaps all three: "These three deficits are interconnected: conceptual plurality... weak empirical validation... methodological fragmentation"
- [§3:29](sections/3_research_gaps.tex#L29) reformulates as "methods that trace adaptation over time"

**Recommendation:** drop §3:27 entirely (pure recap of what just preceded). Optionally fold §3:29's reformulation into the §3:23 deficit paragraph.

### R3 — "Three lines of work" in §4

- [§4:7](sections/4_enactment–scope.tex#L7) introduces technical / organizational / ecosystem lines
- [§4:9](sections/4_enactment–scope.tex#L9) immediately recaps: "technical work under-specifies governance... organizational work under-specifies infrastructures... ecosystem work under-connects"

The recap is essentially the same three claims in negation form. **Recommendation:** merge §4:7 and §4:9 by inlining the "under-specifies" critique into each line's introduction in §4:7, then delete §4:9.

### R4 — Table 2 (RG2) described twice in §3

- [§3:19](sections/3_research_gaps.tex#L19) "Simulation, network analysis, and trace-based measurement concentrate at the infrastructural scope; the organizational and ecosystem scopes lean instead on case studies, conceptual frameworks, and standards"
- [§3:23](sections/3_research_gaps.tex#L23) "simulation, network analysis, and marker design are concentrated in engineering, complex systems, and public health; management and cyber-risk research draw mainly on surveys and case studies"

§3:23 uses the OLD discipline framing of the table (pre-redesign legacy vocabulary) while §3:19 uses the NEW scope framing. **Recommendation:** delete §3:23's first half (the table description) and keep only the methodological-transfer claim. Both paragraphs are otherwise about the same observation.

### R5 — Industry backbone enumerated twice

- [§3:17](sections/3_research_gaps.tex#L17) lists "BCPs, business impact analyses, impact tolerances..., ICT continuity..."
- [§6:5](sections/6_implications_for_research.tex#L5) gives the more comprehensive version: ISO 22301, BCBS principles, FINMA, DORA, ICT continuity, backup-testing, crisis-comms, third-party dep mapping, TIBER-EU, CBEST

**Recommendation:** keep the §6:5 catalogue (it anchors the "we're not asking for more controls" pivot). Compress §3:17 to a sentence or two — "Regulatory convergences (DORA, NIS2, Basel, ISO 22301, NIST CSF) and threat-led testing have made resilience auditable; what they validate weakly is behavior when disruption departs from script" — and let §6:5 do the enumerating.

### R6 — Define / Measure / Govern triad in §6:5 and §7:8

- [§6:5](sections/6_implications_for_research.tex#L5) bold headers: **Define / Measure / Govern**
- [§7:8](sections/7_conclusion.tex#L8) repeats: "**define** adaptive performance before templates substitute for it; **measure** it from digital traces; **govern** it through escalation, review, and cooperative activation"

§7 is the conclusion so some recap is appropriate, but this version copies §6 almost verbatim. **Recommendation:** §7 can replace the bold-triad recap with one prose sentence ("Define, measure, and govern adaptive performance from the traces organizations already produce") — the reader just read §6.

### R7 — Figure 1 (triangle) restated 3 times + caption

- [§4:13](sections/4_enactment–scope.tex#L13) introduces operational indicators / design principles / benchmarks-and-warnings
- [§4:18](sections/4_enactment–scope.tex#L18) caption restates the same triad
- [§4:28](sections/4_enactment–scope.tex#L28) maps the triad to grid rows
- [§5:54](sections/5_research_directions.tex#L54) returns to it in the recap

**Recommendation:** §4:28's mapping is the load-bearing use. §4:13's intro can be shorter — let the figure caption carry the definitions. §5:54 should reference fig:triangle without re-defining.

### R8 — §5 closing paragraph is mostly recap

[§5:54](sections/5_research_directions.tex#L54) opens "Taken together, the agenda above is cumulative..." and then restates:
- §5.1 = theory at each scope clarifies enactment
- §5.2 = measurement operationalizes from digital traces
- §5.3 = governance couples indicators to decision rights

Plus a final recap of the whole paper ("theory, evidence, simulation, and governance advance together"). **Recommendation:** §5:54 could shrink from ~150 words to 40–50: a single sentence about cumulative advance + the bridge sentence to §6.

### R9 — Field-interview invocations cluster

`rota2024` is cited 8× in main + the Quote* macros (`\QuoteSilos`, `\QuoteCompliance`, `\QuoteQuantAmb`, `\QuoteLearning`, `\QuoteCyberRange`, `\QuoteFlexPrec`, `\QuoteSoc`) appear ~10× across §1, §3, §4, §5, §6. Several paragraphs invoke field interviews back-to-back:

- §3:23, §3:25, §3:27 — three field-interview invocations in three consecutive paragraphs
- §5:34, §5:48 — interviews invoked in two adjacent sub-section closings

**Recommendation:** each Quote macro is fine in its first use, but inviting "field interviews report the same pattern" repeatedly creates a circular pattern. Consolidate to one anchor invocation per section. The §3:23–25–27 sequence in particular reads as "and the interviews say so too" three times.

### R10 — "Infrastructural / Organizational / Ecosystem" trichotomy repeated structurally

Every subsection in §5 (theory, measurement, governance) opens with `\textbf{Infrastructural scope (meso infrastructures).}` / `\textbf{Organizational scope (micro routines).}` / `\textbf{Ecosystem scope (inter-organizational ecosystems).}` — and each sub-subsection re-asserts what the matrix says about that cell. This is intentional parallel structure, but each "The matrix marks X as Y..." sentence is a recap.

**Recommendation:** the parallelism is a feature, not a bug, but the per-subsection "The matrix marks..." sentences could be compressed to a half-sentence (or moved to the §5:16 matrix-summary paragraph that already covers all four direction types).

---

## 4. Prose-level micro-redundancies (smaller scale)

These are sentence-level dittos worth catching in a copy-edit pass.

| location | issue |
|---|---|
| [§1:5](sections/1_introduction.tex#L5) | "compresses the time available to revise governance, controls, and cross-unit coordination before prior adaptations have taken hold" + next sentence "the threat environment has continued to accelerate dramatically pushing organizational adaptation to the limits" — both say "things move too fast for orgs to keep up" |
| [§2:5](sections/2_background.tex#L5) | "obscures why organizations can invoke the same label while pursuing different metrics, interventions, and governance logics" — same idea as §3:13 "boards, regulators, and managers can each pursue a different version of resilience while using the same word" |
| [§3:9](sections/3_research_gaps.tex#L9) | "Operationalizable, transferable measures are the critical bottleneck" — restated immediately in §3:23 "It is the weak translation of technical advances in resilience measurement into governance tools" |
| [§5:30](sections/5_research_directions.tex#L30) | Single ~400-word paragraph mixes (a) two-layer research strategy, (b) Splunk/Elastic/Sentinel product mention, (c) Saporo product mention. Each of (b) and (c) could be a footnote — the prose claim is "commercial tools generate indicators but don't reach governance" and it doesn't need three product call-outs |
| [§5:46](sections/5_research_directions.tex#L46) | First sentence "Specify design principles for infrastructure governance under stress---access control, vendor escalation, operator--provider coordination, governance of critical software updates, service-restoration priorities" + later "articulate those principles for infrastructure governance under stress" — second mention is bare recap |
| [§6:5](sections/6_implications_for_research.tex#L5) | Single ~600-word paragraph blends backbone catalogue, BCP-doesn't-evidence-adaptation diagnosis, "journey" reframe, and Define/Measure/Govern triad. Could be 2 paragraphs (one diagnostic, one prescriptive). |
| [§6:9](sections/6_implications_for_research.tex#L9) | Sentence "operating under disruptive conditions is less a control problem than an ongoing business-adaptation problem distributed across infrastructures, units, and partners" + 2 sentences later "resilience is not confined to one asset, one team, or one managerial disposition; it emerges through interaction between people, technical systems, routines, escalation pathways, and governance arrangements" — same distributedness claim said twice |
| [§6:11](sections/6_implications_for_research.tex#L11) | "indicators... coordination speed, stakeholder support, community ties, the capacity to reconfigure infrastructures" — same indicator list shown again at §6:15 ("coordination speed, recovery sequence, or adaptive reconfiguration") |

---

## 5. Citation-density observations (independent of redundancy)

### 5a. Heavy-tail keys carry too much weight per citation

The top-20 most-cited refs collectively appear 270 times — almost half (47%) of all citation instances on just 22% of the refs. Each of these has effectively become a "background" anchor that appears whenever the topic is mentioned. The risk is that the substantive contribution of each individual reference becomes invisible.

- `boin2013resilient` (18×), `bcbs2021operational` (18×), `woods2015four` (18×) — invoked any time the topic of governance, regulation, or capability comes up. Each could probably drop to ~10× with no loss of support.
- `bhamra2011resilience` (16×) and `linkov2013resilience` (16×) — same pattern.

### 5b. Many citations are "agreement clusters" of 4+ keys

A scan of the largest clusters:

- [§5:10](sections/5_research_directions.tex#L10) — `\autocite{francis2014metric, cutter2010disaster, kruk2017building, dawson2011agentbased, aerts2018integrating}` (5 refs)
- [§5:16](sections/5_research_directions.tex#L16) — `\autocite{nist2024csf, bcbs2021operational, european2022regulation}` (×4 such clusters in this paragraph)
- [§4:7](sections/4_enactment–scope.tex#L7) — three back-to-back 4–5-ref clusters in the same sentence
- [§4:26](sections/4_enactment–scope.tex#L26) — nine cells each with 2–4 refs in one paragraph

When 4+ refs appear in a single cluster, the reader can't tell what each contributes. MISQ tends to favor 1–2-ref citations with a brief gloss when more are needed (e.g. "e.g., X; Y; for review see Z"). **Recommendation:** keep clusters ≤ 3 refs unless the claim is genuinely a "many independent sources converge" point.

### 5c. Re-citation in the same paragraph

Paragraphs where the SAME ref is cited multiple times within ~100 words:
- §3:13 cites `hillmann2021organizational` mid-paragraph though the same key appeared in §3:5 just above
- §5:24 cites `duchek2019organizational` twice in two adjacent clusters
- §5:38 cites `dawson2011agentbased` twice in one paragraph
- §5:40 cites `francis2014metric` twice in one paragraph
- §5:46 cites `hausken2020cyber`, `ecb2018tiber`, `skopik2016problem` twice in one paragraph (lead and recap clusters)

**Recommendation:** the second cite in the same paragraph rarely adds attribution value; could be dropped.

---

## 6. Streamlining opportunities — prioritized

### Tier A — high-confidence cuts (no substantive change)
1. Delete §3:27 (pure recap of the three deficits — §3 just walked through them)
2. Delete §5:54 closing recap and replace with one bridging sentence to §6
3. Delete §3:23 first half (Table 2 re-description in old vocabulary) — §3:19 already introduces it in the right framing
4. Compress §3:17 — let §6:5 carry the full backbone catalogue; here just name the regulations
5. Compress §7 to drop the Define/Measure/Govern restatement (§6 just made it) — leave the high-level "from organizing principle to grounded socio-technical capacity" line

Estimated reduction: ~400–500 words and ~30 cite instances.

### Tier B — argument-tightening (needs author judgement)
6. Merge §4:7 and §4:9 (introduction of three lines + critique of three lines = one paragraph)
7. Convert the per-subsection "The matrix marks X..." sentences in §5 into a single matrix-introducing paragraph at §5:16 (already exists but currently followed by three more matrix-recap openings)
8. Split §5:30 (~400 words) into 2 paragraphs and move the Splunk/Elastic/Sentinel/Saporo product call-outs to footnotes
9. Split §6:5 into a diagnostic paragraph + a prescriptive paragraph (currently one ~600-word block)
10. Audit §6 implications for which 5 paragraphs are doing distinct work — currently 5 implications but §6:9 ("blind spot" framing) and §6:15 ("multi-level architecture") overlap significantly in their distributedness claim

Estimated reduction: another ~500 words and ~40 cite instances.

### Tier C — citation density (in addition to Tier A/B)
11. Sweep the top-20 most-cited refs: each occurrence of `boin2013resilient`, `bcbs2021operational`, `woods2015four`, `bhamra2011resilience`, `linkov2013resilience` that appears in a 4+ ref cluster can be reviewed for deletion (the cluster will still cite 3 anchors)
12. Drop the 12 "second occurrence in same paragraph" cases listed in 5c
13. Trim 4+ ref clusters to ≤ 3 refs (§5:10, §5:16, §4:7, §4:26 are the main offenders)

Estimated reduction: another ~50–70 cite instances and possibly 5–8 unique refs that become singletons.

### Combined: where this lands
- **Words**: ~10,000 → ~9,000–9,100 (10% shorter prose)
- **Citation instances**: 572 → ~450–480 (down ~20%)
- **Unique refs**: 91 → ~85 (minor reduction, since the cuts target rotation/overlap rather than new singletons)
- **Average reuse**: 6.3× → ~5.4× (pending MISQ baseline)

---

## 7. Sources for the MISQ baseline

- [Webster & Watson 2002 — "Analyzing the Past to Prepare for the Future"](https://misq.umn.edu/misq/article/26/2/xiii/1323)
- [Rai 2016 — "Writing a Virtuous Review"](https://aisel.aisnet.org/misq/vol40/iss3/2/)
- [MISQ Submission Guidelines](https://misq.umn.edu/pages/submission_guidelines)
- Leidner & Kayworth 2006, Sarker et al. 2019, Berente et al. 2021, Gregor 2006, Sambamurthy et al. 2003, Grover & Lyytinen 2015, Venkatesh et al. 2012, Chen et al. 2012, Gregor & Hevner 2013 — reference counts via [CrossRef API](https://api.crossref.org) and [Semantic Scholar API](https://api.semanticscholar.org).
