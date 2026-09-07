# Boyue Distribution

This document is the repository-level source of truth for Agent Skill distribution. The GitHub repository remains canonical.

## Canonical identity

- Repository: `wuaishare/boyue`
- Skill path: `/SKILL.md`
- Canonical repository license: MIT
- Version source of truth: `SKILL.md` metadata + GitHub Releases
- Agent Skills metadata: `SKILL.md` uses the portable `license`, `compatibility`, and `metadata.author/version` fields

## Distribution matrix

| Surface | Repository policy | Current integration mode |
| --- | --- | --- |
| skills.sh | GitHub-native | Install with `npx skills add wuaishare/boyue`; repository is canonical |
| SkillsMP | GitHub-indexed | Eligible for automated discovery through Agent Skill metadata and GitHub topics |
| AgentSkill.sh | Registry import/sync | Imported from the canonical `SKILL.md`; security score 100/100. GitHub owner-level re-import/claim remains blocked by the registry's GitHub API rate limit |
| skills.re | GitHub import | Submitted and publicly indexed under Wuaishare; registry-generated categorization/evaluation may continue asynchronously |
| Skillstore | GitHub URL + audit PR | Submitted as `8f3ad21f-9dac-4034-9653-052ca42687fa`; automated audit marked it **safe**; review PR #3322 has been merged into Skillstore's review pipeline |
| Smithery Skills | Git-backed/API listing | **Published/listed:** Smithery skill `wuaishare/boyue`, backed by the canonical GitHub repository |
| ClawHub | Registry publish | **Published:** https://clawhub.ai/wuaishare/boyue — initial web import is MIT-0. A corrected `0.2.3` thin bundle is prepared; `.clawhubignore` limits future releases to the canonical Skill, references, and templates |
| AI智库 | First-party catalog | **Published:** https://ai.wuaishare.cn/hub/boyue/ — richer GitHub/i18n/security enrichment is tracked as a catalog pipeline improvement |

## Rules

1. GitHub is the canonical source; registries should not become divergent copies.
2. Keep `SKILL.md`, release version, license and marketplace metadata consistent.
3. Do not silently change the canonical repository license because a marketplace uses a different distribution license.
4. Marketplace listings must preserve links back to Wuaishare and the canonical repository where the platform supports them.
5. ClawHub publishes only the portable Skill/reference/template layer, not the long-form paper, covers, examples, or other repository material.
