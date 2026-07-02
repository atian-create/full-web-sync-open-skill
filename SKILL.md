---
name: full-web-sync-open-skill
description: Package a finished Skill, local project, or open-source repo into a public launch sync bundle. Use when the user says "full web sync", "全网同步", "open-source this", "make a GitHub release", "write X and Knowledge Planet copy", "Build in Public", or asks to turn a local Skill/project into repo-facing docs plus platform-ready launch text.
---

# Full Web Sync Open Skill

## Overview

Turn a completed project into a verified public launch package.

This skill is a release coordinator, not a generic reposting tool. It should preserve project facts, update or create repo-facing materials, verify GitHub state, and then produce copy-paste-ready launch text for X and Knowledge Planet.

## Default Workflow

1. Confirm the correct local workspace and read only necessary project files.
2. Inspect project facts: project name, purpose, source path, current repo, README, Skill files, examples, license, release state, and public/private boundaries.
3. If a GitHub repo exists, update it incrementally. Do not create a duplicate repo for the same project.
4. If no repo exists and the user wants open source, create a lightweight public repo with clear README, install/use instructions, license, topics, and release notes.
5. Route an internal archive if the user's environment supports Feishu or a local project doc. If blocked, fall back to local Markdown.
6. Produce copy-paste-ready X text and Knowledge Planet copy.
7. Report verified links and what was changed.

## Output Defaults

Always include:

- GitHub repo or release status
- local project or Skill path
- what public-facing files changed
- X platform text
- Knowledge Planet text
- any verification gaps

Do not include Xiaohongshu or WeChat public account copy unless the user explicitly asks for those platforms.

Do not produce an old-style "A Tian lightweight Skill breakdown" unless the user explicitly asks for it.

## Safety Boundaries

Never read or publish secrets, API keys, cookies, private customer material, unpublished commercial details, or internal error payloads.

Do not describe a project as an automated data-extraction system, traffic-growth machine, guaranteed monetization system, or viral-copy engine unless that is literally the project's verified purpose.

Prefer wording like:

- public launch package
- open-source Skill
- repo-facing docs
- release notes
- Build in Public
- workflow package
- creator operating workflow
- public content signals

## Verification

Before claiming success, verify the relevant state:

- repo visibility is public when open-sourcing
- pushed branch exists
- release or tag exists if one was created
- README and Skill instructions are present
- links open or can be fetched
- local git tree is clean or any remaining changes are explained

## References

- `references/sync-checklist.md`: detailed launch and verification checklist
- `references/copy-contracts.md`: X and Knowledge Planet output contracts
- `references/public-wording.md`: public wording boundaries and replacement phrases
