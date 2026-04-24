# Contributing to Critical Thinking Partner Protocol

## 1. Proposing a New Protocol Version

A new version proposal is a behavioral change — not a wording preference. Before opening an issue, ask: does this change alter what the model does in a specific, observable situation? If the answer is no, it is a style edit; open a discussion instead.

To propose a new version:

1. Open a Feature Request issue using the issue template in `.github/ISSUE_TEMPLATE/feature_request.md`
2. Identify the specific behavior in the current protocol that the proposal changes, using before/after language (e.g., "Current: the model reconsiders if the user pushes back. Proposed: the model reconsiders only if the user provides a new argument or identifies a specific error")
3. Describe one or more concrete scenarios in which the proposed behavior produces a meaningfully different output than the current version
4. Identify any rule in the existing protocol that the proposed change would conflict with, and state how the conflict is resolved

Proposals that do not include a before/after behavioral description will be closed and asked to resubmit using the template.

---

## 2. Discussion Format for Critique Threads

Critique threads on issues and pull requests follow this structure to keep discussion productive and traceable:

**Claim:** State the specific assertion you are making about the protocol or proposed change — one claim per comment.

**Evidence or reasoning:** Provide the argument, behavioral example, or logical basis for the claim. Assertions without reasoning will be acknowledged but not weighed.

**Condition for revision:** State what would have to be true for you to update your position. This is not optional — a position with no falsification condition is a commitment, not an argument.

Threads that collapse into repetition (the same point made more forcefully without new reasoning) will be summarized and closed by a maintainer. Frustration is not a counter-argument.

---

## 3. PR Checklist

Before submitting a pull request, confirm all of the following:

- [ ] The PR description includes a before/after behavioral description for every protocol change — what the model did under the previous version and what it does under the proposed version, in at least one concrete scenario
- [ ] No verbatim text from an external source has been introduced into the protocol without explicit licensing confirmation
- [ ] The CHANGELOG.md has been updated with the proposed change under an `[Unreleased]` section header, using Keep a Changelog format, with a one-sentence behavioral description of each change
