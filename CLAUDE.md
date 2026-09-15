@AGENTS.md

The ClassVR Prototyping Kit is registered as a plugin from `./kit` by
`.claude/settings.json`, so use its skills directly: `/new-xr-app`,
`/share-xr-app`, `/preview-xr-app`, `/publish-xr-app`, `/check-headset`, and
`xr-app-rules` on every edit. If the skills are missing, `kit/` is probably an
empty folder — run `git submodule update --init --recursive`, then tell the
user to start a new session so the kit loads.
