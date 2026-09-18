# OneBook

OneBook is a self-contained, offline notebook application delivered as a single HTML file.

It is designed around the classic spatial notebook model of **notebooks → sections → pages**, rather than a modern web-app layout. The entire application, interface, data model, editor, styling, and functionality live inside the HTML document, with no server and no external dependencies required.

## Features

* Fully offline operation
* Single-file HTML application
* Notebook and section hierarchy
* Section tabs across the top
* Page list and page management
* Rich-text page editor
* Formatting toolbar
* Font and text-size controls
* Bold, italic, underline and strikethrough
* Superscript and subscript
* Paragraph alignment
* Bulleted and numbered lists
* Indentation controls
* Text colour and highlighting
* Paragraph styles
* Hyperlinks
* Undo and redo
* Page, section and notebook renaming
* Page, section and notebook deletion
* Search
* Light and dark themes
* Persistent theme preference
* HTML export
* No account or network connection required

## Design

OneBook deliberately uses a traditional notebook interface:

```text
┌─────────────────────────────────────────────────────────────────────┐
│ OneBook    Formatting / Editing Controls                            │
├─────────────────────────────────────────────────────────────────────┤
│ Section 1 ✎ │ Section 2 ✎ │ Section 3 ✎                            │
├───────────────┬─────────────────────────────────┬───────────────────┤
│               │                                 │                   │
│ Search        │                                 │ Pages             │
│               │                                 │                   │
│ Notebook     │          Page / Editor           │ ┌───────────────┐ │
│   ├ Section  │                                 │ │ Page 1     ⋮ │ │
│   ├ Section  │                                 │ ├───────────────┤ │
│   └ Section  │                                 │ │ Page 2     ⋮ │ │
│               │                                 │ └───────────────┘ │
│               │                                 │                   │
└───────────────┴─────────────────────────────────┴───────────────────┘
```

The intention is to keep the application's spatial relationships obvious: sections are sections, pages are pages, and the page itself remains the primary workspace.

## Offline and self-contained

OneBook does not require a backend, database server, build system, package manager, or external JavaScript libraries.

The application is contained within the HTML file. This makes it possible to keep a notebook as an ordinary file and open it directly in a compatible web browser.

The data model is embedded in the document itself, allowing the notebook to remain portable rather than depending on a proprietary online service.

## Origin

OneBook was developed from the codebase of **TiddlyWiki Classic 2.x**, retaining and adapting portions of its underlying single-file notebook architecture while substantially changing the user interface and application structure for the OneBook design.

OneBook is its own application; it is not a TiddlyWiki product.

Portions of OneBook are derived from **TiddlyWiki Classic**, created by **Jeremy Ruston and contributors**.

## TiddlyWiki Classic licensing

TiddlyWiki Classic is released under the **BSD 3-Clause License**.

Attribution:

```text
TiddlyWiki created by Jeremy Ruston and contributors.

Copyright (c) 2004-2007, Jeremy Ruston
Copyright (c) 2007-2025, UnaMesa Association
All rights reserved.
```

## Philosophy

OneBook is intended to be:

* **Portable** — a notebook should be an ordinary file.
* **Offline** — basic note-taking should not require a service.
* **Understandable** — the interface should expose the structure of the notebook directly.
* **Self-contained** — no dependency stack is required merely to open a notebook.
* **Durable** — the underlying document should remain useful independently of a particular hosted platform.

