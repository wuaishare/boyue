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
| AgentSkill.sh | Registry import/sync | Imported from the canonical `SKILL.md`; security score 100/100. GitHub owner-level re-import/claim remains blocked by the registry's server-side GitHub API rate limit (HTTP 429) |
| skills.re | GitHub import | **Publicly indexed:** https://skills.re/skills/wuaishare/boyue/boyue under Wuaishare, with registry-generated Strategy / Software-Development / AI-Development tags |
| Skillstore | GitHub URL + independent audit | Submission `8f3ad21f-9dac-4034-9653-052ca42687fa` was audited as **safe** with `safe_to_publish=true`; PR #3322 merged the result into `pending/wuaishare/boyue`. Final promotion from pending to the public `skills/` tree is controlled by Skillstore's review pipeline |
| Smithery Skills | Git-backed/API listing | **Published/listed:** https://smithery.ai/skills/wuaishare/boyue, backed by the canonical GitHub repository |
| ClawHub | Registry publish | **Published/latest:** https://clawhub.ai/wuaishare/boyue — `0.2.3`, MIT-0, 13-file curated bundle (`SKILL.md` + references + templates). ClawHub moderation/scanning is clean/benign. The accidental broad `0.1.0` version has been withdrawn |
| AI智库 | First-party catalog | **Published:** https://ai.wuaishare.cn/hub/boyue/ — richer GitHub/i18n/security enrichment is tracked as a catalog pipeline improvement |

## Rules

1. GitHub is the canonical source; registries should not become divergent copies.
2. Keep `SKILL.md`, release version, license and marketplace metadata consistent.
3. Do not silently change the canonical repository license because a marketplace uses a different distribution license.
4. Marketplace listings must preserve links back to Wuaishare and the canonical repository where the platform supports them.
5. ClawHub publishes only the portable Skill/reference/template layer, not the long-form paper, covers, examples, or other repository material.
