# repoinfo.yml Specification

Version: `repoinfo/v1`

`repoinfo.yml` is a lightweight, repo-native file for declaring repository identity, stack, and relationships.

## File location

The file should live at the root of a repository:

```text
repoinfo.yml
```

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

## Required fields

### `apiVersion`

Identifies the specification version.

```yaml
apiVersion: repoinfo/v1
```

### `repo`

Describes the repository.

```yaml
repo:
  name: assessment-api
  type: service
```

Required:

- `name`
- `type`

### `stack`

Lists the primary technologies used by the repository.

```yaml
stack:
  - java
  - springboot
```

### `related`

Lists repositories, systems, services, databases, queues, or other components related to this repository.

```yaml
related:
  - assessment-ui
  - assessment-db
  - assessment-events
```

## Extensions

Custom fields should use an `x-` prefix.

```yaml
x-enterprise:
  qualityGate: GATE_00
  agileId: 297538057860d
```

Tools should ignore extension fields they do not understand.

## Principles

- Simple
- Repo-native
- Human readable
- Machine readable
- Backward compatible
- Forward compatible
- Extensible

## Philosophy

Relationships are expensive to infer, cheap to declare.

Inference changes. Relationships persist.
