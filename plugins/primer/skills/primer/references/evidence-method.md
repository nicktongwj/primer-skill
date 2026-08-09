# Evidence Method

Use this method to decide what deserves to carry the conclusion. Keep the full
ledger internal; expose only the selected evidence cards and material gaps.

## Source classes

| Class | Typical sources | What it can establish |
|---|---|---|
| **Direct** | Original paper or dataset, official specification, model card, vendor price page, repository, release, filing | What the source formally reports, offers, measured, or shipped |
| **Independent** | Third-party benchmark, documented test, systematic review, reputable analysis with disclosed method | Whether a result replicates or survives outside the originating party |
| **Empirical** | Detailed practitioner account, Reddit post, GitHub issue, forum report, video demonstration | What happened in a specified real-world setup; practical failure modes and counterexamples |
| **Commentary** | News summary, opinion, unsourced comparison, promotional post | Framing, terminology, and leads to stronger sources |

Source class and evidence strength are separate. A direct vendor source may be
decisive for its current list price and weak for a superiority claim. An
independent test may be strong but inapplicable because its conditions differ.
Independence is financial as well as editorial: a sponsored, affiliate-funded,
or vendor-commissioned test belongs to the vendor's evidence family, whatever
its byline.

## Confidence calibration

- **High:** The evidence directly tests the proposition under applicable
  conditions, the method is inspectable, and an independent source or distinct
  evidence family corroborates the result.
- **Medium:** The evidence is credible but limited by one material uncertainty,
  such as a narrow sample, imperfectly matched conditions, one source family, or
  an older measurement.
- **Low:** The claim relies mainly on anecdote, incomplete conditions, promotional
  material, a search snippet, weak comparability, or an unresolved contradiction.

Do not average confidence mechanically. The weakest essential link can limit
the conclusion even when several peripheral facts are strong.

## Conflicting sources

When credible sources disagree, try to dissolve the conflict before weighing it.
Check for mismatched conditions, definitions, dates, or measurement methods;
most apparent contradictions are answers to two different questions. If the
conflict survives, prefer the more direct, more recent, better-conditioned
measurement, and report the disagreement beside the figure used. A conflict
settled by silently discarding the inconvenient source is not settled.

## Null results

A search that finds nothing is a finding about the search, not yet about the
world. Record what was searched before drawing anything from it.

- In a densely covered domain (major products, listed companies, widely
  reported policy), repeated failure to find support for a specific claim is
  weak evidence against it. Report it with that qualifier, not as proof.
- In a thinly covered domain (niche tools, recent events, non-English
  coverage), a null result is uninformative. Do not convert it into "there is
  no evidence".
- State the coverage assumption whenever absence of evidence is asked to carry
  any weight.

## Evidence ledger

Record these fields for each candidate item:

1. **Proposition:** The precise subclaim it supports or challenges.
2. **Datum:** The exact number, observation, quotation, or finding.
3. **Conditions:** The variables needed to interpret or reproduce it.
4. **Direction:** Supports, challenges, or bounds the proposition.
5. **Provenance:** Source class, author or organisation, link, and date.
6. **Independence:** Original, independent replication, or derivative repetition.
7. **Limitation:** The strongest reason not to generalise from it.
8. **Confidence:** High, Medium, or Low, with one-sentence reasoning.

## Condition checklists

Capture only the checklist relevant to the claim.

**Technical performance:** exact product or model and version; parameter count
and quantisation where relevant; hardware and memory; software or inference
backend and version; context and prompt size; batch or concurrency; time to first
result; steady-state throughput; hidden processing or reasoning where relevant;
end-to-end task time; output length; quality or capability reference; power draw;
and measurement date.

**Cost:** complete bill of materials; component versus system price; upfront
versus recurring cost; price of the realistic service or cloud alternative;
taxes, shipping, support, and energy where material; region and currency; new
versus used equipment; and price date.

**Study or survey:** population and sample size; selection method; intervention
or comparison; measured outcome; effect size or absolute numbers; uncertainty;
time period; and whether the result is observational or causal.

**Business or market claim:** denominator; time window; geography; cohort;
selection effects; whether the metric is reported or independently measured; and
whether the evidence establishes causation or only association.

## Community and repository evidence

Prefer first-person reports containing a reproducible setup, exact version,
measurement, and limitation. A detailed low-engagement report can be stronger
empirical evidence than a popular vague post.

Treat engagement as evidence of attention, not truth. Treat GitHub stars as an
adoption or interest proxy, not a quality verdict. Treat issues and complaints
as selection-biased unless corroborated; satisfied users are less likely to file
issues.

Use community evidence in one of three ways:

- illustrate how a direct or independent result feels in practice;
- expose a failure mode that controlled tests omitted; or
- identify a counterexample that narrows an overbroad proposition.

## Practical translation

Translate the result only when the conversion improves understanding. Show the
assumption compactly.

- **Throughput:** `generation time = output tokens / decode tokens per second`.
  Add time to first token separately when available.
- **Percentages:** give the absolute baseline or population where available.
- **Cost:** give total setup or operating cost for the decision-relevant period,
  not only the cheapest component.
- **Scale:** convert abstract totals into per-user, per-day, per-answer, or
  comparable-unit terms where defensible.
- **Break-even:** when a higher fixed cost buys a lower recurring cost, show
  `break-even usage = incremental fixed cost / saving per unit` or the equivalent
  time calculation, with the assumed usage beside it.

Use a two-anchor comparison when a raw scale will not mean much to the intended
reader:

1. **Familiar anchor:** a product, cost, duration, outcome, or experience the
   audience can immediately picture.
2. **Frontier anchor:** the relevant best-in-class, state-of-the-art, or upper
   bound that shows what capability is gained or lost.

Select anchors by audience relevance, not convenience. Prefer a widely bought
complete system over an exotic component, and compare decision-relevant
capability as well as the shared metric. If the anchors differ in quality,
features, conditions, or workload, state that beside the comparison.

## Comparison design

Before using a comparison in the top card, test it against five questions:

1. **Recognisable:** Can the intended reader immediately picture it?
2. **Decision-relevant:** Is it an option the reader might realistically choose?
3. **Complete:** Does the cost cover the usable system or service, not one
   attractive component?
4. **Outcome-matched:** Are both sides being judged on the same useful result?
5. **Condition-matched:** If speed, quality, workload, or features differ, is the
   mismatch visible beside the comparison?

Use the most relatable valid comparison, not the most dramatic one. A common
consumer product can be the right familiar anchor even when an enthusiast device
has better specifications. If the common product cannot support the claimed
workload, say so and step up to the cheapest comfortable option.

For performance claims, keep three layers separate:

1. **Raw metric:** throughput, latency, benchmark score, or component capacity.
2. **User experience:** time to first useful result and total wait under a
   representative task.
3. **Outcome:** whether the result is sufficiently accurate, capable, complete,
   or reliable without retries or manual repair.

The strongest practical measure is usually time and cost to a usable outcome,
not the highest raw throughput. Label thresholds as **technically possible**,
**usable with compromise**, or **comfortable** when that distinction matters.
When a headline metric is only a proxy for the outcome, state the mechanism that
connects them and the most important factor the proxy omits.

When three or more options repeat the same fields, use a compact table. Include
the realistic alternative in the same row or an adjacent column so that local
cost is not shown without cloud cost, a treatment without standard care, or a
product without the incumbent option.

Do not imply false precision. Round translated figures to the granularity the
source conditions support.

## Verification pass

Re-open every source carrying the conclusion and assign an internal verdict:

- **Confirmed:** The source and material conditions support the claim as written.
- **Corrected:** The source is real but the value, date, scope, or characterisation
  required correction; use the corrected form.
- **Unverified:** The source or operative material could not be checked; do not
  let it carry the conclusion.
- **False:** The source does not exist or does not support the claim; remove it.

Check copied claims for a common origin. Three articles repeating one press
release provide one evidence family, not three independent confirmations. A
claim whose origin cannot be traced at all, as with aggregator pages and
uncited summaries, is Unverified however widely it is repeated.
