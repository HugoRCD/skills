# Skills

[![license](https://img.shields.io/badge/license-Apache--2.0-blue.svg)](./LICENSE)

An open-source collection of opinionated skills for AI agents, focused on how I build and maintain my personal repositories. The catalog leans heavily on the Nuxt and Vue ecosystems, and reflects my personal workflows and conventions.

## Features

- Opinionated, reusable skills designed for real-world personal repos
- Nuxt and Vue-centric practices with broader ecosystem applicability
- Single-command install to add the full skill set

## Available skills

Keep this list up to date as new skills are added.

| Skill | Description |
| --- | --- |
| `create-pr-commit` | Suggest conventional commit or pull request titles in the format `type(scope): title`, written in lowercase English. |
| `setup-for-oss` | Review and bootstrap open-source repo health (OSS) by auditing or scaffolding README, CONTRIBUTING, LICENSE, CI workflows, and related files. |
| `unslop` | Remove low-signal AI-generated noise by deleting redundant comments, tightening formatting, and normalizing styling patterns. |

## Install the skills

This repository is distributed as a bundle. Installing it adds **all** skills at once:

```bash
npx skills add hugorcd/skills
```

## Getting Started

Once installed, you can reference any of the skills in this repository directly from your AI agent workflow.

Example usage in an agent that supports slash commands:

```
/unslop
```

## Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md).

## License

Apache-2.0. See [LICENSE](./LICENSE).
