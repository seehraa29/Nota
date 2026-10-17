Nota

A self-contained, offline-first notes app — one HTML file, no server required.

📄 **Single HTML file**

🔒 **Local storage only**

📁 **File System Access API**

🌙 **Multiple themes**

📴 **Works offline**

### Contents

1. [Getting Started](#getting-started)
2. [Notebooks & Organisation](#notebooks)
3. [The Editor](#editor)
4. [Markdown Shortcuts](#markdown)
5. [Search](#search)
6. [Three-Panel View](#three-panel)
7. [Import & Export](#import-export)
8. [Themes & Appearance](#themes)
9. [Keyboard Shortcuts](#keyboard)
10. [Settings Reference](#settings)

## 🚀Getting Started

Nota is distributed as a **single HTML file**. No installation, no account, no cloud. Open it in Chrome, Edge, or any Chromium-based browser and click **Open Folder** to point it at a directory on your computer — that folder becomes your note vault.

📌 Browser requirement

Nota requires the **File System Access API**, available in Chrome 86+, Edge 86+, and Brave. Firefox and Safari are not currently supported.

### First launch

1. Open `Nota.html` in a supported browser
2. Click **Open Folder** in the sidebar and choose (or create) a folder for your notes
3. Grant read/write permission when the browser prompts
4. Click **＋** to create your first notebook, then create notes inside it

💡 Tip

Each note is saved as a plain `.html` file in your chosen folder. You can browse and back up your notes with any file manager, version control system, or cloud sync tool.

Nota — Two-pane view

Nota

🔍 Search notes…

NOTEBOOKS

📓 Archive 101

📓 Personal 13

📓 Journal 8

📓 Work 27

Project kickoff notes

Oct 12, 2026

Weekly review

Oct 10, 2026

Ideas — Q4

Oct 8, 2026

Project kickoff notes

Oct 12, 2026 · 347 words · \~2 min read

B

*I*

U

H1

H2

≡

⌘

⊞

🔗

📎

## Attendees

Sarah (PM), Dev team leads, design ×2. Remote via Meet.

## Action items

- Set up repo and CI pipeline
- Schedule design review for Friday

#project#q4

## 📁Notebooks & Organisation

Notes are grouped into **notebooks**. Notebooks can have one level of **sub-notebooks**. Every note lives in exactly one notebook (or in the root, unfiled area).

📓

#### Create notebooks

Click **＋** in the sidebar header or right-click any notebook.

⊕

#### Sub-notebooks

Hover a notebook row to reveal the **⊕** button and create a nested notebook one level deep.

🎨

#### Icons & colours

Right-click a notebook to set a custom emoji icon and a colour accent for the sidebar.

✏️

#### Rename & delete

Right-click any notebook for rename and delete options. Deleting removes all notes inside.

🖱️

#### Drag notes

Drag any note from the sidebar and drop it onto a notebook or sub-notebook to move it instantly.

📌

#### Pin notes

Right-click a note → *Pin Note* to keep it fixed at the top of its notebook, regardless of sort order.

### Right-click context menus

Both notebooks and notes have rich right-click menus:

- **Notebook:** New Note, New Note from Template, Rename, Change Icon, Set Colour, Delete
- **Note:** Pin/Unpin, Rename, Move to Notebook, Duplicate, Export as Markdown, Delete

### Tags

Add `#hashtags` anywhere in a note body. Tags are extracted automatically and displayed as clickable chips below the note title. Clicking a tag chip populates the search box with `#tagname` to show all notes with that tag.

## ✏️The Editor

Nota uses a rich text editor with a formatting toolbar. Content is stored as HTML, preserving formatting, tables, code blocks, and embedded media across sessions.

### Formatting toolbar

- **Text style:** Bold, Italic, Underline, Strikethrough, Highlight, Text colour
- **Structure:** Headings (H1–H3), Bullet list, Numbered list, Blockquote, Horizontal rule
- **Insert:** Link, Code block, Table, Image, Markdown import, Attachment
- **History:** Back / Forward navigation between recently viewed notes

### Code blocks

Insert a syntax-highlighted code block via the toolbar or by typing ```` ```lang ```` and pressing Enter. Supported languages include JavaScript, Python, SQL, Bash, and [anything highlight.js supports](https://highlightjs.org/usage/). Click the pencil icon to edit, the copy icon to copy to clipboard.

💡 Code block at the top of a note

If a code block is the very first element in a note, press ↑ or Backspace to insert a blank line above it so you can type before the code block.

### Tables

Insert tables via the toolbar. Tables support **Ctrl+Click** to select entire rows or columns, **Ctrl+C** to copy as TSV (paste into Excel/Sheets), and **Ctrl+V** to paste TSV data back in.

### Note links

Type `[[` to open an autocomplete picker. Select a note title to insert a clickable link. Following a link opens that note, and the back button returns you to the previous note.

### Word count & reading time

The area below the note title shows **date, word count, reading time estimate, and character count**, updated live as you type.

### Word count goal

Set a writing goal via Settings → *Set Word Count Goal*. A progress bar appears below the note title as you work towards it.

### Find in note

Press Ctrl+F or Ctrl+H to open the find bar. All matches are highlighted; use the arrows to step through them.

## ⌨️Markdown Shortcuts

Type markdown-style shortcuts at the start of a blank line and press Space or Enter — the text converts to rich formatting instantly.

| Type this | Then press | Result |
| --- | --- | --- |
| # | Space | Heading 1 |
| ## | Space | Heading 2 |
| ### (up to ######) | Space | Heading 3–6 |
| - or * or + | Space | Unordered (bullet) list |
| 1. | Space | Ordered (numbered) list |
| > | Space | Blockquote |
| --- or \*\*\* or \_\_\_ | Enter | Horizontal rule |
| \`\`\`js (any language) | Enter | Syntax-highlighted code block |

### Markdown paste

Copy markdown text from anywhere, then click the **.md paste** button in the toolbar (or use the *Import Markdown file* button) to convert a full markdown document into rich formatted content.

📌 Note

Inline markdown within existing text (like wrapping words in `**`) is not auto-converted — use the toolbar buttons for inline formatting, or the paste function for full documents.

## 🔍Search

The search box at the top of the sidebar searches across **all notes in all notebooks** simultaneously, matching both titles and body text.

Full-text search with body snippets

Nota

🔍 postgres connection…

Setting up PostgreSQL

Archive › PostgreSQL

Node.js backend setup

Archive › Node.js

…configure the postgres connection string in .env before running…

Docker Compose reference

Work › DevOps

…the postgres connection pool defaults to 10 concurrent…

🔍

3 notes match "postgres connection"

### Search features

- **Body snippets:** When a match is found in the note body (not just the title), a short excerpt is shown beneath the note title with the matching text highlighted.
- **Tag search:** Type `#tagname` to filter notes by tag. Click any tag chip in the editor to pre-fill this automatically.
- **Instant results:** Results update on every keystroke — no need to press Enter.

## ⫴Three-Panel View

Enable via **Settings → Three-Panel View**. The layout splits into three resizable panels, similar to Joplin or Bear.

Three-panel view

Nota

📓Archive

📓AI

📓Postgres

📓React

📓Personal

📓Work

Archive › React

🔍 Search notes…

React Hooks guide

useState & useEffect

Component patterns

Performance tips

React Router v6

React Hooks guide

Jul 1, 2026 · 360 words

B

*I*

H1

H2

≡

⊞

# React Hooks guide

Hooks let you use state and lifecycle features in function components. Introduced in React 16.8 — no class components needed.

## Common hooks

`useState` manages local state. `useEffect` handles side effects like data fetching and subscriptions.

### How it works

- **Left panel — Notebooks:** Click a notebook (or sub-notebook) to populate the middle panel. Parent notebooks expand/collapse. Drag notes from the middle panel and drop them onto any notebook row to move them.
- **Middle panel — Notes:** Shows all notes in the selected notebook. Search box and sort buttons (Date / A→Z) at the top. **＋ New Note** button at the bottom. Right-click any note for the full context menu (rename, move, duplicate, delete).
- **Right panel — Editor:** The full note editor, unchanged.

- All three panels are **independently resizable** by dragging the dividers.
- Panel widths and the three-panel preference are saved across sessions.
- A **📁 New Notebook** button sits at the bottom of the left panel.
- Right-clicking a notebook row shows the full notebook context menu (rename, icon, colour, delete).

## ↕️Import & Export

### Import

- **Single Markdown file:** Click the **.md** button in the editor toolbar to import a `.md` file into the current note. Fenced code blocks are converted to interactive code widgets. Windows line endings (`\r\n`) are handled automatically.
- **Bulk Markdown import:** Settings → *Bulk Import Markdown…* — select multiple `.md` files or drag & drop them. Choose a destination notebook. Each file becomes a separate note; the title is taken from the first `#` heading or the filename.
- **JSON backup:** Settings → *Export / Import…* → Import from JSON.

### Export

- **Note as Markdown:** Right-click any note → *Export as Markdown*.
- **Full backup as JSON:** Settings → *Export / Import…* → Export all notes.
- **Print / PDF:** Settings → *Print / Export Notebook…* or Ctrl+P. The print stylesheet strips the UI and produces clean output.

## 🎨Themes & Appearance

Click the theme swatch button in the top-right corner to open the theme picker. The chosen theme is saved automatically.

Parchment

Warm cream · default

Dark Slate

Blue-grey dark

Dark Warm

Amber on brown

High Contrast

Max legibility

Ocean

Cool blue-grey

Forest

Soft green

Rose

Warm pink

Mono

Black & white

### Additional appearance settings

- **Custom accent colour:** Settings → *Custom Accent Colour…* to override the theme's accent with any colour.
- **Compact Sidebar:** Settings → *Compact Sidebar* tightens padding and font sizes throughout the sidebar — useful on 14" laptops or smaller displays. Saved automatically.
- **Swap Sidebar Side:** Move the sidebar from left to right.
- **Zen mode:** Press F11 to hide everything except the note body for distraction-free writing.

## ⌨️Keyboard Shortcuts

Ctrl+S

Save current note

Ctrl+N

New note

Ctrl+F

Find in note

Ctrl+H

Find in note (alternate)

Ctrl+P

Print / export to PDF

Ctrl+Z

Undo

Ctrl+Shift+V

Paste as plain text

F11

Toggle zen mode

Tab

Insert two spaces (in editor)

↑ at note start

Insert line above code block

Ctrl+C on table selection

Copy table as TSV

Ctrl+V into table

Paste TSV into table

## ⚙️Settings Reference

Access all settings via the **⚙ gear icon** in the top-right corner.

| Setting | Description |
| --- | --- |
| Export / Import… | Full JSON backup or restore of all notes |
| Bulk Import Markdown… | Import multiple .md files into a chosen notebook |
| Swap Sidebar Side | Move sidebar between left and right |
| Compact Sidebar | Tighter spacing for small screens |
| Three-Panel View | Joplin-style three-column layout |
| Folder Encryption… | Password-protect notes at rest (AES-256) |
| Custom Accent Colour… | Override theme accent with any hex colour |
| Set Word Count Goal… | Show a progress bar towards a writing target |
| Autosave interval | Cycle through 0.8s / 1.2s / 2s / 5s / manual |
| Print / Export Notebook… | Render all notes in a notebook for print or PDF |

⚠️ Encryption

When folder encryption is enabled, all notes are re-encrypted with AES-256 using your password. **There is no password recovery.** Keep a backup of your unencrypted notes before enabling this feature.

Nota — offline-first notes in a single HTML file.

Built with the File System Access API · No server · No account · Your files stay yours.
