<h1>Hello!</h1>

I have Claude Code use LLM models Opus and Fable to build plugins for [Obsidian](https://obsidian.md) — mostly for capturing things fast
and for editing a lot of notes at once.

### Newest project

<a href="https://github.com/grub-basket/GridSense"><img width="440" alt="GridSense" src="https://img.shields.io/badge/GridSense-A%20real%20spreadsheet%20over%20your%20notes-4c6ef5?style=for-the-badge"></a>

Open a folder as an editable table, then work it like Excel — multi-cell selection,
fill down, TSV copy-paste to and from real spreadsheets, per-column filters, undo.

### Plugins I had Claude work on

#### In the community store

Install these from Obsidian itself — **Settings → Community plugins → Browse**.

**[Stashpad](https://github.com/grub-basket/SP)** — a capture-first, chat-style notes
workspace. Type at the bottom, press Enter, and your notes stack newest-first and nest
under each other, so an outline builds itself while you're just jotting. No filename to
invent, no folder to pick before you can write anything. *Based 
on the former Stashpad (Notes) desktop app.*

**[Bases Toolbox](https://github.com/grub-basket/Bases-Toolbox)** — quality-of-life tools
for Bases and properties. Find & replace a property value across the vault, bulk-edit
every file a base view is currently showing (set, backfill only-if-missing, append or
remove list items, delete outright), and import a CSV straight into notes. Every run is
logged in a history tab and can be reverted file by file.

**[GridSense](https://github.com/grub-basket/GridSense)** — an Excel-grade grid over your
frontmatter, for when you'd rather edit data than open notes one at a time. Rows are
notes, columns are properties, keys behave the way spreadsheet keys should, and every
write goes through Obsidian's own frontmatter API so note bodies are never touched.

**[Starter Packs](https://github.com/grub-basket/starter-packs)** — share a curated set of
plugins and themes as a link or a short paste-anywhere code, the way Bluesky starter packs
work. Annotate each pick with your own note; on the other end everything installs
*disabled* until the recipient reviews the pack.

**[Slide and Reveal](https://github.com/grub-basket/SnR)** — flashcard-style study of
labeled images: anatomy plates, diagrams, maps, sheet music. Drop covers on the labels and
scroll inside the image to uncover them a group at a time, instead of duplicating a slide
per label the way you'd have to in PowerPoint. There's also a quiz mode that pulls cropped
fragments from a whole folder and asks you to identify them out of context.

#### Beta — BRAT only, for now

Not in the store yet. Install with
[BRAT](https://github.com/TfTHacker/obsidian42-brat): *Add beta plugin*, then paste the
repo link.

**[Trynalist](https://github.com/grub-basket/Trynalist)** — a Dynalist-style outliner
where every line of the outline is a real Markdown note. Structure lives in frontmatter,
the file body is the line plus its note, and there are four views over the same data:
outline, flat, article, and a mind map. Nothing is locked inside the plugin. *Beta
software — via BRAT for now, expect rough edges.*

**[Draft Tabs](https://github.com/grub-basket/Draft-Tabs)** — keep several drafts of the
same note and flip between them with a tab strip above the editor. Rewrite a paragraph
three ways, branch an outline, or keep a safe copy before you gut something. Each draft
is an ordinary Markdown note. *Beta software — via BRAT for now, expect rough edges.*

### Community forks

Other people's plugins, patched. Some of it is offered back upstream, some of it ships
as a fork because upstream has gone quiet.

**[Scroll Buttons](https://github.com/grub-basket/obsidian-scroll-buttons)** — top / page
up / page down / bottom buttons and commands, originally built for e-ink devices where
normal scrolling leaves ghosting. Adopted from [triski](https://github.com/chenshutian9610),
with per-button toggles, smart hiding so they stay out of other plugins' way, and pop-out
window support added.

**[Creases](https://github.com/grub-basket/obsidian-creases)** — Liam Cain's fold-management
plugin, with a batch of longstanding bugs fixed: "always fold" silently breaking on
Obsidian 1.7+, template insertion unfolding everything, fold-and-clear corrupting lines,
empty headings jamming the fold-level commands, and a too-small tap target on mobile.
Installable as a drop-in replacement. *Via BRAT — same plugin ID, so disable the original
first.*

**[Edit History](https://github.com/grub-basket/obsidian-edit-history)** — Antonio Tejada's
per-note version history. Branches here fix a save race that could drop edits, harden the
reader against corrupt `.edtz` archives, stop a spurious Node stream notice on mobile,
correct apostrophe escaping, and fix the status bar going stale when you switch tabs.

**[Zotero Integration](https://github.com/grub-basket/obsidian-zotero-integration)** —
the citation, bibliography and PDF-annotation importer, now community-maintained. Branches
here cover a Better BibTeX JSON path for cite-as-you-write, a set of code-evident bugs, and
settings cleanup, with integration tests behind them.

**[BRAT](https://github.com/grub-basket/obsidian42-brat)** — TfTHacker's beta-plugin
installer, which nearly everything above is distributed through. Fixes go upstream as PRs
against its `beta` branch.

### Retired

**[Stashpad Classic](https://github.com/grub-basket/SP-Classic)** — a stable-Obsidian fork
from when mainline Stashpad accidentally shipped against insider-only APIs. Those APIs are
public now, so Classic is frozen; use Stashpad.

**[CSV to Obsidian Properties](https://github.com/grub-basket/CSV-to-Obsidian-Properties-for-Bases)** —
a browser tool that turned CSVs into notes with frontmatter. Archived; it became the CSV
importer in Bases Toolbox, though the
[hosted version](https://grub-basket.github.io/CSV-to-Obsidian-Properties-for-Bases/) still
works.

### Patches for non-Obsidian plugins

Bug fixes sent upstream to [jorio](https://github.com/jorio)'s projects — the retro-Mac
libraries and tools behind his ports of the old Pangea games. Each one is a branch on my
fork and an open pull request; nothing here is a competing release.

**[Pomme](https://github.com/grub-basket/Pomme)** — a cross-platform reimplementation of
the classic Macintosh Toolbox API.
[Fixed 32-bit PICT decoding](https://github.com/jorio/Pomme/pull/11): the 4-plane branch
walked rows with a 3-plane stride, so every row after the first read misaligned data and
the image skewed progressively.
[Guarded two sound-parser reads](https://github.com/jorio/Pomme/pull/12) against malformed
input — an AIFF chunk whose size underflowed into an oversized allocation, and an
unclamped Pascal-string length that returned uninitialized stack bytes.

**[OldMacArchiver](https://github.com/grub-basket/OldMacArchiver)** — an unpacker for
vintage Mac archive formats.
[Hardened AppleDouble sidecar parsing](https://github.com/jorio/OldMacArchiver/pull/2):
the untrusted `._name` file's entry table was used without bounds checks, so a crafted or
truncated sidecar could throw on a negative length or try to allocate 2 GB.
[Fixed byte sign-extension in FourCC](https://github.com/jorio/OldMacArchiver/pull/1) —
any byte ≥ 0x80 sign-extended and flooded the high bits, which classic type and creator
codes hit constantly.

**[PROBE](https://github.com/grub-basket/PROBE)** — a realtime graphical profiler for LÖVE.
[Made the sliding-window argument work](https://github.com/jorio/PROBE/pull/1): `init()`
took a window size but the reader looked it up as an out-of-scope global, so it was always
nil and the window stayed stuck at 60. Also scoped three variables that were leaking into
`_G` from a library module.

**[jorio](https://github.com/grub-basket/jorio)** — his profile README itself, which is
what this page is modelled on.
[Fixed the alt text and a stray tag](https://github.com/jorio/jorio/pull/1).

---

The forks install through [BRAT](https://github.com/TfTHacker/obsidian42-brat) too.
Issues and ideas welcome on any repo.
