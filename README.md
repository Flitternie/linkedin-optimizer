# LinkedIn Profile Optimizer

English | [简体中文](README.zh-CN.md)

A reusable skill for reviewing and improving LinkedIn profiles from a resume, profile text, personal website, and publication list. It focuses on CS PhD students and AI researchers seeking research-oriented industry roles.

## Install

Copy `skills/linkedin-profile-optimizer/` into the appropriate skills directory:

| Host | Personal installation | Project installation |
|---|---|---|
| Codex | `~/.agents/skills/linkedin-profile-optimizer/` | `.agents/skills/linkedin-profile-optimizer/` |
| Claude Code | `~/.claude/skills/linkedin-profile-optimizer/` | `.claude/skills/linkedin-profile-optimizer/` |

The installable skill is at `skills/linkedin-profile-optimizer/`. Keep `SKILL.md` and `references/browser-setup.md` together. `agents/openai.yaml` supplies optional Codex UI metadata; Claude Code does not need it. If the skill does not appear, start a new session or restart the host.

Installation references: [Codex skills](https://developers.openai.com/codex/skills) and [Claude Code skills](https://code.claude.com/docs/en/skills).

### Install through your agent

Send your agent this instruction: “Read https://github.com/Flitternie/linkedin-profile-optimizer and its README, install the skill for your current host, and verify it is available.”

For the installing agent:

1. Download the repository and locate the directory whose `SKILL.md` names `linkedin-profile-optimizer`.
2. Copy that directory, including its references, into the appropriate personal skills directory above. Codex can also use `$skill-installer`.
3. For updates, preserve local modifications and replace only this skill's files.
4. Verify the files and references exist, then check host discovery; request a restart if needed. Installation is complete when the host recognizes the skill. Browser setup happens when running it.

Private repositories require access through the user's existing GitHub authentication.

## Use

In Codex:

```text
Use $linkedin-profile-optimizer to improve my LinkedIn profile for research scientist roles using my resume. Set up browser access if needed, apply the profile changes, and verify they saved.
```

In Claude Code:

```text
/linkedin-profile-optimizer Improve my LinkedIn profile for research scientist roles using my resume. Set up browser access if needed, apply the profile changes, and verify they saved.
```

You can start with a resume, personal homepage, Google Scholar link, portfolio, or pasted background. A resume is optional. When needed information is missing, the skill asks for source materials and focused follow-up details rather than inventing facts. Current LinkedIn content and target roles help tailor the result. The skill contains no candidate-specific profile data.

Optionally share target job descriptions or job links. The agent uses them to tailor positioning, keywords, project emphasis, and skill ordering to requirements supported by your experience. Without a JD, it proceeds using your target role family.

## Browser access

- **Default workflow:** the agent inspects LinkedIn in a browser, prepares and applies authorized changes, and verifies the saved result. Browser access is required; text feedback alone does not complete the task.
- **Connection problems:** the agent actively diagnoses and fixes the setup, including configuring a supported integration or setting up a needed browser client when permitted. You do not need to supply a preconfigured connection. Depending on your environment, the connection may use a browser MCP, Playwright, CDP, or a desktop browser integration.
- **Explicit review or draft-only requests:** the agent honors this narrower scope and does not apply edits.

The ChatGPT desktop app is optional. Installing the skill supplies instructions; the agent establishes browser access during the task using the tools and permissions available in your environment. You may need to grant permissions, restart the host, or complete authentication. See [browser setup](skills/linkedin-profile-optimizer/references/browser-setup.md).

When launching Chrome or Playwright, the agent uses a visible browser window so you can watch the edits and sign in directly. It keeps the same session through verification.

Enter credentials and complete authentication challenges in the browser yourself. The skill's profile-editing scope does not authorize messages, job applications, or public posts.

## Local work and license

Store source documents, edit snapshots, and progress in `.linkedin-profile-work/` in the user's working directory, separate from the installed skill. This directory and local browser state are covered by `.gitignore` when working in this repository.

Licensed under [MIT](LICENSE).
