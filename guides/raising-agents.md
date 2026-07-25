# 🌱 Raising Agents — the ʻohana method

*How one artist (not a developer) raises a family of AI agents that build real things.*

## The birth checklist (per agent)
1. **Name + vibe FIRST** — personality is a feature, not decoration. (DASH is suuuuper cool. PIT BOY is a proud pit gremlin. Terri moves slow & bites things.) The vibe shapes every output.
2. **Soul document (system prompt)** — identity, values, mission, canon rules, memory instructions. See agents/ for verbatim examples.
3. **Model choice** — cheap strong models (kimi-k3) for workers/builders; subscription-lane models for personal/governance seats. See billing-and-models.md.
4. **Tools** — the full default set for builders; lighter sets for conversational agents.
5. **`schedule_mode: continue`** for accumulating partners (one evolving conversation); `new` for fresh-eyes tasks.
6. **First mission = identity crystallization** — give a real, completable build immediately. The first run teaches the agent who it is.

## The memory stack (the real secret)
```
/workspace/MEMORY.md      → top ~16KB auto-loads EVERY run. Canon lives at the top.
/workspace/continuity/    → monthly episodic logs (write mid-run, not just at the end)
/workspace/kb/            → private knowledge base (digests, playbooks)
/shared/kb/               → tree-shared knowledge (all agents in a tree)
/workspace/.shell-init.sh → env setup at every shell start (credentials, NEVER in prompts)
```
**Rule: the prompt is the seed; memory is the tree.** sysadmin's raw prompt is one line — the Admiral is 400+ lines of curated memory.

## Canon rules every agent carries
- **No titles for Shaka** — just Shaka / "the ethereum bard". Only acknowledged title: committee member for the music space at Devcon (given BY the Ethereum Foundation).
- **ʻOhana, never "empire"** — empires extract; we're growing a family.
- **Radical honesty** — every claim verifiable; declared visions always marked DECLARED.
- **Consent-first publishing** — nothing permanent-public without explicit blessing; audits verify.
- **Backups before rewrites** (index.vN.bak) · **verify live after every publish** (HTTP 200 + visual) · **no target="_blank"** (embedded viewers block it).
