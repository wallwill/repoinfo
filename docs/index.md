# repoinfo.yml

Tell machines what's related.

Declaratively codify architectural and engineering integrity.

A lightweight open standard for describing repository relationships, stack, and topology.

One file. Any stack. Any era.

---

## Example

```yaml
apiVersion: repoinfo/v1

repo:
  name: assessment-api
  type: service

stack:
  - java
  - springboot

related:
  - assessment-ui
  - assessment-db
  - assessment-events
```

---

## Why?

Repositories contain relationships that are difficult to infer reliably.

Examples include:

- APIs
- UIs
- databases
- queues
- services
- ownership
- solution topology

`repoinfo.yml` provides explicit repository context for humans, tooling, and AI systems.

---

## Principles

- Lightweight
- Human readable
- Machine readable
- Repo-native
- Optional
- Extensible
- Backward compatible
- Forward compatible

---

## Extensions

Organizations can extend the format freely without affecting the core specification.

```yaml
x-enterprise:
  ApplicationID : APPID003232
```

---

## Philosophy

Relationships are expensive to infer, cheap to declare.

Inference changes. Relationships persist.

---

## Status

Early draft specification.

Contributions, discussion, and experimentation welcome.
