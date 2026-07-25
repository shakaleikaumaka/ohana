# 💰 Billing & Models — the two-lane system (Taurus)

## Lane 1 — `subscription/` prefix (no wallet drain)
Rides the user's Anthropic subscription, not the Taurus wallet. Subject to subscription rate limits.
Used for: personal/governance seats (Private JAI historically, Shaka PA).

## Lane 2 — `openrouter/` prefix (wallet-billed)
Raw OpenRouter cost + 25% platform fee, deducted from a prepaid wallet per message.
Used for: workers, builders, scouts, councils.

## The routing strategy
- **High-volume workers/builders** → `openrouter/moonshotai/kimi-k3` (pennies per big build; DASH + PIT BOY + most of the family)
- **Governance/deep reasoning** → subscription lane where possible
- **NEVER** put premium models (claude-fable-5 ≈ $10/$50 per Mtok) on openrouter lane for routine loops — fan-out agentic loops multiply token burn.

## Model ID gotchas
- Dots, not dashes: `openrouter/anthropic/claude-sonnet-4.6` ✅ (not `claude-sonnet-4-6`)
- `claude-3-haiku` is deprecated (404) — don't use.
- Watch for model-revert drift after platform updates.
