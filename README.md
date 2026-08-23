<h1>Hello!</h1>

I have Claude Code use LLM models Opus and Fable to build plugins for [Obsidian](https://obsidian.md) — mostly for capturing things fast
and for editing a lot of notes at once.

### Newest projects

<a href="https://github.com/grub-basket/Trynalist"><img width="215" alt="Trynalist" src="https://img.shields.io/badge/Trynalist-A%20Dynalist--style%20outliner-4c6ef5?style=for-the-badge"></a>
<a href="https://github.com/grub-basket/Sync-Sentinel"><img width="215" alt="Sync Sentinel" src="https://img.shields.io/badge/Sync%20Sentinel-Sync%20your%20huge%20files-4c6ef5?style=for-the-badge"></a>

**Trynalist** — import your Dynalist OPML or JSON and keep working the way you did, same
keyboard chords and four views over the same outline, except every line is a real Markdown
file in your vault.

**Sync Sentinel** — Obsidian Sync quietly refuses anything past its size limit. This splits
those files into shards it will carry, and rebuilds them byte-for-byte on the other side.

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
outline, flat, article, and a read-only mind map. Mirrors window a subtree from another
document, and imports come from Dynalist OPML, Dynalist JSON, or indented text — so
nothing is locked inside the plugin on the way in or out. *Beta software — via BRAT for
now, expect rough edges.*

**[Draft Tabs](https://github.com/grub-basket/Draft-Tabs)** — keep several drafts of the
same note and flip between them with a tab strip above the editor. Rewrite a paragraph
three ways, branch an outline, or keep a safe copy before you gut something. Each draft
is an ordinary Markdown note. *Beta software — via BRAT for now, expect rough edges.*

**[Sync Sentinel](https://github.com/grub-basket/Sync-Sentinel)** — Obsidian Sync silently
refuses files past its size limit, so your 200 MB video never leaves the laptop it was made
on. Sync Sentinel splits those into shards small enough for Sync to carry, then rebuilds the
original byte-for-byte on your other devices, checked against SHA-256 hashes at every step.
It also tracks which devices hold what, so you can reclaim the shard space once everyone has
the real file. *Beta software, desktop only — via BRAT.*

### Community forks

Other people's plugins, patched. Some of it is offered back upstream, some of it ships
as a fork because upstream has gone quiet.

**[Scroll Buttons](https://github.com/grub-basket/obsidian-scroll-buttons)** — top / page
up / page down / bottom buttons and commands, originally built for e-ink devices where
normal scrolling leaves ghosting. Adopted from [triski](https://github.com/chenshutian9610),
with per-button toggles, smart hiding so they stay out of other plugins' way, and pop-out
window support added. *Via BRAT — it shares the store version's plugin ID, so disable
Page Scroll first.*

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

### Patches for other people's projects

Bug fixes sent upstream to [jorio](https://github.com/jorio)'s projects — his Git UI and
the retro-Mac libraries and tools behind his ports of the old Pangea games. So far:
[GitFourchette](https://github.com/jorio/gitfourchette),
[Pomme](https://github.com/jorio/Pomme),
[rsrcdump](https://github.com/jorio/rsrcdump),
[OldMacArchiver](https://github.com/jorio/OldMacArchiver),
[PROBE](https://github.com/jorio/PROBE), and [his profile
README](https://github.com/jorio/jorio) — which is what this page is modelled on.

[Retrace](https://github.com/haseab/retrace), an open-source Rewind-style screen-history
app for macOS, has a run of seven: the SQLCipher key no longer gets destroyed on a
transient Keychain error (it fails closed rather than quietly falling back to plaintext),
search works with encryption on, the key is redacted from error text, and redaction
masking fails closed instead of persisting an unmasked frame — plus a JPEG encoding path
that skips a TIFF round-trip.

Also [Blot](https://github.com/davidmerfield/blot), the folder-into-a-website publishing
platform, where [a batch of small correctness
fixes](https://github.com/davidmerfield/blot/pull/1616) was merged.

---

The forks install through [BRAT](https://github.com/TfTHacker/obsidian42-brat) too.
Issues and ideas welcome on any repo.
