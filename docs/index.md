---
title: Home
---

# repoinfo.yml

Tell machines what's related.

Declaratively codify architectural and engineering integrity.

A lightweight open standard for describing repository relationships, stack, and topology.

One file. Any stack. Any era.

[View on GitHub](https://github.com/wallwill/repoinfo)

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

## Examples

Example `repoinfo.yml` files are available for common repository shapes across older and newer enterprise stacks:

- C / Oracle / Unix batch
- Java Struts webapp
- .NET WebForms on IIS
- Java Spring Boot API
- Node / React UI
- Python FastAPI ML service
- Go Kubernetes service

See the [examples](examples.html) page or browse the [`/examples`](https://github.com/wallwill/repoinfo/tree/main/examples) directory.

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

Large software estates are rarely all-modern. Agentic SDLC, platform tooling, and architecture automation need reliable context across legacy batch jobs, enterprise web applications, services, UIs, data pipelines, and cloud-native systems. `repoinfo.yml` gives each repository a small, durable context file without requiring a central catalog first.

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

Read the [specification](spec.html), browse [examples](examples.html), or see how to [contribute](contributing.html).
