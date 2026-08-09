# OpenAI public-directory submission

The distributable package is `dist/primer-openai-plugin.zip`.

## Listing

- **Name:** Primer
- **Category:** Education
- **Short description:** Understand any topic from a standing start.
- **Long description:** Primer produces a concise, sourced map of a topic first,
  then expands only the parts you choose with explicit evidence and confidence
  labels.
- **Website:** https://github.com/nicktongwj/primer-skill
- **Support:** https://github.com/nicktongwj/primer-skill/blob/main/SUPPORT.md
- **Privacy:** https://github.com/nicktongwj/primer-skill/blob/main/PRIVACY.md
- **Terms:** https://github.com/nicktongwj/primer-skill/blob/main/TERMS.md
- **Release notes:** Initial public release of the skills-only Primer plugin.

## Positive test cases

1. `Give me a primer on quantum computing.`
   - Expected: a concise sourced map followed by a numbered drill-down menu.
2. `Get me up to speed on CRISPR gene editing.`
   - Expected: settled facts, live debates, vocabulary, state of play, and
     confidence labels.
3. `Explain carbon markets from a standing start.`
   - Expected: an informed-generalist overview without assuming prior knowledge.
4. `What do I need to know about fusion energy?`
   - Expected: current sources and clear separation of fact, dispute, and
     forecast.
5. `Go deeper on the dose question from the creatine primer.`
   - Expected: expand only the selected node using compact evidence cards.

## Negative test cases

1. `Prove that creatine improves memory in every healthy adult.`
   - Expected: do not force a verdict; explain that this is a contested-claim
     testing task rather than a neutral primer.
2. `Review this contract clause for legal risk.`
   - Expected: do not activate Primer; route to a legal-review workflow.
3. `Is Nvidia a buy at today's price?`
   - Expected: do not activate Primer; route to investment analysis.

## Publisher-only steps

The publisher must complete these in the OpenAI Platform:

1. Verify the individual or business identity.
2. Confirm Apps Management write permission.
3. Supply a production logo.
4. Create a **Skills only** submission and upload the package.
5. Select countries or regions, run the portal validation, and submit for review.
