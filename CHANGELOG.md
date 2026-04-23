# Changelog

All notable changes to this marketplace are documented here. The format is based on [Keep a Changelog](https://keepachangelog.com/), and the marketplace and each plugin adhere to [Semantic Versioning](https://semver.org/).

## [Unreleased]

## [0.1.1] - 2026-04-23

### Changed
- **confluence-cli** plugin: reworded README and SKILL.md to reflect plugin terminology (was drafted as a user skill). Install instructions now lead with `/plugin marketplace add` + `/plugin install` and clarify that slash commands live in the Claude Code chat (not the terminal).
- Replaced hardcoded `~/.claude/skills/confluence-cli/...` paths with dynamic discovery via `find ~/.claude -name <script> -path '*confluence-cli*'`, so the skill works regardless of install location (plugin cache vs local skills folder).

## [0.1.0] - 2026-04-23

### Added
- Initial marketplace scaffold (`.claude-plugin/marketplace.json`, layout, docs).
- `confluence-cli` plugin **v0.1.0** (experimental):
  - 11 commands covering read/write/search/attachments against Confluence Cloud v2 REST API.
  - Interactive credential setup script with token validation.
  - Cross-platform (Python 3 stdlib only).
  - Three storage-format templates (spec-api, flow-doc, adr).
  - Storage format cheatsheet for writing pages.
