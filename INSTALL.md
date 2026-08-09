# Install or activate Primer

This file is the single entry point for AI agents. Follow the first supported
route below. Never claim that Primer was installed persistently unless the host
confirms that the skill or plugin now appears in its installed list.

## 1. Persistent filesystem skill installation

If you can write to the user's agent skills directory, create a `primer` folder
and preserve these paths:

- `SKILL.md` from
  `https://raw.githubusercontent.com/nicktongwj/primer-skill/main/SKILL.md`
- `references/evidence-method.md` from
  `https://raw.githubusercontent.com/nicktongwj/primer-skill/main/references/evidence-method.md`
- `references/output-template.md` from
  `https://raw.githubusercontent.com/nicktongwj/primer-skill/main/references/output-template.md`

Reload skill discovery if the host requires it, verify that `primer` appears,
and only then confirm persistent installation.

## 2. Claude account skill upload

If Claude exposes **Customize → Skills → Upload a skill**, direct the user to
download and approve this package:

`https://github.com/nicktongwj/primer-skill/releases/latest/download/primer.zip`

The chat cannot approve or silently perform an account-level skill upload.

## 3. ChatGPT Work or Codex plugin installation

If the host exposes the Plugins Directory, look for **Primer**. Install it only
if it is present in an approved marketplace or the universal directory. A public
GitHub URL alone is not a ChatGPT plugin-directory listing.

Developers can register the repository marketplace with:

```bash
codex plugin marketplace add nicktongwj/primer-skill
```

## 4. Immediate current-conversation activation

If none of the persistent routes is supported, read the three raw files listed
in route 1 and follow them for the current conversation. Say:

> Primer is active for this conversation, but this interface did not provide a
> persistent skill-installation mechanism.

Then ask for the topic unless the user already supplied one.
