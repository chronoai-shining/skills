# qa-test-skillset

> QA E2E skillset for member-private exclusion + auto-revision test.

---

**Mirrored from [Ornn](https://ornn.ornn-cluster.local/skillsets/qa-test-skillset) — read-only.**

A curated multi-skill Claude Code plugin. Edits here are NOT propagated
back; manage this skillset on Ornn.

- Latest version: `1.0`
- Skills bundled: 2

## Master prompt

How an agent should orchestrate the members of this set:

Use qa-set-m1, then qa-set-m2, then qa-set-m3 in order to complete the QA flow.

## Skills in this plugin

- `qa-set-m1@1.0` — QA skillset member qa-set-m1 — used to test member-private exclusion.
- `qa-set-m2@1.0` — QA skillset member qa-set-m2 — used to test member-private exclusion.

Each member ships its own `SKILL.md` under `skills/<name>/`.

## Excluded members

These members are currently private or unresolvable on Ornn, so they are
NOT bundled in this public plugin:

- `qa-set-m3`

## Install

```bash
/plugin marketplace add chronoai-shining/skills
/plugin install qa-test-skillset@skills
```

> Third-party marketplaces default to auto-update OFF. Enable it in
> `/plugin` → Marketplaces if you want this skillset to update automatically.
