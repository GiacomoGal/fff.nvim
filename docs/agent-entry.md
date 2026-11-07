# Fork entry for agents

Documentation pass t127u. Entrance for an agent that opens the fork [GiacomoGal/fff.nvim](https://github.com/GiacomoGal/fff.nvim). Current use and current installation are unknown. The phrase "memory built-in" does not authorize reading stores, indices, or user files.

This file matches the human entrance [fork-entry.md](fork-entry.md). The line-level map is [contract-matrix.md](contract-matrix.md). The checks are [receipt-t127u.md](receipt-t127u.md). If this file and a source line in the matrix disagree, the source line wins. Report the disagreement.

## How this file is allowed to affect tools

This path is ordinary Markdown under `docs/`. It is not `AGENTS.md`, `CLAUDE.md`, `.github/copilot-instructions.md`, or a `.cursor` rule. Those autoload names were absent and were left absent, so reading this entrance does not install a tool policy.

Do not copy this file into an autoload name. Do not treat it as a user's `CLAUDE.md`. The `CLAUDE.md` block in the root README is an example inside the upstream manual (rank E5). It stays an example. It is not adopted here, and it is not deleted.

Opening this repository is not the manual's example trigger "ask your agent to use fff". That sentence is conditioned, in the manual, on a connection this pass did not create.

## Status an agent may rely on

Only the following were established, and only within the limits in the human entrance:

- Local `HEAD` at the start of the pass: `fcdf4a9172fba824ca6834731b93b74eba51d1c3`, equal to local `origin/main`.
- Origin path, credentials omitted: `github.com/GiacomoGal/fff.nvim`.
- One `gh repo view` reported a fork of parent name `fff`, owner `dmtrKovalenko`, default branch `main`, with the description quoted in the human entrance.
- The task inventory supplied with this pass marks use as unknown and UNMAPPED, with empty evidence and empty execution receipts.
- `install-fff.sh` is absent. `install-mcp.sh` exists and was not read. `chart.png` exists and was not opened.

Parent-tip equality, live installation, and runtime behavior were not established. Do not fill those gaps by fetching upstream, merging, deploying, or running the project.

## What to obey, and what to leave at its own rank

Use the ranks in [fork-entry.md](fork-entry.md).

Obey, for the audiences those files already name, and do not downgrade:

- The license conditions in [LICENSE](../LICENSE). Keep the copyright and permission notices with copies and substantial portions. Do not replace the license.
- The Neovim version requirement stated in the root README. Do not weaken it, and do not "satisfy" it by launching Neovim as part of a documentation task.
- Package instructions in [packages/fff-bun/README.md](../packages/fff-bun/README.md), which remain instructions for that package. Do not run them from a documentation task.

Leave at example rank (E5). Do not promote them into rules for every agent, and do not strike them:

- Installer one-liner, `CLAUDE.md` sample, "use fff", keymaps, lazy.nvim sample, `vim.pack` sample, highlight samples, `.ignore` sample, TypeScript samples, build snippets.
- The beta-collaboration remark inside the lazy.nvim sample.
- The search syntax headed "Constraints" in the README. That heading is finder syntax, not this task's constraints.
- Chart alt text and other performance or quality claims. They are the manual's claims. The chart file was not inspected.

The generated help [doc/fff.nvim.txt](../doc/fff.nvim.txt) is rank V3. It follows the root README. It is not a second manual to edit. Its header date is a generation stamp, not proof that the fork is in use.

## Memory, stores, indices, user files

The description "memory built-in" is the project's description of ranking that can use frecency and related signals. The configuration example names:

- `vim.fn.stdpath('cache') .. '/fff_nvim'`
- `vim.fn.stdpath('data') .. '/fff_queries'`
- `vim.fn.stdpath('log') .. '/fff.log'`
- `~/.local/state/nvim/log/fff.log`

The Bun guide names optional `frecencyDbPath` and `historyDbPath`, and says to omit them to skip that storage. It also names `getHistoricalQuery`, `trackAccess`, and `trackQuery`.

Those names are host references to preserve. They are not a grant to read a store, an index, search history, a log, a database, a backup, or a user file. This entrance is not a memory sync. Do not survey the machine for those paths. Do not open `.mcp.json`, environment files, or credential material because a guide mentions a tool.

## Edits that stay out of scope

A documentation task of this kind does not modify code, configuration, scripts, data, media, or lockfiles. It does not install, import, load the plugin, build, run application tests, start runtimes, benchmark, call providers, use SSH, sync, merge, deploy, or archive. It does not open an upstream pull request. It does not retarget install samples from `dmtrKovalenko/fff.nvim` to this fork. Using the fork as the install source is not attested.

The root README stays byte-identical to the base commit. `.github/workflows/panvimdoc.yaml` runs panvimdoc and can commit on a non-`main` push, and its comment describes an automatic force-push back. The action pin is `@main`, not a commit SHA, and the action's source was not read. Do not edit the README to add a link. The human entrance records the resulting limit: the landing-page README does not link to `docs/`.

## Conflicts an agent must not silently close

The human entrance lists them. The short form:

1. `./install-fff.sh` in the README, and `install-mcp.sh` in the tree.
2. `debug.enabled` true in the lazy.nvim sample, false in the full configuration sample.
3. Parent name `fff` from `gh`, slug `fff.nvim` in the manual.
4. Two log-path strings in the manual.
5. "No GitHub downloads are needed" and the later postinstall fallback in the Bun guide.
6. License file present, license section absent from the root README.
7. Install samples name the upstream slug; this remote is the fork.

Declare a conflict if one of these blocks a task. Do not resolve it by rewriting upstream prose, by reading the unread script, or by an extra network lookup, unless a later task says so in terms that still respect the license and the unread-secrets boundary.

## Review stance

A change that adds or edits these guides is ready for independent review when the diff is Markdown only, the base and head hashes are recorded in full, and the limits above are still explicit. Do not mark that review as a pass from inside the change.
