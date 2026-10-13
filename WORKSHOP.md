# SeReCoLiPrInGo workshop

Seven tables build a questionnaire for evaluating Bitcoin self-custody. Each table owns one domain:

- Security
- Resilience
- Coercion
- Liquidity
- Privacy
- Inheritance
- Governance

The work happens in public GitHub issues. Submit one issue per proposed question, then help another table test and improve its questions.

## Safety rule

Use only fictional examples. Never publish real seed words, passphrases, wallet addresses, balances, identities, storage locations, recovery instructions, or details of your own setup.

## Build round

1. Open your table's domain anchor in the repository's [issue list](https://github.com/GRIFORTIS/serecolipringo/issues).
2. Review the domain question and suggested factors.
3. Select the matching domain form from [New issue](https://github.com/GRIFORTIS/serecolipringo/issues/new/choose).
4. Submit one issue for each proposed questionnaire question.

Every proposed question should:

- ask about a fact of the setup, not how safe someone feels;
- measure one factor;
- use answer choices ordered from worst to best;
- include `I don't know`, scored `0`;
- score the home domain from `0` to `5`;
- identify any answer that caps the domain score; and
- identify effects on other domains as `-1`, `0`, or `+1`.

Do not calculate an overall score. Each domain remains a separate `0`–`5` result.

## Critique round

Move to the domain assigned by the facilitator. Read its proposed-question issues and comment using this format:

```text
Clarity:
Answer ordering:
Missing answer:
Breaker or cap:
Cross-effects:
Suggested revision:
```

Look especially for:

- wording that requires expertise or invites a self-rating;
- two factors hidden inside one question;
- answer choices that overlap or are not in a clear order;
- a fatal weakness that should cap the score;
- consequences for other domains; and
- requests for real amounts, identities, or locations.

## Merge round

GitHub issues are not literally merged. In this workshop, merging means:

1. revise the strongest issue using the critique;
2. mark that issue `status: accepted`;
3. close overlapping alternatives as duplicates and link to the accepted issue; and
4. add the accepted issue to the domain anchor's final checklist.

The facilitator or another repository maintainer applies status labels. Participants do not need repository permissions beyond the ability to open and comment on issues.

## Definition of done

An accepted question has:

- one clear factor;
- wording a non-expert can answer;
- ordered, scored answers including `I don't know — 0`;
- an explicit breaker or a statement that none is proposed;
- cross-effects for every affected domain; and
- a result for at least one fictional test persona.

The output of the workshop is the set of accepted issues linked from the seven domain anchors.
