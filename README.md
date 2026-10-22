# CTO Relationship Intelligence

**Executive research and relationship strategy for CTO-level conversations.**

A skills-driven meeting-preparation assistant for technology leaders building relationships with founders, CEOs, CTOs, investors, executives, and strategic partners. It connects business insight with genuine technical depth—**without turning every conversation into a software-services sales pitch**.

Maintained by **CoderzHunt**. Source version: **v1.0.0**.

## What it does

- **Research people and companies:** professional background, positioning, business model, recent activity, and publicly supported technology signals.
- **Keep evidence separate from inference:** prioritize verifiable sources, explain confidence, and avoid manufacturing customer or funding claims.
- **Map relationship opportunities:** mutual interests, knowledge exchange, product strategy, potential collaboration, and longer-term engineering needs.
- **Develop two Technology Plays:** two specific, evidence-backed technical opportunities with disconfirmation research, adoption checks, high-level architecture, pilot paths, risks, and conversation triggers.
- **Steer a meeting:** opening direction, intelligent questions, topics to avoid, possible technical bridges, and a natural conclusion.
- **Create Parakeet AI instructions:** context and live trigger logic for a CTO to use during the conversation.
- **Close the loop:** work from prior discussions, analyze meeting outcomes, and plan thoughtful follow-ups.

## Source files

```text
cto-relationship-gpt/
├── README.md
├── plugin.json
├── .codex-plugin/
│   └── plugin.json
├── skills/
│   └── cto-relationship-intelligence/
│       └── SKILL.md
└── docs/
    └── INSTALL.md
```

The complete workflow is in **[SKILL.md](skills/cto-relationship-intelligence/SKILL.md)**. The two manifests preserve the original plugin metadata and CoderzHunt authorship.

## Setup

See **[Installation & usage](docs/INSTALL.md)**.

```bash
git clone https://github.com/cognetheus/cto-relationship-gpt.git
cd cto-relationship-gpt
```

This is a **skill/instruction package**, not a standalone chat app, background service, or preconfigured web-scraper. To run it, load the skill in an AI-agent environment compatible with skill files, following that host's own installation instructions.

Cloning the GitHub repository does not install, enable, or grant permissions to a private ChatGPT plugin.

## Example prompts

```text
Research this CTO and their company. I'm meeting them for the first time.
Focus on genuine technical overlap, two Technology Plays, and useful
questions—not a pitch.
```

```text
Prepare Parakeet AI meeting instructions in Markdown. Include what to listen
for, technical questions, live triggers, and what topics to avoid.
```

```text
Analyze these conversation notes and suggest a relationship-first follow-up,
with evidence-backed collaboration possibilities.
```

## Operating principles

1. **Relationships before selling.** The purpose is an informed executive conversation, not an unsolicited proposal.
2. **Evidence over invented certainty.** Distinguish confirmed information, inference, and unknowns.
3. **Disconfirm your own ideas.** Before proposing a technology opportunity, investigate whether the organization already has it.
4. **Be technically useful.** Surface relevant architectures, constraints, proof-of-concept options, and business implications.
5. **Respect privacy.** Use information the user is authorized to share and sources that can be accessed legitimately.

## Ownership and license

Original plugin author: **CoderzHunt**. Repository maintained under [cognetheus](https://github.com/cognetheus).

**No open-source license is granted by default.** Public repository visibility is not a license for modification, redistribution, or commercial reuse. Contact the maintainer about permissions.

---
*The source here is independently maintained; publishing it does not change the distribution or edit permissions of the original ChatGPT plugin.*
