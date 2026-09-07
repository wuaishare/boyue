# Boyue Distribution

This document is the repository-level source of truth for Agent Skill distribution. The GitHub repository remains canonical.

## Canonical identity

- Repository: `wuaishare/boyue`
- Skill path: `/SKILL.md`
- License: MIT
- Version source of truth: `SKILL.md` + GitHub Releases

## Distribution matrix

| Surface | Repository policy | Current integration mode |
| --- | --- | --- |
| skills.sh | GitHub-native | Install with `npx skills add wuaishare/boyue`; repository is canonical |
| SkillsMP | GitHub-indexed | Eligible for automated discovery through Agent Skill metadata and GitHub topics |
| AgentSkill.sh | GitHub import/sync | Ready for owner-verified GitHub import; registry account connection is external to this repository |
| Smithery Skills | Git-backed/API listing | Ready for listing; Smithery namespace/API authorization is required to publish |
| ClawHub | Registry publish | **Not published**: ClawHub applies MIT-0 to published skills; Boyue is MIT and must not be silently relicensed |
| AI智库 | First-party catalog | Canonical first-party listing should point back to this repository and preserve authorship/version/license metadata |

## Rules

1. GitHub is the canonical source; registries should not become divergent copies.
2. Keep `SKILL.md`, release version, license and marketplace metadata consistent.
3. Do not relicense or duplicate the methodology text for a marketplace without an explicit project decision.
4. Marketplace listings must preserve attribution to Wuaishare and the canonical repository.
