# Contributing to productskills

## Requesting a Skill

Open an issue describing the skill you'd like to see. Include what framework it would encode and when someone would use it.

## Adding a New Skill

### 1. Create the skill directory

```bash
mkdir -p skills/your-skill-name
```

Directory names are lowercase with hyphens. No underscores, no spaces.

### 2. Create SKILL.md

```yaml
---
name: your-skill-name
description: >
  One paragraph (~50 words). Must contain trigger phrases for when
  to use this skill. The description is always loaded in context;
  the body only loads when triggered.
---
```

The `name` field must match the directory name exactly. Only `name` and `description` in the frontmatter — no version, author, or other fields.

### 3. Write the body

Use `skills/prd-writing/SKILL.md` as a reference. General pattern:

```
[Opening: what this does and core philosophy, 1-2 sentences]

## [Core Framework]
[The methodology. This is 60%+ of the skill.]

## Guidelines
[ALWAYS/NEVER/CRITICAL rules]
```

### 4. Optional: add references

If the skill needs deeper templates or guides, add them in `references/`:

```
skills/your-skill-name/
  SKILL.md
  references/
    template.md
```

No other files — no README, CHANGELOG, or docs per skill folder.

## Quality Checklist

- [ ] `name` matches directory name
- [ ] Description includes trigger phrases
- [ ] Body is 50-150 lines
- [ ] Grounded in a real, citable framework
- [ ] Uses ALWAYS/NEVER/CRITICAL rules, not suggestions
- [ ] Assumes teams of 3-50, not enterprise
- [ ] Examples over explanations
- [ ] No "You are an expert..." role-setting
- [ ] No corporate PM language (SAFe, velocity, story points, RACI)
- [ ] No implementation details or code snippets

## Submitting

1. Fork the repo and create a branch
2. Add your skill
3. Open a PR

## Reporting Issues

If a skill gives bad output, open an issue with the skill name and what went wrong.
