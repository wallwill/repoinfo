# Contributing to repoinfo.yml

Thank you for your interest in contributing. repoinfo.yml is an open, vendor-neutral standard. No one owns it. Everyone can improve it.

---

## Principles

- The spec should stay lightweight. If in doubt, leave it out.
- Backwards compatibility is non-negotiable. Existing files must never break.
- Declarations over inference. Every addition should make relationships more explicit, not more clever.

---

## Ways to contribute

### Discuss
Open an issue to propose a change, challenge an assumption, or share how you're using repoinfo.yml in the wild. Discussion is contribution.

### Improve the spec
Changes to the core specification require an issue first. Describe the problem you're solving, not just the solution. Small, focused changes are preferred over large ones.

### Share examples
Real-world examples from real stacks are the most valuable thing you can add. Open a PR adding an example to the `/examples` directory.

### Fix documentation
Typos, clarity improvements, and better examples are always welcome and can go straight to a PR.

---

## Making a pull request

1. Fork the repo and create a branch from `main`.
2. Make your changes.
3. Open a pull request with a clear description of what you changed and why.
4. Be patient and open to feedback.

---

## Spec change process

Core spec changes follow this process:

1. **Open an issue** describing the problem and proposed change.
2. **Discussion period** — at least 14 days for community input.
3. **Consensus** — changes should have clear support and no strong objections.
4. **PR** — once consensus is reached, a PR implements the change.
5. **Version bump** if the change affects the schema.

Changes that break backwards compatibility will not be accepted.

---

## Extensions

If you need something the core spec doesn't cover, use the `x-` prefix. You don't need to open an issue for this — extensions are intentionally ungoverned. If your extension proves widely useful, bring it back as a proposal for the core spec.

---

## Code of conduct

Be direct. Be kind. Assume good intent. This is a small project and everyone here is trying to make something useful.

---

## Questions

Open an issue. There are no wrong questions.
