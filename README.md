# Chakraborty Research Lab — Mind Map Guide

A single-file, self-contained lab notebook. No install, no server, no account —
just a `.html` file that saves your data in the browser it's opened in.

## 1. Opening it

Double-click `chakraborty-lab-mindmap.html` to open it in your default browser,
or drag it into an open browser window.

> **First run:** the browser will ask for your name once (a plain browser
> prompt). This sets up your single workspace — there's no separate "Add
> Member" step.

## 2. The layout

- The map is organized into **week columns**, each covering one real
  calendar week (Sunday–Saturday). A node's position always follows its date.
- Your **project** is marked by a big 🙂 emoji on the left, with the project
  name in bold beside it and how many topics it holds underneath.
- Every entry (node) sits in the week column that matches its date, and
  connects back to whatever it was added under with a curved line.

## 3. Adding entries

Three shapes are available from the toolbar, each a different "depth":

| Button | Shape | Use for |
|---|---|---|
| ● **Node** | ribbon/banner, full column width | top-level milestones |
| ■ **Sub Node** | squared octagon, ⅓ column width | smaller items under a Node |
| ◆ **Sub Sub Node** | parallelogram, full column width | detail under a Sub Node |

**Where a new entry attaches** depends on what's currently selected:

- Click any node on the map first (it gets a gold ring around it) — the next
  thing you add becomes its child.
- Click the project's 🙂 emoji to attach fresh top-level entries to the
  project directly.
- The toolbar hint text (next to Undo/Redo) always tells you what you're
  "continuing from."

A popup asks for the entry's **text (max 5 words)** and **date** — the date
decides which week column it lands in.

## 4. Editing

- **Rename:** click directly on a node's text on the map, type, and press
  Enter (or click away) to save. Esc cancels.
- **Full edit / change type / delete / connect:** click a node once to select
  it, then use the **✎ Edit**, 🔗 **Connect**, or ✕ **Delete** buttons that
  appear in the toolbar (top right).
  - Inside **Edit**, a row of small shape buttons lets you switch the node
    between Node / Sub Node / Sub Sub Node without moving it in the tree.
- **Deleting** a node keeps its own sub-nodes — they just move up to take its
  place, reconnecting to whatever came before it. Nothing "downstream" is
  lost.

## 5. Adding descriptions

Hover any node to reveal a popup with 🙂-marked points. Type in a box, click
**+ Add 🙂** for another, or ✕ to remove one — each point is capped at 20
words. Click a node (rather than hover) to see the same points numbered in
the right-hand detail panel, along with its date, week, creation time, and
what it's connected to.

## 6. Repositioning

Each node has a small 🙂 grip (with ▲/▼ arrows) on its left edge — drag it
up or down to nudge the node within its own week column. Double-click the
grip to snap it back to automatic placement.

## 7. Connecting nodes across the map

Select a node, click 🔗 **Connect**, and search for another topic to link to
it (a dashed cross-topic line, independent of the tree structure). Click any
line on the map — tree or cross-connection — to change its color/style or
(for cross-connections) remove it.

## 8. Projects

**+ Add Project** starts a second independent trail with its own 🙂 marker.
Click a project's 🙂/name and use the panel's **+ Add Node** / **✕ Delete
Project** actions.

## 9. Undo / Redo

Every change is tracked — use the toolbar buttons or `Ctrl+Z` / `Ctrl+Y`
(`Ctrl+Shift+Z` also works for redo).

## 10. Your data

Everything is saved to the browser's **localStorage**, tied to this specific
file and browser:

- It **won't sync** across different browsers or computers.
- Clearing that browser's site data/history will erase it.
- There's currently no built-in export/backup — if you want a safety copy,
  ask for that feature and it can be added.

## Tips

- If the map looks empty or you want to reset the camera, click **Reset
  View** in the bottom-right corner.
- Multiple browser tabs open on the same file share the same saved data —
  edits in one won't appear in another until you reload it.
