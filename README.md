<p align="center">
  <img src="https://github.com/daSkier/notis-releases/raw/main/screenshots/editor-light.png" width="800" alt="Notis — Markdown note-taking for professionals">
</p>

<h1 align="center">Notis</h1>

<p align="center">
  <strong>Markdown note-taking for professionals who take meeting notes and need cross-note task visibility.</strong>
</p>

<p align="center">
  <a href="https://github.com/daSkier/notis-releases/releases/latest"><img src="https://img.shields.io/github/v/release/daSkier/notis-releases?style=flat-square&label=download&color=007AFF" alt="Download Latest"></a>
  <img src="https://img.shields.io/badge/platform-macOS%2015+-333?style=flat-square&logo=apple&logoColor=white" alt="macOS 15+">
  <a href="https://notis.hotdish.dev"><img src="https://img.shields.io/badge/web-notis.hotdish.dev-4285F4?style=flat-square" alt="Web App"></a>
</p>

---

## Download

**[Download the latest release](https://github.com/daSkier/notis-releases/releases/latest)** — macOS 15+, Apple Silicon and Intel.

Notis auto-updates via Sparkle. Once installed, updates are applied automatically in the background.

---

## What Is Notis?

Notis connects your calendar to your notes. Create meeting notes directly from calendar events, write in markdown with live inline rendering, and aggregate tasks across every note you've ever written.

**The core workflow:** You're in a meeting, you take notes, you assign tasks with `@mentions` and `#topics`, and later you can instantly answer *"What are all outstanding items for @sarah?"* across your entire vault.

---

## Features

### Live Markdown Editor

Write in markdown with real-time syntax highlighting. Syntax characters dim when your cursor moves away, headings render at display size, and checkboxes become interactive controls.

<p align="center">
  <img src="https://github.com/daSkier/notis-releases/raw/main/screenshots/editor-light.png" width="700" alt="Markdown editor with live rendering">
</p>

- Inline tokens: `@mentions` (blue), `#topics` (purple), `due:dates` (orange), `[[wiki-links]]` (cyan)
- Interactive checkboxes, styled list markers, vertical indent guides
- Autocomplete for `@mentions` and `#topics` ranked by usage frequency
- Optional format bar for quick access to Bold, Italic, Code, Headings, Links
- Inline image previews (Obsidian-style Live Preview)

### Cross-Note Task Aggregation

View all tasks from all notes in one place. Filter by person, topic, due date, or completion status. Save filters for quick access.

<p align="center">
  <img src="https://github.com/daSkier/notis-releases/raw/main/screenshots/tasks-light.png" width="700" alt="Task aggregation across all notes">
</p>

- Filter by `@person`, `#topic`, completion, due date
- Save named filters (e.g. "My Tasks", "Due This Week")
- Click any task to jump to the exact line in the source note
- Sub-context (indented lines) preserved and expandable

### Calendar Integration

Connect your calendars (EventKit + Google Calendar API) and create meeting notes with one click. Events show attendees, meeting links, and link back to existing notes.

<p align="center">
  <img src="https://github.com/daSkier/notis-releases/raw/main/screenshots/calendar-light.png" width="700" alt="Calendar sidebar with events">
</p>

- Day view sidebar with chronological event list
- One-click meeting note creation from any event
- Direct Google Calendar API integration with OAuth
- Pre-populated attendees, meeting links, and metadata
- Configurable note templates per calendar
- Join meeting buttons for Zoom, Meet, and Teams

### Folder Management

Organize notes in a hierarchical folder tree. Create, rename, and move folders directly from the sidebar.

<p align="center">
  <img src="https://github.com/daSkier/notis-releases/raw/main/screenshots/folders-light.png" width="700" alt="Folder tree in sidebar">
</p>

### Plain Markdown Files

Your notes are standard `.md` files with YAML frontmatter. No proprietary format, no database lock-in. Store them anywhere — iCloud Drive, Dropbox, or a local folder. Cross-device sync works with any file sync service.

```markdown
---
created: 2026-03-22T10:00:00
event_id: "abc123"
attendees: ["@sarah", "@mike"]
meeting_link: "https://zoom.us/j/123456"
---

# Weekly Sync

## Action Items
- [ ] Review mockups @mike #design due:2026-03-28
- [x] Share research @sarah #user-research
```

---

## Dark Mode

Full dark mode support with a consistent design across every panel.

| Light | Dark |
|:-----:|:----:|
| <img src="https://github.com/daSkier/notis-releases/raw/main/screenshots/editor-light.png" width="400"> | <img src="https://github.com/daSkier/notis-releases/raw/main/screenshots/editor-dark.png" width="400"> |

---

## Web App

Notis is also available as a web app at **[notis.hotdish.dev](https://notis.hotdish.dev)**. Built with React, CodeMirror 6, and Cloudflare Workers, it provides the same core features — markdown editing, task aggregation, and calendar integration — accessible from any browser.

---

## Requirements

- macOS 15.0 (Sequoia) or later
- Apple Silicon or Intel Mac

## Installation

1. **[Download the latest DMG](https://github.com/daSkier/notis-releases/releases/latest)**
2. Open the DMG and drag Notis to Applications
3. Launch Notis — it will ask where to create your vault (default: `~/Documents/Notis`)
4. Start writing

Updates are delivered automatically via Sparkle.

---

<p align="center">
  <sub>Built with SwiftUI, TextKit 2, GRDB, and too much coffee.</sub>
</p>
