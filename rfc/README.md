# RFC Process

This folder holds proposals under community discussion — draft guidance that isn't yet adopted. Anything here should be treated as a starting point for debate, not settled practice.

## Where Discussion Happens

Proposals are drafted and discussed on [HackMD](https://hackmd.io), not primarily through GitHub pull request review. HackMD lowers the bar for community members (Professors, TOs, judges) to read and comment without needing a GitHub account or git familiarity — which matters more here than it does for the rest of this repo, since the whole point of an RFC is getting feedback from people who may never otherwise touch this repository.

Each RFC file in this folder links to its corresponding HackMD document, where the live discussion happens.

## GitHub Stays the Source of Truth

The copy in this repo is canonical, not the HackMD doc. HackMD is the working surface during open review; it is **not** kept in continuous two-way sync with the file here, since that reliably drifts and leaves nobody sure which copy is current.

Instead: once a round of discussion on HackMD settles into concrete changes, those changes get pulled back into this repo as a normal, deliberate pull request — same as any other change to this repo. The file here always reflects the last point someone chose to sync, not necessarily the very latest HackMD edit.

## Lifecycle

1. **Draft** — proposal is written and added here, seeking review.
2. **Discussion** — feedback happens on the linked HackMD doc (and/or PR comments on this repo).
3. **Revision** — settled changes are periodically pulled back into the file here via PR.
4. **Resolution** — once the community reaches consensus (or the proposal is dropped), the document either moves out of `rfc/` into the appropriate guide location, or is archived/closed with a note explaining the outcome.

## Content Requirements

Same [AI usage policy](../CONTRIBUTING.md#ai-usage-policy) as the rest of the repo: substantive content is human-originated. AI assistance drafting or editing an RFC happens at the author's explicit direction, turn by turn — not by generating proposal content unprompted.
