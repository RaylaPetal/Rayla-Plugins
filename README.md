# Rayla-Plugins

A single Dalamud custom-repository `repo.json` listing every plugin Rayla
Petal maintains, so users add one repository URL instead of one per plugin.

## Plugins

| Plugin | Repo |
|---|---|
| WatchAlong | https://github.com/RaylaPetal/kosmi-watch-14 |
| ReactToMe | https://github.com/RaylaPetal/ReactToMe |
| PoseKit | https://github.com/RaylaPetal/PoseKit |
| Oathbound | https://github.com/RaylaPetal/xiv-collar |

StreamMask is not yet listed here — it has no tagged release or CI-published
zip yet, so there's nothing for a download link to point at.

## Adding this repository in-game

`/xlsettings` → `Experimental` → Custom Plugin Repositories → add the raw URL
to `repo.json` in this repo (once it's pushed and hosted somewhere reachable,
e.g. `https://raw.githubusercontent.com/<owner>/Rayla-Plugins/master/repo.json`).

## Keeping it in sync

`repo.json` here is a merge of each plugin's own `repo.json` (each plugin
repo's release CI keeps its own copy up to date on every tagged release).
When a plugin ships a new version, re-run the merge (or copy that one
entry over) and commit here — this repo does not itself run a build for
any plugin.
