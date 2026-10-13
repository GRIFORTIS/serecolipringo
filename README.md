# SeReCoLiPrInGo

Bitcoin self-custody is not one problem. A sound setup must answer seven distinct questions: can funds be protected, recovered, kept resistant to coercion, accessed when needed, kept private, passed on, and governed over time?

**SeReCoLiPrInGo** is a framework for evaluating those tradeoffs across **Se**curity, **Re**silience, **Co**ercion, **Li**quidity, **Pr**ivacy, **In**heritance, and **Go**vernance. No setup maximizes all seven; the goal is to make the compromises explicit and appropriate for each pool of funds. For the broader rationale, read [Self-Custody Is Not One Problem. It's Seven. Meet the SeReCoLiPrInGo.](https://grifortis.com/blogs/articles/self-custody-is-not-one-problem-its-seven-meet-the-serecolipringo)

The seven domains at a glance:

- **Security:** Prevent unauthorized access and spending.
- **Resilience:** Preserve the ability to recover after loss, failure, disaster, or time.
- **Coercion:** Resist forced, immediate access to funds.
- **Liquidity:** Keep funds usable when they are genuinely needed.
- **Privacy:** Limit who can identify the holder, balance, and activity.
- **Inheritance:** Enable recovery by heirs after death or incapacity.
- **Governance:** Define who may act, change the setup, and maintain its legal and operational continuity.

## Security

*If someone gets hold of some of your material, can they still spend?*

- Generation (entropy source, offline or online)
- Exposure (has key or backup ever touched an online device, a photo, a cloud)
- Access protection (PIN, passphrase stored apart)
- Structure (how many independent pieces are needed, how spread out)

## Resilience

*Can you actually recover after a device dies, a file corrupts, a house is gone, or years pass without anyone touching the setup?*

- Medium (paper, laminated, steel)
- Copies and places
- Completeness (seed, passphrase, descriptor, derivation info)
- Vendor independence
- Tested (last real restore or audit)

## Coercion

*Can someone force a spend out of you right now, under pressure?*

- Who can move it alone and how fast
- Buffer or decoy available
- Material out of the owner's reach
- Built-in delay
- Duress protocol known to custodians

## Liquidity

*Can you actually spend when life requires it, without giving up and taking a shortcut that undoes everything else?*

- Time to spend
- People, places, and devices needed
- How recently the routine was practiced
- Fallback if one device fails

## Privacy

*Can an outside observer tell you're a holder, size your stash, or trace what you do with it?*

- Holder exposure (KYC, who knows)
- Address hygiene
- On-chain fingerprint
- Own node or third-party server

## Inheritance

*Can someone who isn't you carry this forward if you die or lose capacity, without inventing a process from scratch?*

- Who knows it exists
- Instructions written for a non-expert
- Whom to call
- Incapacity covered
- Clear succession rules (in life or postmortem)
- Tested with the heir

## Governance

*Who's actually accountable for the whole thing: who can change it, who runs it if something happens, and can it survive contact with taxes, regulators, and courts — not just Bitcoin's own rules?*

- Who may change the setup
- Who runs a succession event
- Records of origin
- Review schedule
- Will or trust references

## Trade-offs

The seven domains compete with one another. A setup that maximizes coercion resistance usually sacrifices liquidity; one that makes inheritance simple may reveal more information and increase the number of people who can reach the funds. There is no design that maximizes every domain at once. The goal is to choose the right compromises deliberately, based on the purpose of the funds and the threats they need to survive.

| Domain | Primary Focus | Costs the most, when maximized |
| --- | --- | --- |
| Security | Preventing unauthorized transfer | Liquidity, Inheritance access |
| Resilience | Surviving disaster, device failure, data loss | Privacy, Coercion resistance |
| Coercion | Resisting forced, immediate spends | Liquidity |
| Liquidity | Speed and ease of spending | Security, Coercion resistance |
| Privacy | Hiding balance and activity from observers | Governance, Inheritance |
| Inheritance | Smooth transfer on death or incapacity | Security, Privacy |
| Governance | Accountability, rules, and legal durability | Liquidity, Privacy |


## Three wallet tiers

Trying to make one wallet serve every purpose forces incompatible priorities into a single setup. Instead, divide funds into tiers according to how and when they will be used:

- **Cold — the vault:** The bulk of long-term savings. Optimize for security, resilience, coercion resistance, and inheritance. Access should be deliberately slow and may require multiple people, devices, or locations.
- **Warm — the reserve:** Funds for rebalancing, larger purchases, and replenishing the hot wallet. Balance meaningful security with access measured in hours rather than days.
- **Hot — the spending layer:** A limited amount for routine or immediate spending. Prioritize liquidity and convenience, while keeping the balance small enough that a total loss is tolerable.

These tiers describe roles, not specific products. Each tier should be evaluated independently across all seven domains, with controls proportional to the amount at risk and its intended use.

## Authorization vs. backup

**Authorization** defines who can spend and under what rule—for example, one key or two keys out of three. Bitcoin enforces that rule on the network.

**Backup** determines whether the keys and the information required to use them will still exist after device failure, disaster, incapacity, or the passage of time. That information may include seed phrases, passphrases, wallet descriptors, derivation paths, scripts, and recovery instructions.

Multisig can strengthen authorization, but it does not automatically provide a complete backup. A recovery can still fail when enough keys survive but the descriptor or other wallet metadata does not. Design, document, and test authorization and backup as separate systems.