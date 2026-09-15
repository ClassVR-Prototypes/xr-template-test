# XR prototype template

A ready-made home for **WebXR prototypes for ClassVR headsets**, built by
talking to an AI. Make a copy of this repository, open it in Claude Code, and
say "make a new VR app called Planet Walk". A minute later there is a link you
can open on a desktop or a headset.

The [ClassVR Prototyping Kit](https://github.com/ClassVR-Prototypes/classvr-prototyping-kit)
is bundled in `kit/`, so every copy of this template already knows how to
create, check, share and publish an app. Nothing to install.

## Start a new project (about two minutes, no terminal)

1. Press **Use this template → Create a new repository**. Give it a name —
   that name becomes part of the web address — and keep it **Public**
   (GitHub Pages needs that on a free plan).
2. In the new repository: **Settings → Pages → Build and deployment →
   Source: GitHub Actions**. One dropdown, once.
3. Open [claude.ai/code](https://claude.ai/code), pick the new repository, and
   type what you want: *"Make a new VR app called Planet Walk."*
4. When Claude finishes, press **Create PR**, then **Merge** on GitHub. A
   minute or two later the link Claude gave you is live:
   `https://<owner>.github.io/<repo>/planet-walk/`

Open the link on a desktop to look around (click, then move the mouse; W/A/S/D
to walk). Open it in the headset's browser — or scan a QR code of it — and
press **Enter VR**.

From then on it is conversation: "add a table", "make the sky darker", "put a
sign here". Every change ends with a refreshed link.

## What's in here

```
kit/                         the ClassVR Prototyping Kit (git submodule) — don't edit here
.claude/settings.json        registers the kit as a Claude Code plugin from ./kit
AGENTS.md                    instructions any AI assistant reads (Codex, Copilot, Cursor, Gemini CLI…)
CLAUDE.md                    the same, for Claude Code
.github/workflows/pages.yml  publishes every app on main to GitHub Pages
.github/scripts/build_pages.py   assembles the site: one folder per app → /<slug>/
.github/workflows/update-kit.yml brings the kit up to date (Mondays, or Actions → Run workflow)
<App Name>/                  each app: index.html, xr-project.json, local libraries
```

## Updating the kit

The kit is pinned to a version so an update can't surprise you mid-project.
To move to the latest: **Actions → "Update the prototyping kit" → Run
workflow** (or wait for Monday). In Claude Code, "update the kit" does the
same.

## Other AI tools

The kit's skills follow the open [Agent Skills](https://agentskills.io)
format and `AGENTS.md` tells any assistant where they are. Tools with a
sandbox (Codex, Copilot coding agent, Cursor) can run the kit's scripts;
chat-only tools can still apply the headset rules and edit the app.

## Made by

Avantis — Project Ptah. Prototypes here are public; keep anything private
elsewhere.
