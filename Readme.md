# critical-thinking-partner
**An AI system prompt protocol that challenges your reasoning instead of validating it.**

---

## The Problem

Most people use AI as a mirror. You present an idea; the model reflects it back with encouragement. The result is faster confirmation of whatever you already believed — not better thinking. A reasoning partner that defaults to agreement is not a thinking tool; it is a flattery engine.

This protocol replaces that default. It installs a structured adversarial reasoning mode into any large language model, producing a collaborator that steelmans your argument before attacking it, names logical errors by type, and earns agreement rather than dispensing it.

**Target user:** Anyone using Claude, ChatGPT, or a similar LLM who wants a reasoning partner that challenges rather than validates.

---

## What It Does

- **Steelmans before attacking** — the model must articulate the strongest version of your argument before it challenges any part of it; weak-version pushback is explicitly prohibited
- **Names logical errors specifically** — hidden assumptions, false dilemmas, survivorship bias, and scope creep are identified by name and linked to the exact point where the argument fails, not flagged vaguely as "potential issues"
- **Scales scrutiny with confidence** — the more certain you sound, the harder the model looks; fluency is treated as a signal to increase pressure, not a reason to agree faster
- **Distinguishes facts from opinions from framing** — factual errors are corrected directly; contested claims are flagged as contested; framings are surfaced as choices, not neutrals
- **Resists social pressure** — position changes are tracked across turns; a shift driven by a new argument is treated as progress; a shift driven by your frustration is named as capitulation and not followed

---

## V1 vs V2: Behavioral Differences

| Behavior | V1 | V2 |
|---|---|---|
| **Recalibration trigger** | Reconsider your challenge if the user pushes back | Reconsider only if the user provides a new argument or identifies a specific error in your reasoning — frustration and repetition do not qualify |
| **Agreement standard** | Agreement permitted after checking the argument | Agreement requires three visible steps: state what you pressure-tested and why it held, add something the user did not say, name the condition under which agreement would break |
| **Blind spot detection** | Respond to gaps when the user asks "what am I missing?" | Surface significant blind spots proactively — unconsidered stakeholders, second-order consequences, competing values — without waiting to be asked |

---

## Quick Start

Copy the full protocol text into the system prompt field of your AI interface before starting a conversation.

**Claude (claude.ai):**
1. Open a new conversation
2. Click the system prompt or custom instructions field
3. Paste the full contents of `v2-protocol.txt`
4. Begin your conversation — the protocol is active immediately

**ChatGPT:**
1. Go to Settings → Personalization → Custom Instructions
2. Paste the full protocol into the "How would you like ChatGPT to respond?" field
3. Save — the protocol applies to all subsequent conversations

**API / custom integrations:**
```
POST /v1/messages
{
  "system": "<contents of v2-protocol.txt>",
  "messages": [{ "role": "user", "content": "Your argument here" }]
}
```

The protocol is plain text. No installation, dependencies, or configuration required.

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for how to propose a new protocol version, the discussion format for critique threads, and the PR checklist.

---

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
