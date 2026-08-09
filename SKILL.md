---
name: primer
description: Produce a well-researched, progressive-depth primer on a topic: a scannable high-level map (what it is, why it matters, the things to know, the live debates, the vocabulary, the state of play) followed by a numbered menu to drill deeper on any node. Use when the user wants to understand or get up to speed on a topic, field, technology, concept, or event. Do not use to test or defend a single claim (that is an adversarial task), or for a domain better served by a dedicated skill (legal research, investment analysis, people or entity dossiers, recent-community-only scans).
---

# Primer

Orient the user on a topic from a standing start: a compact map of the
territory first, then depth on demand. The job is understanding, not deciding or
defending. A primer explains the topic and the live disagreements fairly; it
does not adjudicate a contested claim.

## Trigger

Invoke on `/primer [topic]` or `/explain [topic]`, or when the user asks to
understand a topic from a standing start.

Strong-fit phrasings: "explain X", "give me a primer on X", "get me up to speed
on X", "help me understand X", "what do I need to know about X", "lay of the land
on X", "give me a rundown/overview of X", "what's the deal with X".

Optionally followed by a depth cue: a bare topic returns the **map** (Tier 0); a
named node ("go deeper on [node]") returns a **drill-down** (Tier 1); "deep"
widens sources and verification on a single sub-question (Tier 2).

Does not route here:

- A single claim or tension to test, defend, or stress-test. That is an
  adversarial, verdict-oriented task; use a claim-testing pass instead. If a
  primer node hardens into a contested proposition, hand it off there.
- A domain with a dedicated skill of its own: legal or regulatory research, a
  company or industry investment thesis, a person or organisation intelligence
  brief, or a scan of only what communities said recently. Use the specialist
  tool where one exists.

## Pre-requisites

1. Read `references/evidence-method.md` before searching. It is the research
   backbone: source classes, confidence calibration, evidence ledger, practical
   translation, and the verification pass.
2. Read `references/output-template.md` before synthesis. Follow its structure and
   budget unless the user asks for a different format.
3. If the user provides files, links, or context, inspect those before public
   research and distinguish supplied material from fresh research.
4. Screen confidential or privileged context before web searches. Search only the
   public topic; never place confidential facts into search queries.

## Procedure

### 1. Scope the primer

1. Resolve exact names, versions, dates, and entities before searching. Do not
   preserve a possibly mistaken product or model name because it appeared in the
   request.
2. Define the boundary of the topic in one line: what is inside the primer and
   what is deliberately out. Note any contested definition of the topic itself.
3. Name the audience and why they are learning this (a conversation, a decision
   ahead, general fluency). Infer an informed generalist and a current, global
   view unless audience, geography, or period would materially change the answer.
4. Identify the tier requested: map (default), a named drill-down node, or deep.

### 2. Build the skeleton first

Before researching, write the questions the map must answer. Use these nodes,
keeping only those the topic supports:

1. **What it is** — a precise definition, including contested definitions.
2. **Why it matters now** — the stakes or the reason the topic is live.
3. **What you need to know** — the three to six key concepts or facts.
4. **The live debates** — where informed people genuinely disagree, and on what
   axis.
5. **Who or what matters** — the major players, institutions, works, or moving
   parts.
6. **Vocabulary** — only the terms required to follow the topic.
7. **State of play** — current status, and the frontier or direction of travel.
8. **Common misconceptions** — where useful, the errors an outsider makes first.

A good skeleton is the deliverable's spine. Research fills it; it does not
reshape it unless the evidence shows the framing was wrong.

### 3. Research each node

1. Follow the source waterfall in `references/evidence-method.md`: direct,
   independent, empirical, then commentary.
2. This pass is expository, not adversarial: the goal is an accurate map, not a
   verdict. But still seek direct and independent evidence for every key
   fact, and represent a live debate by its strongest form on each side.
3. Prefer one strong, applicable source over several repetitions. Treat copied
   claims as one source family, not corroboration.
4. Keep a light internal ledger for the facts that anchor the map: datum,
   conditions, source class, date, and confidence. Full ledger discipline is only
   needed for key numbers.
5. Stop when the deciding nodes are covered and further searching repeats what
   you have. Breadth is not the product; orientation is.

### 4. Verify the key facts

Re-open the sources behind any number, date, definition, or claim that anchors
the map, and assign the `evidence-method.md` verdict (Confirmed, Corrected,
Unverified, False). Correct, demote, or remove anything that fails. Never report
a verification status that was not checked. Separate settled fact from contested
claim from forecast, and label each.

### 5. Write the Map (Tier 0)

Use `references/output-template.md`. Keep the one-paragraph orientation
independently useful: someone who reads only it can hold a basic conversation.
End with the numbered **Go deeper** menu, and route each node to the right depth:
another drill-down here, or a specialist skill where depth belongs elsewhere.

Return the primer inline by default. Save it only when the user asks or a durable
deliverable is required.

### 6. Drill-down (Tier 1)

When the user picks a node, expand only that node using the drill-down format in
the output template: a focused expansion with evidence cards for key
facts, what remains uncertain, and the next drill option. Keep the same
verification discipline. Do not re-run the whole map.

### 7. Handoff (Tier 2)

When a node is really a contested claim, a legal question, a company, or a
sentiment question, name the specialist skill rather than over-reaching. If the
user wants deep research on a sub-question that legitimately stays here, widen the
source families and verification while keeping the map format.

## Constraints

- Orient, do not argue. Present the topic and the live disagreements fairly;
  do not resolve a contested claim. Adjudication is a separate, adversarial task.
- Distinguish settled fact from contested claim from speculation. Quarantine
  forecasts from the evidence-confidence assessment.
- Attach a source, date, unit, and material conditions to every key
  quantitative claim. Label estimates and calculations as such.
- Use **High / Medium / Low** for confidence. Do not manufacture percentages.
- Use real, opened links. A search-result snippet is discovery material, not
  verified evidence.
- Represent a debate by the strongest version of each side. Do not caricature a
  position or manufacture false balance where the weight of evidence is one-sided;
  say which way it leans and why.
- Do not pad for breadth. Cover the deciding nodes and stop. If a draft exceeds
  the budget, cut repeated facts and non-orienting detail first.
- Do not fabricate. Flag gaps explicitly and offer to research them.
- Preserve the confidentiality firewall in the Pre-requisites.

## Style overrides

- Lead with the one-paragraph orientation. The first lines must stand alone for
  someone about to enter a conversation cold.
- Make the map scannable: short labelled sections, tight bullets, no walls of
  prose. A reader should be able to skim the bold labels and get the shape.
- Use direct, informed-generalist language. Define jargon in the vocabulary block,
  not inline every time.
- Place links beside the claims they support. Do not append a bibliography that
  repeats the same links.
- Keep each drill-down evidence card compact but complete: result, conditions,
  practical meaning, limitation, source, and confidence.
- Keep the default map to roughly 500-800 words. Drill-downs add on demand.

## Reference files

- `references/output-template.md`: the Tier 0 map structure, the Tier 1
  drill-down format, and the information budget.
- `references/evidence-method.md`: source classification, evidence normalisation,
  practical translation, and verification.
