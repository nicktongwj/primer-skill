# Primer — an AI agent skill for understanding a topic

Primer is a skill for getting up to speed on something. Ask your agent about a
field, technology, concept, or event, and it returns a short, sourced map of the
territory first, then expands whichever part you choose. It explains the topic
and the live disagreements; it does not argue a verdict.

Each key fact comes with a source, a date, and a High, Medium, or Low confidence
label, checked before it reaches you.

## Why this exists

Much of what we take as true arrives second-hand. A friend swears by a
supplement, a relative buys a product because a neighbour did, a claim moves
through a group chat until it reads as settled. Often the claim is fine.
Sometimes it is wrong, or true only under conditions nobody passed on. Primer is
for the person on the receiving end: ask it before you decide, and you get the
map of the topic, the evidence under each part, and how far that evidence can be
trusted, so the choice is yours rather than the last confident person's.

## What Primer is

Primer is a standard **Agent Skill**: a folder the agent loads on demand. It
contains a `SKILL.md` — a short instruction file with a name and a description —
plus a `references/` folder with the method and output format it follows. The
agent reads the description to decide when the skill is relevant, then pulls in
the full instructions only when it is, so an idle skill costs nothing. It depends
on no other skill.

## Try it in one conversation

To sample Primer without installing anything, paste this into any agent that can
open public links:

> Read
> `https://raw.githubusercontent.com/nicktongwj/primer-skill/main/SKILL.md` and
> its `references/` files, then follow them to give me a primer on **[topic]**.

This applies Primer for the current conversation only; it does not install the
skill or change any settings. To keep it, install it (below).

## Use it

```
/primer [topic]
/explain [topic]
```

Plain language works too: "explain X", "get me up to speed on X", "give me a
primer on X".

The skill answers at three depths:

- **The map** is the default. A one-paragraph orientation, then what it is, why it
  matters now, what you need to know, the live debates, who matters, the
  vocabulary, and the state of play. It ends with a numbered menu of nodes to
  open.
- **A drill-down** opens one node. Say "go deeper on 3" and the skill expands that
  node alone, with sourced evidence cards.
- **Deep** widens the sources on a single sub-question. When the question is
  really a claim to test, a legal question, a company, or current sentiment, the
  skill says so and points you to the right kind of tool.

## Examples

Real, unedited runs. Each block below is exactly what the skill returned.

<details>
<summary><strong>/primer creatine for brain health</strong></summary>

<br>

**Creatine for brain health: Primer**

> **In one paragraph:** Creatine is proven for muscle strength and is safe for
> healthy people at normal doses. The newer claim that it sharpens a healthy
> person's thinking is much weaker: meta-analyses find only small memory gains,
> concentrated in older, sleep-deprived, or low-baseline people, and Europe's food
> regulator refused the cognition claim in 2024. The standard 5 g gym dose is
> probably too little to move the brain.

**What it is.** Creatine is a compound stored mostly in muscle, with a smaller
amount in the brain, that helps recycle cellular energy (ATP). The body makes
some; meat and fish supply the rest. Supplements are almost always creatine
monohydrate.

**Why it matters now.** A 2026 wellness wave has rebranded creatine from a gym
supplement into a "brain" supplement, so more friends and family are taking it for
focus and memory. The muscle claim and the brain claim do not rest on the same
strength of evidence, and that gap is the whole point.

**What you need to know**

1. **Muscle and strength: settled.** Creatine monohydrate is one of the
   most-studied supplements in existence and reliably improves strength, power, and
   lean mass. This part is not in dispute.
2. **Cognition: small and patchy.** The largest [2024 meta-analysis](https://pmc.ncbi.nlm.nih.gov/articles/PMC11275561/)
   (16 RCTs, 492 people) found a small memory effect (SMD 0.31) plus attention and
   processing-speed gains, but no effect on executive or overall cognition. It was
   formally corrected in February 2025.
3. **Who benefits most: people under strain.** Gains show up mainly when brain
   energy is taxed or baseline creatine is low, such as [older and sleep-deprived people](https://www.alzdiscovery.org/cognitive-vitality/ratings/creatine);
   healthy, rested, meat-eating young adults show little. Vegetarian results are
   mixed.
4. **Dose is the catch.** The brain absorbs creatine poorly, so the 5 g/day
   muscle-maintenance dose is likely too small. Visible cognitive effects tend to
   appear at about 20 g/day or a [single large dose under stress](https://www.nature.com/articles/s41598-024-54249-9).
5. **Regulators are unconvinced.** In November 2024, [EFSA concluded](https://www.nutraingredients.com/Article/2024/12/12/stakeholders-react-to-efsas-health-claim-rejection-of-creatine-for-cognitive-function/)
   that a cause-and-effect link to cognition was not established, and the EU refused
   the health claim; acute memory effects appeared only at 20 g/day, not at 5 g/day.
6. **Safety: reassuring.** At normal doses creatine is safe for healthy people;
   intake at or above 2 g/day is not linked to kidney or liver harm, though anyone
   with existing kidney disease should check first.

**The live debates**

- **Whether it helps a healthy brain at all.** Meta-analyses say a little; a
  [2024 systematic review](https://www.sciencedirect.com/science/article/pii/S0166432824001384)
  and a 2026 "cart before the horse" critique argue the theoretical basis is thin
  and the effect disappears in well-fed, rested young adults.
- **How much you would need.** There is no clinically established brain dose. The
  10 to 20 g/day some researchers propose collides with the 5 g most people
  actually take.

**Vocabulary**

- **Creatine monohydrate** — the standard, cheapest, best-studied form.
- **Effect size (SMD)** — a way to size a result independent of the test; about 0.3
  counts as small.
- **Loading** — a few days at roughly 20 g to fill stores quickly, then a lower
  maintenance dose.

**State of play.** Settled: the muscle benefit and the safety profile. Contested:
any cognitive benefit in healthy people, and the dose it would take. Direction of
travel: the recent high-quality reviews and the EFSA ruling have made the field
more sceptical of the brain claims, not less.

**Go deeper**

1. **The dose question** — 5 g versus 20 g, why brain uptake is slow, and whether
   loading matters.
2. **Older adults and Alzheimer's** — what the clinical trials, including the 2025
   KU Medical Center pilot, actually show.
3. **Sleep deprivation** — the single-dose study, and what it does and does not
   prove.

To pressure-test one specific claim as a straight yes or no (for example,
"creatine improves memory in healthy adults"), use an adversarial claim-testing
pass.

**Confidence:** Medium overall. The muscle benefit and safety are High; the
cognitive claims are Low to Medium and hinge almost entirely on dose and
population.

</details>

<details>
<summary><strong>/primer tech retrenchments attributed to AI displacement</strong></summary>

<br>

**Tech layoffs blamed on AI: Primer**

> **In one paragraph:** Tech layoffs in 2025–2026 are real and large, and companies
> increasingly name AI as the reason. The best evidence says AI is one genuine
> factor among several, not the whole story: the clearest AI fingerprint is a
> squeeze on entry-level and young workers in exposed roles, while economists find
> little sign of broad AI-driven job loss in the aggregate. The stated cause
> shifted to "AI" far faster than the technology improved, which points to some of
> it being narrative.

**What it is.** "AI displacement" here means jobs cut or never created because
software, mostly generative AI, now does the work. It is distinct from cuts driven
by interest rates, post-pandemic overhiring, or budgets being redirected to AI
infrastructure, even when those also get labelled "AI".

**Why it matters now.** 2026 has seen large, continuing tech cuts (about
[142,000 US tech workers in the first five months](https://www.techtimes.com/articles/317392/20250529/tech-layoffs-reach-142000-2026-profitable-companies-cut-jobs-fund-700b-ai-infrastructure.htm)
per trackers), and the share of announcements naming AI has climbed steeply.
Whether AI is the cause or the cover changes what a worker should actually do.

**What you need to know**

1. **The layoffs are real and large.** Scale is not in dispute; the cause is.
2. **Attribution jumped faster than capability.** AI was blamed for
   [roughly 7% of cuts in January and about 40% by May](https://techcrunch.com/2026/07/06/the-running-list-major-tech-layoffs-in-2026-where-employers-cited-ai/),
   while the technology improved only incrementally. That gap is the tell that some
   attribution is strategic.
3. **Economists are sceptical of broad displacement.**
   [Oxford Economics](https://invezz.com/news/2026/05/04/is-big-techs-725b-ai-splurge-being-funded-by-mass-layoffs/)
   found firms "don't appear to be replacing workers with AI on a significant scale",
   and economy-wide employment has kept growing even as the cuts made headlines.
4. **But entry-level is genuinely hit.** The strongest independent evidence,
   Stanford's ["Canaries in the Coal Mine?"](https://digitaleconomy.stanford.edu/publication/canaries-in-the-coal-mine-six-facts-about-the-recent-employment-effects-of-artificial-intelligence/)
   (November 2025, ADP payroll data), finds workers aged 22–25 in the most
   AI-exposed jobs down about 13% since late 2022 while older workers held steady.
   The harm is a closing door for new entrants, which does not register as a
   classic layoff.
5. **"AI washing" is a named phenomenon.** Even Sam Altman concedes "some AI
   washing where people are blaming AI for layoffs that they would otherwise do",
   alongside "some real displacement".
6. **The money is moving to AI, not only away from people.** The biggest cutters
   are redirecting payroll into AI capital spending, so a cut can be an "AI" story
   in a budget sense even when no worker was literally replaced by a model.

**The live debates**

- **Cause or cover.** Is AI driving the cuts, or a convenient, investor-pleasing
  label on ordinary cost-cutting and rate-driven correction? The honest answer is a
  mix; the proportion is what is argued.
- **Displacement versus a frozen ladder.** Aggregate unemployment looks calm, yet
  entry-level hiring is shrinking. Whether that is a temporary adjustment or a
  structural loss of the bottom rung is unresolved.

**Vocabulary**

- **AI washing** — attributing a business decision to AI for narrative or
  share-price reasons.
- **AI-exposed occupation** — a job with many tasks a model can do (coding, support,
  content, QA).
- **Automation versus augmentation** — AI replacing a task versus assisting it; cuts
  cluster in the former.

**State of play.** Settled: the cuts are real, and young workers in exposed roles
are measurably down. Contested: how much of the total is truly AI versus
macroeconomics and narrative. Direction of travel: evidence is firming that the
effect is concentrated at the career entry point rather than across the board.

**Confidence:** Medium overall. The entry-level effect is Medium-High (one strong
study with corroboration); the claim that AI is the main cause of total layoffs is
Low.

</details>

## Install

**Claude Code and other filesystem agents**

```bash
git clone https://github.com/nicktongwj/primer-skill.git ~/.claude/skills/primer
```

**Claude (web or desktop)** — [download the ZIP](https://github.com/nicktongwj/primer-skill/releases/latest/download/primer.zip),
enable Code execution in Settings → Capabilities, then **Customize → Skills → +
Create skill** and upload it.

**Any web app, no install** — create a project, add `SKILL.md` and `references/`
as project knowledge, and tell it to act as Primer. Every chat in that project
uses it.
