<!-- changelog-schema: 2 -->
# Detailed Changelog

## Table of Contents & Work Log Index

- **Total Separate Work Sessions Logged:** 3
- **Total Git Commits Created Across All Entries:** 32

| Entry # | Date & Time | Work / Change Title | Agent & Model | Commits Count & Hashes | Jump Link |
| :---: | :---: | :--- | :--- | :--- | :---: |
| Entry #3 | 2026-11-26T15:47:34Z | Fix macOS Pre-Setup RunEvent::Opened Launch Race (#31) and Prepare Production Release v1.1.0 | Antigravity (agy) (Gemini 4 Neon (High)) | 2 Commits (`8945365`, `356281c`) | [Jump to Entry #3](#entry-3) |
| Entry #2 | 2026-11-26T15:30:10Z | Prevent .git/index.lock Collisions via --no-optional-locks and Serialized Mutating Git Commands | Antigravity (agy) (Gemini 4 Neon (High)) | 1 Commit (`7c791b3`) | [Jump to Entry #2](#entry-2) |
| Entry #1 | 2026-11-26T15:08:30Z | Audit and resolve 29 security, correctness, performance, accessibility, and upstream bugs (Issues #1-#29) | Antigravity (agy) (Gemini 4 Neon (High)) | 29 Commits (`9891888`, `96468d2`, `6def4da`, `026c8e5`, `706ae77`, `108375e`, `aceb369`, `0bb9d53`, `1b3eca6`, `e9c6b78`, `233f591`, `27b7dc9`, `73f92f4`, `2b6c60b`, `d7f851c`, `1941fe1`, `e0d520d`, `b894cdd`, `b1572a4`, `b4ace19`, `369797e`, `3555dcd`, `720f316`, `b0daa60`, `726f229`, `ba7c27f`, `925f930`, `4ad7144`, `6daaad9`) | [Jump to Entry #1](#entry-1) |

---


---

<a id="entry-1"></a>
## [Entry #1] 2026-11-26T15:08:30Z — Audit and resolve 29 security, correctness, performance, accessibility, and upstream bugs (Issues #1-#29)

- **Date & Exact Timestamp:** `2026-11-26T15:08:30Z`
- **Executed By Agent:** `Antigravity (agy)` | Model: `Gemini 4 Neon (High)`
- **Category:** `Fixed`
- **Status:** `committed`
- **Tier:** `full`
- **Commits Made in This Specific Work:** `29 Commits (`9891888`, `96468d2`, `6def4da`, `026c8e5`, `706ae77`, `108375e`, `aceb369`, `0bb9d53`, `1b3eca6`, `e9c6b78`, `233f591`, `27b7dc9`, `73f92f4`, `2b6c60b`, `d7f851c`, `1941fe1`, `e0d520d`, `b894cdd`, `b1572a4`, `b4ace19`, `369797e`, `3555dcd`, `720f316`, `b0daa60`, `726f229`, `ba7c27f`, `925f930`, `4ad7144`, `6daaad9`)`
  - Commit `9891888` (`2026-11-26T14:39:22Z`): `fix(security): validate file path and notes-folder containment in ai_execute_codex`
  - Commit `96468d2` (`2026-11-26T14:39:50Z`): `fix(security): block reserved directory names and path escapes in rename_folder`
  - Commit `6def4da` (`2026-11-26T14:40:34Z`): `fix(security): restrict write_file command to validated markdown export paths`
  - Commit `026c8e5` (`2026-11-26T14:41:39Z`): `fix(editor): flush pending WYSIWYG and source-mode saves reliably on unmount and note switch`
  - Commit `706ae77` (`2026-11-26T14:42:46Z`): `fix(storage): handle case-only note renames safely and keep notes_cache updated`
  - Commit `108375e` (`2026-11-26T14:43:19Z`): `fix(preview): avoid double-decoding file query parameter in preview mode`
  - Commit `aceb369` (`2026-11-26T14:43:41Z`): `fix(ai): read child stdout and stderr concurrently in execute_ai_cli`
  - Commit `0bb9d53` (`2026-11-26T14:44:04Z`): `fix(git): detect 'nothing to commit' in git commit stdout and avoid empty errors`
  - Commit `1b3eca6` (`2026-11-26T14:44:40Z`): `fix(folders): render FolderTreeView when vault has empty folders and zero notes`
  - Commit `e9c6b78` (`2026-11-26T14:46:19Z`): `fix(markdown): strictly parse YAML frontmatter in strip_frontmatter`
  - Commit `233f591` (`2026-11-26T14:47:28Z`): `fix(settings): prevent cross-folder setting bleed, serialize writes, and open external links safely`
  - Commit `27b7dc9` (`2026-11-26T14:47:56Z`): `fix(editor): use data-sidebar selector for Cmd+F guard and guard image insertion without notes folder`
  - Commit `73f92f4` (`2026-11-26T14:48:42Z`): `fix(folders): allow creating root-level folders when a nested note is open`
  - Commit `2b6c60b` (`2026-11-26T14:49:11Z`): `fix(clipboard): copy clean plain text instead of raw Markdown fences in WYSIWYG editor`
  - Commit `d7f851c` (`2026-11-26T14:50:48Z`): `fix(table): preserve line breaks inside table cells across Markdown round-trips`
  - Commit `1941fe1` (`2026-11-26T14:52:07Z`): `fix(windows): resolve concrete AI CLI executable path (.exe/.cmd/.bat) and Windows PATH`
  - Commit `e0d520d` (`2026-11-26T14:53:35Z`): `fix(cli): decode file:// URIs on Linux Open With and queue cold-start select-note`
  - Commit `b894cdd` (`2026-11-26T14:55:06Z`): `fix(images): store portable relative image paths and resolve local/Obsidian images at render time`
  - Commit `b1572a4` (`2026-11-26T14:55:58Z`): `fix(table): preserve task lists inside table cells across Markdown round-trips`
  - Commit `b4ace19` (`2026-11-26T14:56:29Z`): `fix(a11y): announce new lines to VoiceOver/screen readers on Return in editor`
  - Commit `369797e` (`2026-11-26T14:57:05Z`): `fix(a11y): mark hidden sidebar, focus mode chrome, and hidden format bar aria-hidden and inert`
  - Commit `3555dcd` (`2026-11-26T14:57:58Z`): `fix(table): preserve and render Markdown table column alignment (:---, :---:, ---:)`
  - Commit `720f316` (`2026-11-26T14:58:36Z`): `fix(tasks): preserve checked state when inserting a task above a checked task item`
  - Commit `b0daa60` (`2026-11-26T14:59:11Z`): `fix(wikilink): dismiss wikilink suggestion after ]] and stop swallowing Enter on empty results`
  - Commit `726f229` (`2026-11-26T15:00:59Z`): `fix(ai): disable Ollama word-wrap and strip CR/ANSI/thinking artifacts from output`
  - Commit `ba7c27f` (`2026-11-26T15:02:28Z`): `perf(startup): build Tantivy search index asynchronously and cache compiled regexes`
  - Commit `925f930` (`2026-11-26T15:03:25Z`): `fix(windows): use native Tauri WebView zoom and remove sidebar transform to fix tooltip/menu placement`
  - Commit `4ad7144` (`2026-11-26T15:04:54Z`): `perf(icloud): eliminate auto-save typing lag on iCloud Drive folders`
  - Commit `6daaad9` (`2026-11-26T15:07:09Z`): `fix(macos): avoid opening main window alongside preview on Finder cold-start double-click`
- **Files Touched Summary:** `19 files changed, +1967, -427`

### 1. In-Depth Executive Summary of Work

Performed a full codebase security, correctness, performance, and accessibility audit of the `Talhamehar007/scratch` fork alongside a complete triage of all 63 open upstream issues on `erictli/scratch`. Filtered strictly to genuine defects (excluding feature requests, suggestions, and non-code items), created 29 tracked GitHub issues on `Talhamehar007/scratch` (12 newly discovered codebase bugs/security vulnerabilities in Issues #1–#12 and 17 deduplicated upstream bug reports covering 20 upstream tickets in Issues #13–#29), and resolved every single issue individually with 1 dedicated atomic commit per issue before closing all 29 issues.

Key technical pillars delivered:
- **Security Hardening (#1–#3):** Enforced Markdown extension + canonical notes-folder containment in `ai_execute_codex`, blocked reserved directory names (`.git`, `.scratch`, `.obsidian`, `.trash`, `assets`, `.`, `..`) and folder escapes in `rename_folder`, and restricted `write_file` to validated `.md`/`.markdown` export paths.
- **Editor Reliability & Markdown Interoperability (#4, #6, #10, #12, #14, #15, #18, #19, #22, #23, #24):** Fixed Editor unmount/switch save loss in both WYSIWYG and Markdown source modes, fixed Preview window `%`-path double-decoding crash, hardened `strip_frontmatter` against horizontal rules (`---`/`----`), switched WYSIWYG clipboard `text/plain` to clean plain text while preserving rich HTML, added custom `ScratchTable`/`ScratchTableCell`/`ScratchTableHeader` extensions for `<br>` cell line breaks, task lists in table cells, and `:---`/`:---:`/`---:` column alignment, added `ScratchImage`/`ObsidianImageEmbed` for portable relative image paths and Obsidian `![[image.ext]]` embeds, added `ScratchTaskItem` to preserve checked state when inserting tasks above checked items, and fixed wikilink suggestion dismissal on `]]` and empty-result `Enter` handling.
- **Cross-Platform OS & AI CLI Fixes (#5, #7, #8, #16, #17, #25, #27, #29):** Fixed case-only note renames on APFS/NTFS and stale `notes_cache`, eliminated `execute_ai_cli` stdout/stderr pipe deadlocks, fixed `git::commit_all` empty-error handling on `nothing to commit`, unified Windows AI CLI resolution (`.exe` > `.cmd` > `.bat`) and PATH expansion, added Linux `file://` URI decoding + cold-start `pending_select_note` queuing + `--version`/`-V`, disabled Ollama word-wrapping (`--nowordwrap`) and stripped CR/ANSI/`<think>`/`Thinking...` blocks, switched interface zoom to native Tauri WebView zoom to fix Windows Radix tooltip/context-menu positioning, and fixed macOS Finder double-click opening both main and preview windows.
- **Performance, Folders, Settings & Accessibility (#9, #11, #13, #20, #21, #26, #28):** Moved Tantivy search index initialization/rebuilding off the main startup thread, cached hot-path regexes via `OnceLock`, eliminated iCloud Drive typing lag via self-write watcher suppression, background index commits, and in-place note list metadata updates, fixed empty-folder visibility and root-level folder creation when a nested note is open, fixed cross-folder settings bleed and concurrent settings write races, and added VoiceOver Return-key live announcements plus `aria-hidden`/`inert` on hidden sidebar and Focus Mode chrome.

### 2. Exhaustive Change-by-Change & File Breakdown

- **`src-tauri/src/lib.rs`** (`+764 / -164`):
  - **Functions / Classes / Symbols Modified:** `AppState`, `SearchIndex::new`, `strip_frontmatter`, `strip_markdown`, `mark_self_write`, `spawn_background_search_index_build`, `initialize_notes_folder`, `paths_refer_to_same_file`, `save_note`, `rename_folder`, `validate_export_markdown_path`, `write_file`, `setup_file_watcher`, `get_expanded_path`, `no_window_cmd`, `select_best_cli_candidate`, `resolve_cli`, `check_cli_exists`, `strip_ansi_and_cr`, `clean_ollama_output`, `execute_ai_cli`, `validate_note_path_in_folder`, `ai_execute_codex`, `ai_execute_ollama`, `try_select_in_notes_folder`, `take_pending_select_note`, `resolve_cli_arg_path`, `handle_cli_args`, `run`, `tests`.
  - **Detailed Breakdown of Changes:** Hardened `ai_execute_codex`, `rename_folder`, and `write_file`; added inode/canonical same-file detection and two-step case-only renames plus `notes_cache` upserts in `save_note`; drained child `stderr` concurrently with `stdout` in `execute_ai_cli`; tightened `strip_frontmatter` to require exact `---` lines and YAML key-value content; unified Windows/Unix CLI path resolution (`resolve_cli`) and native PATH joining; decoded `file://` URIs and queued cold-start `pending_select_note` + `--version`/`-V`; added `--nowordwrap` and CR/ANSI/thinking cleanup for Ollama; moved startup/folder-switch Tantivy rebuilds to a background task with 15MB writer buffer and `OnceLock` regexes; added self-write `debounce_map` marking and background Tantivy commits in `save_note`; deferred macOS cold-start main-window display and added `RunEvent::Opened` hiding + `RunEvent::Reopen` Dock restoration; added 4 unit tests.
  - **Reason & Technical Impact:** Closes security boundaries, eliminates cross-platform Windows/Linux/macOS desktop integration bugs, prevents AI CLI deadlocks/corruption, and eliminates cold-start and iCloud Drive typing stalls.
- **`src-tauri/src/git.rs`** (`+12 / -3`):
  - **Functions / Classes / Symbols Modified:** `commit_all`.
  - **Detailed Breakdown of Changes:** Checked both `stdout` and `stderr` for `"nothing to commit"` and fell back to trimmed `stdout` or a clear default error when `stderr` is empty.
  - **Reason & Technical Impact:** Prevents committing on a clean tree from failing with an empty error string (#8).
- **`src-tauri/capabilities/default.json`** (`+1 / -0`):
  - **Functions / Classes / Symbols Modified:** `permissions`.
  - **Detailed Breakdown of Changes:** Added `"core:webview:allow-set-webview-zoom"`.
  - **Reason & Technical Impact:** Enables native Tauri WebView zoom for #27.
- **`src/components/editor/TableExtensions.ts`** (`+350 / -0`, new file):
  - **Functions / Classes / Symbols Modified:** `ScratchTable`, `ScratchTableCell`, `ScratchTableHeader`, `parseTableCellTokens`, `serializeCellContent`, `formatAlignmentSeparator`.
  - **Detailed Breakdown of Changes:** Implemented full GFM table round-tripping for `<br>` cell line breaks (`hardBreak` + multi-paragraph), task lists inside cells (`- [ ]`/`- [x]` <-> `taskList`/`taskItem`), and `:---`/`:---:`/`---:` column alignments (`textAlign`).
  - **Reason & Technical Impact:** Fixes #15, #19, and #22 without losing formatting across saves and note switches.
- **`src/components/editor/ImageExtension.ts`** (`+233 / -0`, new file):
  - **Functions / Classes / Symbols Modified:** `ScratchImage`, `ObsidianImageEmbed`, `buildImageCandidatePaths`, `computePortableImagePath`, `resolveRelativeFsPath`, `getParentDir`.
  - **Detailed Breakdown of Changes:** Added a DOM NodeView that resolves relative local paths and Obsidian bare image filenames via Tauri `convertFileSrc` with `onerror` fallback candidates while keeping Markdown `src` portable, plus an `![[image.ext]]` Markdown tokenizer.
  - **Reason & Technical Impact:** Eliminates Scratch-specific `http://asset.localhost/...` URLs from `.md` files and restores cross-app compatibility with Obsidian (#18).
- **`src/components/editor/TaskItemExtension.ts`** (`+60 / -0`, new file):
  - **Functions / Classes / Symbols Modified:** `ScratchTaskItem`.
  - **Detailed Breakdown of Changes:** Overrode the `Enter` keyboard shortcut at offset 0 of non-empty checked task items to insert a new unchecked `taskItem` above instead of letting `splitListItem` uncheck the pushed-down task.
  - **Reason & Technical Impact:** Fixes #23.
- **`src/components/editor/Editor.tsx`** (`+186 / -62`):
  - **Functions / Classes / Symbols Modified:** `Editor`, `flushPendingSave`, `handleSourceChange`, `clipboardTextSerializer`, `handlePaste`, `handleAddImage`, `announceNewLine`.
  - **Detailed Breakdown of Changes:** Tracked latest `saveNote`, `sourceContent`, and `needsSourceSaveRef` via refs to flush pending WYSIWYG and source-mode saves reliably on unmount/switch (#4); fixed `[data-sidebar]` guard and guarded missing `notesFolder` in Preview mode (#12); switched `clipboardTextSerializer` to clean plain text and bypassed Markdown re-parsing for internal `data-pm-slice` pastes (#14); wired `ScratchTable`/`ScratchTableCell`/`ScratchTableHeader`, `ScratchImage`/`ObsidianImageEmbed`, and `ScratchTaskItem` (#15, #18, #19, #22, #23); added VoiceOver `sr-only` `aria-live="polite"` Return-key announcer (#20) and `aria-hidden`/`inert` on hidden Focus Mode chrome and format bar (#21).
  - **Reason & Technical Impact:** Fixes data loss, clipboard fidelity, portable images, tables, tasks, and VoiceOver accessibility.
- **`src/components/editor/WikilinkSuggestion.tsx`** (`+14 / -6`) & **`src/components/editor/SuggestionList.tsx`** (`+5 / -1`):
  - **Functions / Classes / Symbols Modified:** `WikilinkSuggestion.allow`, `SuggestionListInner.onKeyDown`.
  - **Detailed Breakdown of Changes:** Dismissed wikilink suggestions once text contains `]]` or `\n`, and returned `false` on `Enter`/`ArrowUp`/`ArrowDown` when `items.length === 0`.
  - **Reason & Technical Impact:** Fixes cursor trapping after typing a non-existent wikilink (#24).
- **`src/App.tsx`** (`+4 / -2`):
  - **Functions / Classes / Symbols Modified:** `App`, `AppContent`.
  - **Detailed Breakdown of Changes:** Removed double `decodeURIComponent` on `previewFile` (#6), added `aria-hidden`/`inert` to hidden `[data-sidebar]` (#21), and removed `translate-x-0` transform from `[data-sidebar]` (#27).
  - **Reason & Technical Impact:** Prevents Preview crashes on `%` paths, hides collapsed sidebar from screen readers, and fixes Windows popup anchoring.
- **`src/context/ThemeContext.tsx`** (`+190 / -151`):
  - **Functions / Classes / Symbols Modified:** `ThemeProvider`, `persistSettingsUpdate`, `loadSettingsFromBackend`.
  - **Detailed Breakdown of Changes:** Reset missing per-folder settings to defaults on folder switch, serialized all `getSettings`/`updateSettings` writes through a promise queue (#11), and replaced CSS `documentElement.style.zoom` with `getCurrentWebview().setZoom()` (#27).
  - **Reason & Technical Impact:** Stops cross-folder settings bleed, eliminates write races, and fixes Windows WebView2 zoom coordinate distortion.
- **`src/context/NotesContext.tsx`** (`+47 / -5`) & **`src/services/notes.ts`** (`+4 / -0`):
  - **Functions / Classes / Symbols Modified:** `NotesProvider`, `derivePreview`, `saveNote`, `takePendingSelectNote`.
  - **Detailed Breakdown of Changes:** Consumed cold-start `takePendingSelectNote()` during initialization (#17) and updated note list metadata in place on `saveNote` with a 2500ms self-save suppression window (#28).
  - **Reason & Technical Impact:** Fixes Linux/CLI cold-start note opening and eliminates iCloud Drive typing lag.
- **`src/components/notes/FolderNameDialog.tsx`** (`+35 / -5`) & **`src/components/layout/Sidebar.tsx`** (`+21 / -3`):
  - **Functions / Classes / Symbols Modified:** `FolderNameDialog`, `Sidebar`.
  - **Detailed Breakdown of Changes:** Added an optional location selector defaulting to Root folder so users can create root-level folders even when a nested note is open (#13).
  - **Reason & Technical Impact:** Resolves upstream #222.
- **`src/components/notes/NoteList.tsx`** (`+10 / -9`) & **`src/components/notes/FolderTreeView.tsx`** (`+7 / -0`):
  - **Functions / Classes / Symbols Modified:** `NoteList`, `FolderTreeView`.
  - **Detailed Breakdown of Changes:** Checked `foldersEnabled` before returning early on zero notes and rendered empty-vault placeholder inside `FolderTreeView` only when both notes and folders are empty (#9).
  - **Reason & Technical Impact:** Ensures newly created folders in an empty vault remain visible.
- **`src/components/settings/GeneralSettingsSection.tsx`** (`+13 / -11`) & **`src/components/settings/ToolsSettingsSection.tsx`** (`+11 / -5`):
  - **Functions / Classes / Symbols Modified:** `GeneralSettingsSection`, `ToolsSettingsSection`.
  - **Detailed Breakdown of Changes:** Replaced `<a target="_blank">` external links with buttons calling `open_url_safe` IPC (#11).
  - **Reason & Technical Impact:** Ensures external documentation and installer links open properly in the system browser under Tauri WebView.

### 3. Verification & System Impact

- **Tests & Commands Run:**
  - `npm run build` (`tsc && vite build`) — passed with 0 TypeScript or Vite errors.
  - `cargo test` in `src-tauri/` — passed (`4 passed; 0 failed`: `strip_frontmatter_handles_valid_yaml_and_ignores_horizontal_rules`, `select_best_cli_candidate_prefers_runnable_windows_wrappers`, `resolve_cli_arg_path_handles_file_uris_and_relative_paths`, `clean_ollama_output_strips_cr_ansi_thinking_and_outer_fences`).
  - `cargo clippy --all-targets -- -D warnings` in `src-tauri/` — passed with 0 warnings/errors.
  - Node.js native TypeScript round-trip verification suites via `@tiptap/markdown` `MarkdownManager` — verified table `<br>` line breaks (#15), task lists in table cells (#19), table column alignments (#22), and portable/Obsidian image paths (#18); all assertions passed.
  - `gh issue list -R Talhamehar007/scratch --state open` — returned `[]` (all 29 issues closed with commit references).
- **Breaking Changes / Side Effects:** None. Existing notes containing legacy `http://asset.localhost/...` image URLs continue to render normally alongside portable relative Markdown paths and Obsidian `![[image.ext]]` embeds.

---

<a id="entry-2"></a>
## [Entry #2] 2026-11-26T15:30:10Z — Prevent .git/index.lock Collisions via --no-optional-locks and Serialized Mutating Git Commands

- **Date & Exact Timestamp:** `2026-11-26T15:30:10Z`
- **Executed By Agent:** `Antigravity (agy)` | Model: `Gemini 4 Neon (High)`
- **Category:** `Fixed`
- **Status:** `committed`
- **Tier:** `full`
- **Commits Made in This Specific Work:** `1 Commits (`7c791b3`)`
  - Commit `7c791b3` (`2026-11-26T15:30:03Z`): `fix(git): disable optional locks for git status and serialize mutating git commands`
- **Files Touched Summary:** `2 files changed, 102 insertions(+), 11 deletions(-)`

### 1. In-Depth Executive Summary of Work

Resolved Issue `#30` (`Talhamehar007/scratch#30`), where committing changes inside Scratch on slow, virtual, or cloud-backed vaults (such as Cryptomator WebDAV mounts or iCloud Drive) could fail during staging with `fatal: Unable to create '.../.git/index.lock': File exists`.

Investigation identified two root causes in the Rust backend:
1. `git::get_status()` invoked `git status --porcelain` without `--no-optional-locks` / `GIT_OPTIONAL_LOCKS=0`, causing routine background status refreshes (triggered 1s after every `file-change` and on the 60s poll) to acquire `.git/index.lock` to refresh Git's stat cache. On slow WebDAV vaults, this directly collided with user-initiated `git add -A` and risked leaving stale 0-byte `.git/index.lock` files if interrupted.
2. Mutating Tauri git commands (`git_init_repo`, `git_commit`, `git_push`, `git_fetch`, `git_pull`, and remote management) ran concurrently on `spawn_blocking` with no synchronization, allowing periodic background `git fetch` calls to race with user commits/pulls/pushes.

Added `git_readonly_cmd()` (`GIT_OPTIONAL_LOCKS=0` + `--no-optional-locks`) for read-only git inspection, added an async `tokio::sync::Mutex<()>` (`git_op_lock`) to `AppState` to serialize mutating git commands without blocking UI status refreshes, appended a concise recovery hint when staging or committing hits an existing `.git/index.lock`, and added Rust unit tests covering both behaviors.

### 2. Exhaustive Change-by-Change & File Breakdown

- **`src-tauri/src/git.rs`** (`+90 / -11`):
  - **Functions / Classes / Symbols Modified:** `git_readonly_cmd`, `get_status`, `get_remote_url`, `commit_all`, `format_lock_hint_if_needed`, `tests::get_status_succeeds_without_touching_index_lock`, `tests::commit_all_appends_stale_lock_hint_when_index_lock_exists`.
  - **Detailed Breakdown of Changes:** Added `git_readonly_cmd()` setting `GIT_OPTIONAL_LOCKS=0` and `--no-optional-locks` and switched `get_status()` (`branch --show-current`, `remote`, `status --porcelain`, `rev-list`) and `get_remote_url()` to use it; added `format_lock_hint_if_needed()` and wired it into `commit_all()` staging and commit error paths so existing `.git/index.lock` errors include actionable stale-lock guidance; added two unit tests verifying status works when `.git/index.lock` exists and `commit_all()` formats the stale-lock hint cleanly.
  - **Reason & Technical Impact:** Prevents background status refreshes from creating `.git/index.lock` or blocking/failing when an index lock exists, and gives users clear recovery instructions when a pre-existing stale lock blocks commits.
- **`src-tauri/src/lib.rs`** (`+12 / -0`):
  - **Functions / Classes / Symbols Modified:** `AppState`, `AppState::default`, `git_init_repo`, `git_commit`, `git_push`, `git_fetch`, `git_pull`, `git_add_remote`, `git_set_remote_url`, `git_remove_remote`, `git_push_with_upstream`, `run`.
  - **Detailed Breakdown of Changes:** Added `pub git_op_lock: Arc<tokio::sync::Mutex<()>>` to `AppState` (initialized in both `Default::default()` and `run()`), and acquired `state.git_op_lock.clone().lock_owned().await` across all 9 mutating git Tauri commands while keeping read-only `git_get_status` non-blocking.
  - **Reason & Technical Impact:** Serializes concurrent mutating git operations (e.g., 60s background `git_fetch` vs user `git_commit`/`git_pull`/`git_push`) without stalling Tokio blocking threads or UI status refreshes.

### 3. Verification & System Impact

- **Tests & Commands Run:**
  - `cargo test` in `src-tauri/` — passed (`6 passed; 0 failed`, including the 2 new tests `git::tests::get_status_succeeds_without_touching_index_lock` and `git::tests::commit_all_appends_stale_lock_hint_when_index_lock_exists`).
  - `cargo clippy --all-targets -- -D warnings` in `src-tauri/` — passed with 0 warnings/errors.
- **Breaking Changes / Side Effects:** None. Read-only `git status` no longer rewrites `.git/index` stat caches opportunistically, which is the standard practice used by VS Code, Lazygit, and other GUI Git clients to avoid lock contention.

---

<a id="entry-3"></a>
## [Entry #3] 2026-11-26T15:47:34Z — Fix macOS Pre-Setup RunEvent::Opened Launch Race (#31) and Prepare Production Release v1.1.0

- **Date & Exact Timestamp:** `2026-11-26T15:47:34Z`
- **Executed By Agent:** `Antigravity (agy)` | Model: `Gemini 4 Neon (High)`
- **Category:** `Changed`
- **Status:** `committed`
- **Tier:** `full`
- **Commits Made in This Specific Work:** `2 Commits (`8945365`, `356281c`)`
  - Commit `8945365` (`2026-11-26T15:45:48Z`): `fix(macos): queue pre-setup RunEvent::Opened paths and coordinate Ready/Opened launch state`
  - Commit `356281c` (`2026-11-26T15:47:34Z`): `chore(release): bump version to 1.1.0 and point updater endpoint to fork`
- **Files Touched Summary:** `6 files changed, 203 insertions(+), 65 deletions(-)`

### 1. In-Depth Executive Summary of Work

Resolved Issue `#31` (`Talhamehar007/scratch#31`, follow-up to `#29` / upstream `erictli/scratch#92`) and prepared production release `v1.1.0` across all manifests and lockfiles.

Live event tracing on macOS revealed why opening an external Markdown file on cold start via Finder or `open -a Scratch file.md` still opened both the preview window and the main window: Tauri v2 / AppKit delivers `RunEvent::Opened` **before** `.setup()` executes and registers `AppState`. As a result, `try_state::<AppState>()` returned `None` inside `RunEvent::Opened`, causing `has_notes_folder` to evaluate to `false` and `try_select_in_notes_folder()` to fail on cold start. Flag-only LaunchServices CLI arguments (such as `-psn_...`) and `.setup()` I/O delays on slow WebDAV/iCloud mounts also risked showing `main` prematurely.

Introduced a `MacLaunchState` mutex coordinating `.setup()`, `RunEvent::Ready`, `RunEvent::Opened`, and `RunEvent::Reopen`: pre-setup `RunEvent::Opened` file paths are queued into `pending_opened_paths` and drained inside `.setup()` immediately after `AppState` is registered, flag-only CLI arguments are ignored, and deferred main-window display is scheduled only after `RunEvent::Ready` when no launch files were opened. Empirically verified on macOS via CoreGraphics `CGWindowListCopyWindowInfo` on-screen window checks across all three launch scenarios, then bumped Scratch to `v1.1.0` across all Node/Cargo/Tauri manifests and pointed the Tauri updater endpoint to `Talhamehar007/scratch`.

### 2. Exhaustive Change-by-Change & File Breakdown

- **`src-tauri/src/lib.rs`** (`+196 / -58`):
  - **Functions / Classes / Symbols Modified:** `run`, `MacLaunchState` (new local macOS state struct inside `run`).
  - **Detailed Breakdown of Changes:** Replaced the `150ms` `.setup()` sleep and `startup_instant` atomic boolean with `Arc<Mutex<MacLaunchState>>` (`pending_opened_paths`, `deferred_main_show`, `opened_in_launch`, `opened_preview_only`, `main_shown_for_user`, `ready_instant`). Ignored flag-only CLI arguments via `has_positional_cli_arg`; queued pre-setup `RunEvent::Opened` Markdown paths when `AppState` is not yet registered and drained them in `.setup()` after `app.manage(state)`; moved the deferred main-window show to `RunEvent::Ready` (dispatched via `run_on_main_thread`); guarded `RunEvent::Reopen` against cold-start races.
  - **Reason & Technical Impact:** Eliminates the duplicate main window on macOS cold-start Markdown launches and ensures cold-start Finder launches of notes inside `notes_folder` properly select in the main window.
- **`package.json`** (`+1 / -1`), **`package-lock.json`** (`+2 / -2`), **`src-tauri/Cargo.toml`** (`+1 / -1`), **`src-tauri/Cargo.lock`** (`+1 / -1`):
  - **Functions / Classes / Symbols Modified:** Package version metadata.
  - **Detailed Breakdown of Changes:** Bumped version from `1.0.0` to `1.1.0` consistently across frontend and Rust manifests and lockfiles.
  - **Reason & Technical Impact:** Prepares synchronized semantic version `v1.1.0` for tagging, CLI `--version` output, and release artifact naming.
- **`src-tauri/tauri.conf.json`** (`+2 / -2`):
  - **Functions / Classes / Symbols Modified:** `version`, `plugins.updater.endpoints`.
  - **Detailed Breakdown of Changes:** Bumped bundle version to `1.1.0` and updated updater endpoint to `https://github.com/Talhamehar007/scratch/releases/latest/download/latest.json`.
  - **Reason & Technical Impact:** Ensures macOS/desktop bundles report `1.1.0` and prevents fork installations from auto-updating back to upstream releases.

### 3. Verification & System Impact

- **Tests & Commands Run:**
  - Live macOS CoreGraphics (`CGWindowListCopyWindowInfo` `.optionOnScreenOnly`) verification on built `Scratch.app`:
    - Cold-start `open -a Scratch.app /tmp/scratch-repro-1.md` — `COUNT=1 NAMES=["scratch-repro-1.md — Scratch"]` (passed).
    - Second external file while preview-only — `COUNT=2 NAMES=["scratch-repro-2.md — Scratch", "scratch-repro-1.md — Scratch"]` (passed).
    - Cold-start normal launch `open -a Scratch.app` — `COUNT=1 NAMES=["Scratch"]` (passed).
  - `npm run build` (`tsc && vite build`) — passed with 0 errors.
  - `cargo test` in `src-tauri/` — passed (`6 passed; 0 failed`).
  - `cargo clippy --all-targets -- -D warnings` in `src-tauri/` — passed with 0 warnings/errors.
- **Breaking Changes / Side Effects:** None. Fork updater endpoint now targets `Talhamehar007/scratch` instead of upstream `erictli/scratch`.

---
