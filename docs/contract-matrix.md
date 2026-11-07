# Contract matrix

Map from existing sources to the documents added in documentation pass t127u. Base commit for every line number in the repository: `fcdf4a9172fba824ca6834731b93b74eba51d1c3`. The root README, the Vim help, the Bun guide, and `LICENSE` were not edited, so these line numbers remain the lines in the tree.

Ranks are labels for readers of this matrix. They do not create a policy above the cited file.

| Rank | Scope |
| --- | --- |
| M0 | This documentation pass only |
| L1 | License conditions on dealing in the software |
| U2 | Upstream human manual, original audiences kept |
| V3 | Generated Vim help, derivative of the root README |
| P4 | Nested Bun package guide |
| E5 | Example, prompt, comment, or invitation; not universal policy, and not withdrawn |
| A0 | Recorded absence |
| W | Workflow file observed because it constrains this pass; not a product rule |

Destination shorthand: `H` is [fork-entry.md](fork-entry.md), `A` is [agent-entry.md](agent-entry.md), `R` is [receipt-t127u.md](receipt-t127u.md), `I` is [README.md](README.md). "In place" means the source file was left unchanged.

## M0 — mandate that binds this pass

External to the repository. Not copied in full. Section 4 of the attached batch note, the common constraints above that section, and the task statement.

| Field | Content |
| --- | --- |
| Rango | M0 |
| Destinatario | The author of this pass and a later reviewer of the unmerged fork pull request |
| Condizioni | Markdown only; unmerged pull request on the fork; no upstream pull request; current use unknown (UNMAPPED); identity of use not proven; evidence, proposal, later-decision, and execution-receipt lists empty |
| Trigger | Task t127u for `GiacomoGal/fff.nvim` |
| Host ref | None opened. The note's "memory built-in" wording is a description, and the task states that this wording does not authorize reading stores, indices, or user files |
| Destinazione | `H`, `A`, `R`, `I` |
| Motivo | The new pages exist to carry this mandate without rewriting upstream instructions |
| Trattamento | Applied to this pass. Not promoted into the root README, and not written into an autoload tool file |

Inventory fields restated, not re-investigated: reference `main`; fork true; archived false; language not detected; `identity_proven` false; `unknowncurrentuse` true; `nextdocscope` unresolved.

## Sources that remain in place

### C01 — title and two audiences

| Field | Content |
| --- | --- |
| Fonte | `README.md` 1–11 |
| Rango | U2 |
| Destinatario | Human readers. The line 5 links name two audiences: AI agents (MCP) and Neovim users |
| Condizioni | None in these lines |
| Trigger | None |
| Host ref | None |
| Destinazione | In place. `H` and `A` point at this manual instead of replacing the audiences |
| Motivo | The fork entrance must keep the manual's own split of readers |
| Trattamento | Preserved |

### C02 — upstream slug on the badges

| Field | Content |
| --- | --- |
| Fonte | `README.md` 14–18 |
| Rango | U2 |
| Destinatario | Readers of the landing page |
| Condizioni | None |
| Trigger | None |
| Host ref | `https://github.com/dmtrKovalenko/fff.nvim` (stargazers, issues, contributors) |
| Destinazione | In place. Slug repeated under conflict K3 |
| Motivo | Badge targets stay the upstream slug. They were not pointed at the fork |
| Trattamento | Preserved. URLs not requested |

### C03 — product sentence and ranking factors

| Field | Content |
| --- | --- |
| Fonte | `README.md` 23–25 |
| Rango | U2, descriptive |
| Destinatario | Human readers and, in the prose, AI agents as users of the finder |
| Condizioni | None |
| Trigger | None |
| Host ref | None. Factors named in prose: frecency, git status, file size, definition matches |
| Destinazione | In place. `H` and `A` state that this sentence is not a permission to open stores |
| Motivo | "Memory" here is a description of ranking. The task forbids treating it as a read grant |
| Trattamento | Preserved. Not downgraded to a disclaimer inside the manual, and not upgraded to a read permission |

### C04 — MCP purpose and chart

| Field | Content |
| --- | --- |
| Fonte | `README.md` 27–31 |
| Rango | U2, descriptive. The superiority claim is the manual's claim, tied to an image |
| Destinatario | Readers considering the MCP path |
| Condizioni | None |
| Trigger | None |
| Host ref | `./chart.png` |
| Destinazione | In place. `R` records that the file exists and was not opened |
| Motivo | The image is media. This pass does not edit media and does not inspect pixels, so the alt text stays an unverified upstream claim |
| Trattamento | Preserved |

### C05 — installer instruction

| Field | Content |
| --- | --- |
| Fonte | `README.md` 33–39 |
| Rango | U2 instruction for people installing upstream FFF. It is not an instruction this pass executed |
| Destinatario | The person who chooses to install the MCP dependency |
| Condizioni | The blockquote tells that person they can review the script before running it |
| Trigger | None automatic. The following section's "once you have it connected" depends on this install having been done by that person |
| Host ref | `https://dmtrkovalenko.dev/install-fff-mcp.sh`; relative `./install-fff.sh` |
| Destinazione | In place. `H`, `A`, and conflict K1. `R` records the filename check |
| Motivo | Named commands and URLs do not authorize execution. The relative path does not resolve; see K1 |
| Trattamento | Preserved. Not run. Not retargeted. The installer URL was not requested |

### C06 — example `CLAUDE.md`

| Field | Content |
| --- | --- |
| Fonte | `README.md` 41–47 |
| Rango | E5 |
| Destinatario | A person writing their own agent instructions after connecting FFF. The sample addresses "any file search or grep in the current git indexed directory" |
| Condizioni | The prose says the sample works perfectly after the connection in C05. That condition was not met in this pass, and the quality sentence stays the author's example, not a measured result |
| Trigger | Example trigger: ask the agent to "use fff". Opening this fork is not that trigger |
| Host ref | None |
| Destinazione | In place. `A` refuses to copy it into an autoload file |
| Motivo | An example prompt is not universal policy. Removing it would downgrade a published example |
| Trattamento | Left at E5 |

### C07 — Neovim demo invitation

| Field | Content |
| --- | --- |
| Fonte | `README.md` 49–53 |
| Rango | U2 framing, E5 invitation ("you better fill it yourself") |
| Destinatario | Neovim users |
| Condizioni | None that this pass can confirm. The size claims (linux repository, 100k files, 8GB) are the manual's claims |
| Trigger | None |
| Host ref | `https://github.com/user-attachments/assets/5d0e1ce9-642c-4c44-aa88-01b05bb86abb` |
| Destinazione | In place |
| Motivo | The invitation is not a result observed here. The asset was not requested |
| Trattamento | Preserved at its ranks |

### C08 — Neovim version requirement

| Field | Content |
| --- | --- |
| Fonte | `README.md` 57. The Vim help header repeats `Neovim >= 0.10.0` (`doc/fff.nvim.txt` line 1) |
| Rango | U2 prescription |
| Destinatario | Neovim users of FFF.nvim |
| Condizioni | The requirement applies to use of the plugin as stated by the manual |
| Trigger | Installation section |
| Host ref | None |
| Destinazione | In place. `H` and `A` repeat it as still in force and as not checked on this machine |
| Motivo | A prescription is not downgraded to a suggestion, and a documentation pass does not discharge it by launching Neovim |
| Trattamento | Preserved as a requirement |

### C09 — lazy.nvim sample

| Field | Content |
| --- | --- |
| Fonte | `README.md` 59–107 |
| Rango | E5 |
| Destinatario | A Neovim user configuring lazy.nvim |
| Condizioni | Sample comment: prebuilt binary download or an existing rustup toolchain. NixOS build line is commented. `lazy = false`, with the comment that the plugin initializes itself lazily |
| Trigger | Sample keys `ff`, `fg`, `fz`, `fc` |
| Host ref | Plugin spec `dmtrKovalenko/fff.nvim` (line 62). Build calls `require("fff.download").download_or_build_binary()` |
| Destinazione | In place. Conflict K2 (debug flag). Conflict K7 (slug not retargeted) |
| Motivo | The sample is an example, including the beta-collaboration comment at lines 73–74 (`debug.enabled` true, `show_scores` true). It was not promoted to a duty of this fork and not edited |
| Trattamento | Left at E5. Not executed |

### C10 — vim.pack sample

| Field | Content |
| --- | --- |
| Fonte | `README.md` 109–137 |
| Rango | E5 |
| Destinatario | A Neovim user configuring `vim.pack` |
| Condizioni | `PackChanged` callback runs the download when `event.data.updated` is true, inside the sample. `lazy_sync = true` is commented as starting sync when the picker is open |
| Trigger | Sample keymap `ff` |
| Host ref | `https://github.com/dmtrKovalenko/fff.nvim` (line 112) |
| Destinazione | In place. Conflict K7 |
| Motivo | Same as C09: example stays example; upstream URL stays upstream |
| Trattamento | Left at E5. Not executed |

### C11 — configuration reference

| Field | Content |
| --- | --- |
| Fonte | `README.md` 139–290 |
| Rango | U2 as the manual's statement that this is the complete option set; the Lua values are a sample of that set (E5 where they are one choice among comments) |
| Destinatario | Neovim users configuring `require('fff').setup` |
| Condizioni | Comments inside the sample state defaults and alternatives (layout, preview size limit 10MB, path shortening, grep modes). Those comments stay comments |
| Trigger | None |
| Host ref | See C12 and C13 |
| Destinazione | In place |
| Motivo | The block is the published option reference. This pass did not re-derive options from source, because "jump to the definition" (C15) was not followed |
| Trattamento | Preserved. Not re-verified against Lua or Rust |

### C12 — frecency and history paths

| Field | Content |
| --- | --- |
| Fonte | `README.md` 252–263 |
| Rango | U2 documented fields inside the sample. `enabled = true` is the value published in that sample |
| Destinatario | Neovim users |
| Condizioni | Frecency stores file-open frecency. History stores successfully opened queries. `min_combo_count` and `combo_boost_score_multiplier` are sample numbers |
| Trigger | None in this pass. The feature, as described, triggers on use of the picker |
| Host ref | `vim.fn.stdpath('cache') .. '/fff_nvim'`; `vim.fn.stdpath('data') .. '/fff_queries'` |
| Destinazione | In place. Named again in `H` and `A` as closed references |
| Motivo | The paths are host references to preserve. The task forbids opening stores, indices, search history, and user files. The sample's `enabled = true` is not a grant to read those directories |
| Trattamento | Preserved. Not opened. Not surveyed on disk |

### C13 — log path in the configuration sample

| Field | Content |
| --- | --- |
| Fonte | `README.md` 272–276 |
| Rango | U2 |
| Destinatario | Neovim users |
| Condizioni | Sample sets `logging.enabled` true and `log_level` to `info` |
| Trigger | None executed |
| Host ref | `vim.fn.stdpath('log') .. '/fff.log'` |
| Destinazione | In place. Conflict K4 with C20 |
| Motivo | A log path is a host reference. It was not opened |
| Trattamento | Preserved |

### C14 — debug flags in the full sample

| Field | Content |
| --- | --- |
| Fonte | `README.md` 268–271 |
| Rango | E5 value inside the U2 option reference |
| Destinatario | Neovim users |
| Condizioni | None beyond being the value in this sample |
| Trigger | None |
| Host ref | None |
| Destinazione | In place. Conflict K2 with C09 |
| Motivo | The two samples disagree. Closing the disagreement would rewrite upstream prose |
| Trattamento | Both values preserved. Not resolved |

### C15 — methods

| Field | Content |
| --- | --- |
| Fonte | `README.md` 292–304 |
| Rango | U2 names. The sentence "just jump to the definition and see what other APIs are exposed" is an invitation (E5) |
| Destinatario | Neovim users |
| Condizioni | None |
| Trigger | Calling the named functions, which this pass did not do |
| Host ref | None |
| Destinazione | In place. `H` lists the names as names |
| Motivo | The invitation was not followed, so this matrix does not add APIs from source comments or from Lua |
| Trattamento | Names preserved. Source not mined. Comments in code are not promoted |

### C16 — commands

| Field | Content |
| --- | --- |
| Fonte | `README.md` 306–315 |
| Rango | U2 |
| Destinatario | Neovim users |
| Condizioni | `:FFFClearCache` takes an optional argument `all`, `frecency`, or `files`, as written |
| Trigger | The commands themselves. Not run |
| Host ref | Clearing frecency is named. The frecency path in C12 was not opened |
| Destinazione | In place |
| Motivo | A named command is not authorization to execute, to use an account, or to read real data |
| Trattamento | Preserved as names |

### C17 — debug mode, multi-select, grep modes

| Field | Content |
| --- | --- |
| Fonte | `README.md` 317–375 |
| Rango | U2 description, with E5 configuration samples at 347–372 |
| Destinatario | Neovim users |
| Condizioni | Plain mode is described as the default. A single configured mode hides the indicator, as stated |
| Trigger | Sample keys `F2`, `<Tab>`, `<C-q>`, `<S-Tab>`, and `:FFFDebug` |
| Host ref | None |
| Destinazione | In place |
| Motivo | Feature prose stays feature prose. Samples stay samples |
| Trattamento | Preserved. Not exercised |

### C18 — finder search syntax headed "Constraints"

| Field | Content |
| --- | --- |
| Fonte | `README.md` 377–401 |
| Rango | U2 syntax for the finder |
| Destinatario | Users of file search and grep |
| Condizioni | Some tokens are grep-only, as the manual says (`*.md`, a single file path) |
| Trigger | Typing those tokens into the finder. Not performed |
| Host ref | `https://github.com/dmtrKovalenko/zlob` (line 385) |
| Destinazione | In place. `H` and `A` distinguish this heading from the mandate's constraints |
| Motivo | The word "constraints" in the manual is query syntax. Treating it as this task's rules, or deleting it, would change its rank |
| Trattamento | Preserved as finder syntax. URL not requested |

### C19 — cross-mode suggestions, git highlights, filtering

| Field | Content |
| --- | --- |
| Fonte | `README.md` 403–480 |
| Rango | U2, with E5 samples (highlight overrides, `.ignore` contents) |
| Destinatario | Neovim users |
| Condizioni | Git text color is described as opt-in (`git.status_text_color = true`). Sign column indicators are described as enabled by default. `.gitignore` is described as respected. `.ignore` is described as an extra filter that does not require editing `.gitignore` |
| Trigger | `:FFFScan` after filter changes, as written. Not run |
| Host ref | None beyond the project-root `.ignore` the manual tells a user they may create. No user `.ignore` and no repository ignore file was read for this matrix |
| Destinazione | In place |
| Motivo | Filtering prose is not permission to read ignore files, indexes, or user projects |
| Trattamento | Preserved. Ignore files not read |

### C20 — troubleshooting and the other log path

| Field | Content |
| --- | --- |
| Fonte | `README.md` 482–500 |
| Rango | U2 |
| Destinatario | Neovim users who hit a problem |
| Condizioni | `:FFFHealth` is described as checking picker initialization, optional dependencies (git, image preview tools), and database connectivity |
| Trigger | `:FFFHealth`, `:FFFOpenLog`. Not run |
| Host ref | `~/.local/state/nvim/log/fff.log` (line 500), called the default location |
| Destinazione | In place. Conflict K4. `H` states that database-connectivity prose is not a grant to open a database |
| Motivo | Same boundary as C12 |
| Trattamento | Preserved. Not run. Path not opened |

### C21 — generated Vim help

| Field | Content |
| --- | --- |
| Fonte | `doc/fff.nvim.txt`. Header line 1 (`Last change: 2026 March 13`, `Neovim >= 0.10.0`). Generator credit line 549 (`panvimdoc`, `https://github.com/kdheepak/panvimdoc`). Body sampled at 1–80 and 520–551; those spans track the README sections they correspond to, including the installer URL, the `CLAUDE.md` sample, and the log path |
| Rango | V3 |
| Destinatario | Neovim `:help` readers |
| Condizioni | Derivative of the root README. Not an independent contract |
| Trigger | The docs workflow in W01, which this pass did not run |
| Host ref | The same URLs and paths as the README, plus the generator URL |
| Destinazione | In place, byte-identical to the base |
| Motivo | Editing the help file would break the "Markdown only" limit. Regenerating it would be a tool run. A partial read is not a byte-for-byte equivalence proof against the README |
| Trattamento | Preserved. Not regenerated. Equivalence not fully proven |

### C22 — Bun guide, install and platforms

| Field | Content |
| --- | --- |
| Fonte | `packages/fff-bun/README.md` 1–34 |
| Rango | P4 |
| Destinatario | Users of the Bun package |
| Condizioni | Line 19 states that no GitHub downloads are needed. Line 34 states a fallback download from GitHub releases when the platform package is absent. See conflict K5 |
| Trigger | `bun add @ff-labs/bun`. Not run |
| Host ref | Package names `@ff-labs/bun` and the eight `@ff-labs/fff-bun-*` platform packages listed in the table |
| Destinazione | In place |
| Motivo | Nested package instructions stay scoped to that package. They were not executed and not copied into the root manual |
| Trattamento | Preserved |

### C23 — Bun init options and optional databases

| Field | Content |
| --- | --- |
| Fonte | `packages/fff-bun/README.md` 63–78, and the query-syntax lines 100–105 |
| Rango | P4 |
| Destinatario | Callers of `FileFinder.init` |
| Condizioni | `basePath` is marked required. `frecencyDbPath` and `historyDbPath` say to omit them to skip frecency and query tracking. `useUnsafeNoLock` is described as faster and less safe |
| Trigger | Calling `init`. Not called |
| Host ref | The two optional database path fields. Sample `basePath` strings in the guide are placeholders (`/path/to/project`, `/my/project`) |
| Destinazione | In place. `H` and `A` keep the "omit to skip" condition |
| Motivo | Optional storage is a published condition. It is not permission to read a path when one is set, and this pass did not set one |
| Trattamento | Preserved. Not called |

### C24 — Bun methods that record or read history

| Field | Content |
| --- | --- |
| Fonte | `packages/fff-bun/README.md` 107–165 and 179–189 |
| Rango | P4 names |
| Destinatario | Callers of the package |
| Condizioni | As written for each method (timeouts, page sizes, modes). Those numbers stay the guide's numbers |
| Trigger | `trackAccess`, `trackQuery`, `getHistoricalQuery`, `liveGrep`, `healthCheck`, and the other names in "Other Methods". Not called |
| Host ref | `getHistoricalQuery` would read past queries if called. It was not called |
| Destinazione | In place |
| Motivo | Method names are not a memory sync and not a grant to read search history |
| Trattamento | Preserved as names |

### C25 — Bun build, CLI, license line

| Field | Content |
| --- | --- |
| Fonte | `packages/fff-bun/README.md` 256–283 |
| Rango | P4 instructions (256–279). The license line 281–283 points at MIT and has rank L1 for the legal terms, which live in C26 |
| Destinatario | Someone building the C library or using the CLI; readers of the license line |
| Condizioni | "If prebuilt binaries aren't available" introduces the build steps |
| Trigger | The shell snippets `git clone`, `cargo build`, `bunx fff download`, `bunx fff info`. Not run |
| Host ref | `https://github.com/dmtrKovalenko/fff.nvim` (line 262). Output path `target/release/libfff_c.{so,dylib,dll}` |
| Destinazione | In place. Conflict K7 |
| Motivo | Build and download snippets are not authorization to build, download, or clone upstream |
| Trattamento | Preserved. Not run |

### C26 — MIT license

| Field | Content |
| --- | --- |
| Fonte | `LICENSE` 1–21. Copyright line 3: Copyright (c) 2025 Dmitriy Kovalenko. Condition lines 12–13: the copyright notice and the permission notice shall be included in all copies or substantial portions of the Software. Lines 16–21: provided as is, without warranty |
| Rango | L1 |
| Destinatario | Any person obtaining a copy of the software and associated documentation |
| Condizioni | The notice condition above. The warranty disclaimer is part of the same license |
| Trigger | Dealing in the software in the ways the permission grant lists |
| Host ref | None |
| Destinazione | In place. `H` and `A` cite it without replacing it. This matrix quotes the condition in one sentence and cites the lines |
| Motivo | License conditions are not downgraded. This pass does not relicense and does not paste the whole license into a second license |
| Trattamento | Preserved |

### C27 — recorded absences

| Field | Content |
| --- | --- |
| Fonte | Working tree at the base commit. `test -f` exit 1 for `AGENTS.md` and `CLAUDE.md`. No `docs/` directory and no `.cursor` directory at the start. No `CONTRIBUTING`, `SECURITY.md`, or pull-request template was found by a filename search |
| Rango | A0 |
| Destinatario | Agents and humans who might expect an autoload policy |
| Condizioni | Absence is the state at that commit. It is not a claim about other branches |
| Trigger | None |
| Host ref | Those filenames |
| Destinazione | `A` keeps the absences. This pass adds `docs/*.md` and does not add the autoload names |
| Motivo | Creating `AGENTS.md` or `CLAUDE.md` would install a tool policy. The task forbids that interference. An absence is not filled with a promoted prompt |
| Trattamento | Autoload names left absent |

### W01 — docs workflow

| Field | Content |
| --- | --- |
| Fonte | `.github/workflows/panvimdoc.yaml` 1–36. Trigger: push, branches-ignore `main` (lines 1–4). `permissions.contents: write` (lines 11–12). Comment line 16: `fetch last 2 commits required for auto force push back`, applied to `fetch-depth: 2` (line 17). panvimdoc step lines 18–24, `uses: kdheepak/panvimdoc@main` (line 19), `vimdoc: fff.nvim` (line 21). Auto-commit step lines 32–36 |
| Rango | W. Observed CI text. Not a product rule for Neovim users, and not rewritten |
| Destinatario | The author of this pass, because a push of a non-`main` branch starts it |
| Condizioni | The trigger is any push to a branch other than `main`. It does not say the README must have changed |
| Trigger | `git push` of this branch |
| Host ref | `kdheepak/panvimdoc@main` (a branch name, not a commit SHA). The action's own source was not read. This repository's help file credits panvimdoc (C21) |
| Destinazione | Decision recorded in `H`, `A`, and `R`: do not edit the root README or the Vim help |
| Motivo | The job has write permission and an auto-commit step, and its comment is about an automatic force-push back. The usual source file for that action was not re-checked against the action repository. A README edit is still the change most likely to make the job write `doc/fff.nvim.txt`. This pass does not force-push, does not edit the workflow, and does not edit those two files |
| Trattamento | Workflow left unchanged. Side effect on push is a residual limit in `R`, not a resolved conflict |

### W02 — spelling workflow

| Field | Content |
| --- | --- |
| Fonte | `.github/workflows/spelling.yaml` 6–10 (`pull_request` and push to `main`). `_typos.toml` read: excludes and extra words do not mention these new files |
| Rango | W |
| Destinatario | The author of this pass |
| Condizioni | The workflow checks the repository with typos. The dictionary file was not modified |
| Trigger | Opening the pull request |
| Host ref | Action `crate-ci/typos` pinned in that workflow |
| Destinazione | `R` |
| Motivo | New Markdown is visible to that check. Editing `_typos.toml` would be a configuration change, which this pass does not do |
| Trattamento | Dictionary left unchanged. A local typos result, if recorded in the receipt, is a documentary check with the limits stated there |

## Conflicts declared and not resolved

| Id | Sides | Why it stays open |
| --- | --- | --- |
| K1 | C05 cites `./install-fff.sh`. The tree contains `install-mcp.sh` and does not contain `install-fff.sh` | The script body was not read. Renaming the citation would change the manual. Renaming the script would change a script |
| K2 | C09 sample `debug.enabled = true` (README 73–74). C14 sample `debug.enabled = false` and `show_scores = false` (README 268–271) | Both are published samples. Unifying them rewrites upstream |
| K3 | `gh repo view` parent name `fff`, owner `dmtrKovalenko`. C02 and C10 use the slug `fff.nvim` | No second request was made to see whether the slug and the parent name are one repository |
| K4 | C13 `vim.fn.stdpath('log') .. '/fff.log'`. C20 `~/.local/state/nvim/log/fff.log` | Neither path was opened. The manual calls the second one the default location. They were not collapsed |
| K5 | Bun guide line 19, no GitHub downloads needed. Line 34, postinstall may download a GitHub release | Both sentences stay. This pass did not install the package |
| K6 | C26 `LICENSE` and Bun guide lines 281–283 name MIT. The root README has no license section | Notices that exist were not moved and not duplicated into a new license |
| K7 | Install and clone samples name `dmtrKovalenko/fff.nvim`. This remote is `GiacomoGal/fff.nvim` | The fork is not attested as an install source. Samples stay upstream |

## Claims introduced by this pass

Each new claim in `H` and `A` is one of the rows above, or one of the following observations. Nothing in the new pages is a runtime result.

| New claim | Source | Motivo |
| --- | --- | --- |
| This GitHub record is a fork of parent name `fff`, owner `dmtrKovalenko`, default branch `main`, with the description quoted in `H` | One `gh repo view` during this pass. Fields: `isFork`, `parent.name`, `parent.owner.login`, `defaultBranchRef.name`, `description` | Identity of the GitHub record only. Not current use. Not parent-tip equality |
| Local base is `fcdf4a9172fba824ca6834731b93b74eba51d1c3`, equal to local `origin/main`, clean tree, subject and author and committer time as in `H` | `git rev-parse`, `git merge-base`, `git status`, `git log -1` | Local clone state at authoring. No fetch of the parent |
| Use and installation are unknown; the inventory lists are empty; scope is unresolved | Task attachment, section 4 | The attachment is the source. This pass does not add usage evidence |
| `install-fff.sh` absent, `install-mcp.sh` present, `chart.png` present | `test -f` exit status | Filename presence only |
| Autoload agent files were absent | C27 | So the new guides would not become tool policy |
| Root README and Vim help were left unchanged because of W01 | W01 | Minimal fork adaptation that avoids a write workflow |
| Landing page does not link to `docs/` | Consequence of the previous row | Discoverability limit, declared |
| These pages are not a memory sync and do not authorize store, index, or user-file reads | Task statement, plus C03, C12, C20, C23, C24 | The description and the path names stay; the read does not happen |
| The pass is ready for independent review and is not a pass | Task statement | A document must not grade itself |

`I` only points at `H`, `A`, this file, and `R`. It adds no further factual claim.
