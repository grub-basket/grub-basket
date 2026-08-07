<div align="center">

<h1>Hey!</h1>

I build plugins for [Obsidian](https://obsidian.md) — mostly for capturing things fast
and for editing a lot of notes at once.

<br/>

### Newest project

<a href="https://github.com/grub-basket/GridSense"><img width="440" alt="GridSense" src="https://img.shields.io/badge/GridSense-A%20real%20spreadsheet%20over%20your%20notes-4c6ef5?style=for-the-badge"></a>

Open a folder as an editable table, then work it like Excel — multi-cell selection,
fill down, TSV copy-paste to and from real spreadsheets, per-column filters, undo.

<br/>

### Plugins

<a href="https://github.com/grub-basket/SP"><img width="180" alt="Stashpad" src="https://img.shields.io/badge/Stashpad-Capture--first%20notes-5c7cfa?style=for-the-badge"></a>
<a href="https://github.com/grub-basket/Bases-Toolbox"><img width="180" alt="Bases Toolbox" src="https://img.shields.io/badge/Bases%20Toolbox-Bulk%20property%20editing-5c7cfa?style=for-the-badge"></a>
<a href="https://github.com/grub-basket/GridSense"><img width="180" alt="GridSense" src="https://img.shields.io/badge/GridSense-Frontmatter%20as%20a%20grid-5c7cfa?style=for-the-badge"></a>
<br/>
<a href="https://github.com/grub-basket/Trynalist"><img width="180" alt="Trynalist" src="https://img.shields.io/badge/Trynalist-Outliner%2C%20one%20note%20per%20line-5c7cfa?style=for-the-badge"></a>
<a href="https://github.com/grub-basket/Draft-Tabs"><img width="180" alt="Draft Tabs" src="https://img.shields.io/badge/Draft%20Tabs-Versions%20of%20one%20note-5c7cfa?style=for-the-badge"></a>
<a href="https://github.com/grub-basket/starter-packs"><img width="180" alt="Starter Packs" src="https://img.shields.io/badge/Starter%20Packs-Share%20a%20whole%20setup-5c7cfa?style=for-the-badge"></a>
<br/>
<a href="https://github.com/grub-basket/SnR"><img width="180" alt="Slide and Reveal" src="https://img.shields.io/badge/Slide%20and%20Reveal-Study%20labeled%20diagrams-5c7cfa?style=for-the-badge"></a>

<br/>

### Community forks

Other people's plugins, patched. Some of it is offered back upstream, some of it ships
as a fork because upstream has gone quiet.

<a href="https://github.com/grub-basket/obsidian-creases"><img width="180" alt="Creases" src="https://img.shields.io/badge/Creases-Folding%2C%20unbroken-868e96?style=for-the-badge"></a>
<a href="https://github.com/grub-basket/obsidian-edit-history"><img width="180" alt="Edit History" src="https://img.shields.io/badge/Edit%20History-Crash%20%26%20race%20fixes-868e96?style=for-the-badge"></a>
<a href="https://github.com/grub-basket/obsidian-zotero-integration"><img width="180" alt="Zotero Integration" src="https://img.shields.io/badge/Zotero%20Integration-Citation%20picker%20fixes-868e96?style=for-the-badge"></a>
<br/>
<a href="https://github.com/grub-basket/obsidian-scroll-buttons"><img width="180" alt="Scroll Buttons" src="https://img.shields.io/badge/Scroll%20Buttons-Paging%20for%20e--ink-868e96?style=for-the-badge"></a>
<a href="https://github.com/grub-basket/obsidian42-brat"><img width="180" alt="BRAT" src="https://img.shields.io/badge/BRAT-Upstream%20PRs-868e96?style=for-the-badge"></a>

</div>

### What each one is

**[Stashpad](https://github.com/grub-basket/SP)** — a capture-first, chat-style notes
workspace. Type at the bottom, press Enter, and your notes stack newest-first and nest
under each other, so an outline builds itself while you're just jotting. No filename to
invent, no folder to pick before you can write anything. *In the community store.*

**[Bases Toolbox](https://github.com/grub-basket/Bases-Toolbox)** — quality-of-life tools
for Bases and properties. Find & replace a property value across the vault, bulk-edit
every file a base view is currently showing (set, backfill only-if-missing, append or
remove list items, delete outright), and import a CSV straight into notes. Every run is
logged in a history tab and can be reverted file by file. *In the community store.*

**[GridSense](https://github.com/grub-basket/GridSense)** — an Excel-grade grid over your
frontmatter, for when you'd rather edit data than open notes one at a time. Rows are
notes, columns are properties, keys behave the way spreadsheet keys should, and every
write goes through Obsidian's own frontmatter API so note bodies are never touched.
*In the community store.*

**[Trynalist](https://github.com/grub-basket/Trynalist)** — a Dynalist-style outliner
where every line of the outline is a real Markdown note. Structure lives in frontmatter,
the file body is the line plus its note, and there are four views over the same data:
outline, flat, article, and a mind map. Nothing is locked inside the plugin. *Beta
software — via BRAT, expect rough edges.*

**[Draft Tabs](https://github.com/grub-basket/Draft-Tabs)** — keep several drafts of the
same note and flip between them with a tab strip above the editor. Rewrite a paragraph
three ways, branch an outline, or keep a safe copy before you gut something. Each draft
is an ordinary Markdown note. *Beta software — via BRAT, expect rough edges.*

**[Starter Packs](https://github.com/grub-basket/starter-packs)** — share a curated set of
plugins and themes as a link or a short paste-anywhere code, the way Bluesky starter packs
work. Annotate each pick with your own note; on the other end everything installs
*disabled* until the recipient reviews the pack.

**[Slide and Reveal](https://github.com/grub-basket/SnR)** — flashcard-style study of
labeled images: anatomy plates, diagrams, maps, sheet music. Drop covers on the labels and
scroll inside the image to uncover them a group at a time, instead of duplicating a slide
per label the way you'd have to in PowerPoint. There's also a quiz mode that pulls cropped
fragments from a whole folder and asks you to identify them out of context.

### What the forks fix

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

---

Anything not in the community store installs through
[BRAT](https://github.com/TfTHacker/obsidian42-brat). Issues and ideas welcome on any repo.
