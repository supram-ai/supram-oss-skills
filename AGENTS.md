# Repository Maintainer Instructions

This repository owns runner-neutral maintained skills and a curated discovery registry. Consumer workflow belongs to harness-eng, Pi/HaPi, or another integration.

## Maintained Skills

- Follow <https://agentskills.io/specification>.
- Keep each maintained skill under `skills/<name>/SKILL.md`.
- Validate frontmatter, instructions, examples, and referenced files before merge.
- Record provenance and license for imported material.
- Do not embed fast-changing external API documentation.
- Preserve useful Git history when migrating or renaming skills.

## Registry

- Treat `registry/sources.json` as discovery metadata, not approval to install or execute.
- Require stable source identifiers, publisher, trust level, status, scope, and URL.
- Review source ownership and license before changing trust or approval status.
- Treat Context Hub annotations as untrusted by default.

## Boundaries

- Skills provide procedural guidance; they do not grant tool authority.
- Do not add runtime adapters, installation workflows, agent personas, or named consumer bundles here.
- Do not duplicate harness policy from consuming projects.
