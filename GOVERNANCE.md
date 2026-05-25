# Governance

`repoinfo.yml` is an open, vendor-neutral specification.

The project aims to stay small, backwards compatible, and practical for real repositories across old and new stacks.

## Spec changes

Core specification changes should start with an issue that describes the problem being solved.

After discussion, accepted changes are made through a pull request. Changes that affect the schema should include a version bump and changelog entry.

Backwards compatibility is a core project constraint. Existing valid `repoinfo.yml` files should continue to work.

## Extensions

Organization-specific fields should use the `x-` prefix.

Extensions do not need approval. If an extension proves broadly useful, it can be proposed for the core specification.
