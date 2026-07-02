# Full Web Sync Checklist

Use this checklist when packaging a local project, Skill, or repo for public launch.

## 1. Workspace Check

- Confirm the current workspace path.
- Read the minimum necessary files: `SKILL.md`, `README.md`, package files, examples, release notes, and existing docs.
- Search for private names, secrets, cookies, API keys, customer names, unpublished commercial details, and internal-only notes.
- If the user provided a template, apply it to the current project instead of only explaining the template.

## 2. Repo Check

- Check whether a public repo already exists.
- If it exists, update that repo instead of creating a duplicate.
- If it does not exist and the user asked for open source, create a clear public repo.
- Keep the repo focused: main instructions, examples, license, agent metadata, and references.

## 3. Repo-Facing Files

For a Skill repo, prefer:

- `SKILL.md`
- `agents/openai.yaml`
- `references/` for detailed workflow instructions
- `README.md` for human installation and use
- `LICENSE`
- examples only when they help a new user understand usage

Avoid dumping private working notes into the public repo.

## 4. GitHub Release

When creating or updating a release:

- Use semantic-ish tags such as `v0.1.0`, `v0.2.0`, or a date tag when that fits the project.
- Release notes should say what changed, who it is for, and how to use it.
- Add topics that describe the user's search intent, not just the internal brand.

Useful topics for creator Skill repos:

- `codex-skill`
- `creator-tools`
- `open-source`
- `build-in-public`
- `content-workflow`
- `knowledge-management`
- `ai-workflow`

## 5. Archive Route

If Feishu or another project-doc system is available, create or update a project record.

If external docs are blocked, write a local Markdown fallback and clearly report that it is the fallback.

Do not retry blocked authentication endlessly.

## 6. Final Verification

Before final response:

- Verify GitHub repo URL.
- Verify repo visibility.
- Verify release URL if created.
- Verify local git status.
- Verify no obvious private or banned wording remains.
- Summarize only the important outputs.
