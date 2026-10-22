# Installation and Usage

This repository contains the **CTO Relationship Intelligence v1.0.0 skill** and metadata for compatible agent hosts. It is not an independently executable application.

## Clone the source

```bash
git clone https://github.com/cognetheus/cto-relationship-gpt.git
cd cto-relationship-gpt
```

### What is included

- `skills/cto-relationship-intelligence/SKILL.md` — the complete operating workflow and response formats.
- `plugin.json` — portable agent-plugin metadata.
- `.codex-plugin/plugin.json` — compatibility metadata for hosts supporting that manifest format.

The repository requires no Python or Node dependencies merely to read the source. You need an AI-agent runtime to execute the skill.

## Use the skill in a compatible agent host

1. Follow your agent host's official guidance for importing Agent Skills.
2. Add the `skills/cto-relationship-intelligence` directory, preserving the `SKILL.md` filename.
3. Enable only the tools and data connectors you are prepared to authorize for that host. The skill does not grant access by itself.
4. Ask the agent to use **CTO Relationship Intelligence** for meeting research, strategic preparation, or follow-up analysis.
5. Give the person/company and relevant public URLs. Optionally include existing relationship context, earlier messages, meeting details, and what would constitute a useful outcome.

Not every AI host understands the manifests or automatically discovers the skill. Consult the supported host's documentation. This source repository does **not** install the original private ChatGPT plugin or convert it to a publicly installable plugin.

## Prepare a first meeting

Start with a prompt such as:

```text
Use CTO Relationship Intelligence.

Person: [name, title, LinkedIn]
Company: [name, website]
Meeting purpose: Build a CTO-to-founder relationship and explore real
technology/product overlap. This is not a sales call.

Please provide:
- Verified person and company research with sources and caveats
- Recent signals worth discussing
- Exactly two Technology Plays, checking whether either is already in use
- Technical/business questions to ask
- Conversation steering and topics to avoid
```

## Prepare Parakeet AI instructions

```text
Using the research and context above, generate concise Parakeet AI
live-meeting instructions in Markdown:
- Person and company context
- Positioning and relationship goal
- Two Technology Plays with strong/weak/negative triggers
- Listening cues and technical questions
- What not to claim or pitch
```

## Handle information responsibly

- Ask permission before using private correspondence, meeting transcripts, or CRM notes.
- Do not upload secrets, confidential engineering documents, or personal contact lists to services without appropriate authorization.
- Avoid fabricated market claims or claims that a company has implemented a technology when it has not been verified.
- Be mindful of platform terms and the difference between public professional information and private user data.

## Update the source

Edit `skills/cto-relationship-intelligence/SKILL.md` and review the two manifest files for consistency. Changes to GitHub source do not automatically update any separately installed plugin release.

Current source version: **1.0.0**.
