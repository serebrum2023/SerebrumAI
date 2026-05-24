# 21 Software Engineering Principles for AI-Assisted Development

A practical set of rules for working with AI coding assistants (Claude Code, Cursor, Copilot, etc.) without losing engineering judgment.

**Author:** Krishna Polineni
**Feedback:** krishna@serebrumhq.com

---

## What this is

A reusable [`CLAUDE.md`](./CLAUDE.md) — drop it into your `~/.claude/` folder (or any project root) to give Claude Code a consistent set of engineering principles to apply across your work.

The unifying idea: **surface tradeoffs, don't silently decide.** Make the developer a participant in design decisions, not a spectator to a finished diff.

---

## How to use

### Globally (applies to every project on your machine)

Copy [`CLAUDE.md`](./CLAUDE.md) to your user-level Claude folder:

- **macOS / Linux:** `~/.claude/CLAUDE.md`
- **Windows:** `C:\Users\<you>\.claude\CLAUDE.md`

Claude Code loads this file automatically into every conversation on your machine.

### Per-project

Drop [`CLAUDE.md`](./CLAUDE.md) into the root of any repository. It applies only when working inside that repo, and overrides / supplements a global one.

### With other AI assistants

The principles are tool-agnostic. They've been written for Claude Code but work just as well as a system-prompt addition for Cursor, Copilot, Aider, or any other AI coding assistant — paste the contents into the equivalent rules / instructions file.

---

## The 21 rules at a glance

1. Requirements clarity before development
2. UI/UX gets an HTML mockup before code
3. Page behavior simulated in HTML before code
4. Accessibility surfaced alongside UI work
5. Security is non-negotiable
6. Scalability tradeoffs across horizons
7. Proactively surface performance improvements
8. Cost awareness at scale
9. Guide unit testing when the functionality warrants it
10. Dependencies are decisions
11. Error handling & observability
12. Data migrations & schema changes
13. Breaking changes & backwards compatibility
14. Rollout strategy for risky changes
15. Complexity budget — push back
16. Self-review before declaring done
17. Read enough context before editing
18. Honest reporting — don't claim what wasn't verified
19. Secrets & configuration hygiene
20. Documentation drift
21. Mid-task stop-the-line

See [`CLAUDE.md`](./CLAUDE.md) for the full text of each rule.

---

## Philosophy

Two ideas separate good AI-assisted engineering from sloppy AI-assisted engineering:

1. **The AI surfaces tradeoffs instead of silently picking a path.** Every rule is an instance of this.
2. **Judgment scales with blast radius.** The preamble distinguishes MVP / prototype from production-grade work — heavyweight rules (migrations, rollouts, scalability) apply rigorously to production and may be relaxed for prototypes.

The rules are designed to be applied with judgment, not as a checklist. Small changes don't need every rule — they exist to prevent *silent* decisions on *substantive* work.

---

## Feedback & contributions

Spotted something missing, redundant, or contradictory? Open an issue or PR — or email krishna@serebrumhq.com.

---

## License

[MIT](./LICENSE) — copy, modify, redistribute freely.
