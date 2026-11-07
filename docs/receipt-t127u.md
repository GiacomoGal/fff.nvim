# Receipt t127u

Documentary receipt for the fork entrance in [GiacomoGal/fff.nvim](https://github.com/GiacomoGal/fff.nvim). This file does not grade the change. Independent review comes first. Nothing here is a pass.

The obligation map is [contract-matrix.md](contract-matrix.md). The human entrance is [fork-entry.md](fork-entry.md). The agent entrance is [agent-entry.md](agent-entry.md).

## Scope

- Repository remote, credentials omitted: `github.com/GiacomoGal/fff.nvim`.
- Intended pull request: unmerged, base `main`, head branch `cursor/fff-nvim-fork-entry-fec4`, on this fork.
- No upstream pull request, and no push to the parent repository.
- Intended diff: Markdown under `docs/` only.

## Identifiers known when these pages were written

| Item | Value |
| --- | --- |
| Base, `HEAD`, and local `origin/main` | `fcdf4a9172fba824ca6834731b93b74eba51d1c3` |
| `git merge-base HEAD origin/main` | `fcdf4a9172fba824ca6834731b93b74eba51d1c3` |
| Work tree | Clean, on `main`, before the branch was created |
| Commit subject | `feat(mcp): Make install script understand upgrade use case` |
| Author on that commit | Dmitriy Kovalenko |
| Committer time | `2026-03-13T16:45:21-07:00` |

This file does not embed the head hash of the commit that adds it. A commit cannot stably contain its own hash. After the branch is pushed, the pull request description records full `git rev-parse` output for base and head, plus `git diff --name-only` and `git diff --stat` from the base to the head. Those command outputs are the identifiers a reviewer should trust. If they disagree with this table, trust the command outputs and treat the disagreement as a defect.

Push is a normal push. This pass does not force-push and does not rebase.

## Checks performed

Effects are listed beside each check. None of them starts the plugin, installs a package, or reads a store.

| Check | What was done | Result used | Limit |
| --- | --- | --- | --- |
| Local git identity | `git rev-parse HEAD`, `git rev-parse origin/main`, `git merge-base`, `git status`, `git log -1` | Values in the table above | Local refs only. The parent repository was not fetched, so equality with the parent tip is unknown |
| GitHub record | One read-only `gh repo view --json nameWithOwner,isFork,parent,defaultBranchRef,url,description` | `isFork` true; name `GiacomoGal/fff.nvim`; default branch `main`; description `Fast File Finder for your AI and neovim, with memory built-in`; parent name `fff`; parent owner `dmtrKovalenko` | Metadata of the GitHub record. Not current use, not an install survey, not a content sync. No further GitHub lookup was made, including no lookup to resolve parent name `fff` against the slug `fff.nvim` |
| Filename presence | `test -f` on `install-fff.sh`, `install-mcp.sh`, `chart.png`, `AGENTS.md`, `CLAUDE.md`; directory presence of `docs/` and `.cursor` | `install-fff.sh` absent (exit 1); `install-mcp.sh` present; `chart.png` present; `AGENTS.md` and `CLAUDE.md` absent; `docs/` and `.cursor` absent at the start | Presence only. Bodies and pixels were not read |
| Manuals read | Root `README.md` (500 lines), `packages/fff-bun/README.md` (283 lines), `LICENSE` (21 lines) | Line citations in the matrix | Read as text. Not executed |
| Vim help sampled | `doc/fff.nvim.txt` lines 1–80 and 520–551 | Header date, generator credit on line 549, and a structural match in the spans that were read | Not a full equivalence proof between the help file and the README. `wc -l` reports 551 lines |
| Workflow files read | `.github/workflows/panvimdoc.yaml` (lines 1–36), `.github/workflows/spelling.yaml`, `_typos.toml` | The docs workflow triggers on any non-`main` push, has `contents: write`, uses `kdheepak/panvimdoc@main` (a branch, not a commit SHA), and auto-commits. Comment line 16 mentions an automatic force-push back. Spelling runs on pull requests. The typos word list was not changed | CI text, not product rules. Read so this pass would not edit the README into that job and would not edit the dictionary. The action source was not read. The workflows were not run locally |

## Checks not performed

Neovim was not started. The plugin was not loaded. Nothing was installed, imported, built, tested as an application, benchmarked, or run. No provider, package registry, installer URL, demo asset, or chart image was requested. No SSH, sync, merge, deploy, or archive. No global skill was changed. The body of `install-mcp.sh` was not read. `.mcp.json` was not read. Environment files, lockfiles, backups, databases, indices, search history, logs, frecency stores, and user files were not read and were not searched for on the machine. Source files were not mined for comments or for a hidden API list. Code comments, examples, and the history feature stay at the ranks in the matrix.

## Files this pass intends to add

- `docs/README.md`
- `docs/fork-entry.md`
- `docs/agent-entry.md`
- `docs/contract-matrix.md`
- `docs/receipt-t127u.md`

A reviewer can confirm the diff with `git diff --name-only fcdf4a9172fba824ca6834731b93b74eba51d1c3...HEAD`. Any path outside `docs/`, or any non-Markdown path, is outside this receipt.

## Residual limits

- Current use and current installation stay unknown. UNMAPPED stands.
- The root README does not link to `docs/`, because a README edit is wired to `.github/workflows/panvimdoc.yaml`.
- A normal push of this branch still matches that workflow's trigger. The action ref is `@main`, so the bytes it would write were not frozen here. If a run writes `doc/fff.nvim.txt`, that commit sits outside this receipt. The workflow file was not changed, so this residual effect is declared and not closed.
- Spelling CI may report words in these pages. `_typos.toml` was not edited to silence it. A local `typos` binary was not on `PATH`, and it was not installed. No local spelling run is recorded.
- The Vim help was not proven byte-equivalent to the README.
- Parent name `fff` and manual slug `fff.nvim` were not resolved against each other.
- The head hash lives in the pull request description, taken from git after the commit, not in this file.

## Review

The change is ready for a reviewer who checks the hashes, the name-only diff, the matrix sources, and the limits above. This receipt does not declare that review successful.
