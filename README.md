# Chakraborty Research Lab — Mind Map Guide

A shared lab notebook, live for everyone in the lab. Sign in with your account
and your entries sync instantly to every other computer — no drive to map, no
manual sync step.

## 1. Signing in

Open the site's URL and sign in with the email and password your admin set up
for you. Don't have a login? Ask your admin — new logins are created for you,
not self-registered.

The very first time you sign in, you'll be asked what name should show for
you in the lab map — that's the only setup step.

## 2. The layout

- The map is organized into **week columns**, each covering one real
  calendar week (Sunday–Saturday). A node's position always follows its date.
- Your **project** is marked by a big 🙂 emoji on the left, with the project
  name in bold beside it and how many topics it holds underneath.
- Every entry (node) sits in the week column that matches its date, and
  connects back to whatever it was added under with a curved line.
- The **left sidebar** lists every lab member as a tab, with their photo (or
  initials). Click a tab to view that person's board.

## 3. Whose board you're looking at

- **Your own board** — fully editable.
- **Someone else's board** — read-only. You can look, but every edit control
  is disabled.
- **Admins** can edit anyone's board, including committed/locked entries.

## 4. Adding entries

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

## 5. Editing

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

## 6. Adding descriptions

Hover any node to reveal a popup with 🙂-marked points. Type in a box, click
**+ Add 🙂** for another, or ✕ to remove one — each point is capped at 20
words. Click a node (rather than hover) to see the same points numbered in
the right-hand detail panel, along with its date, week, creation time, and
what it's connected to.

## 7. Repositioning

Each node has a small 🙂 grip (with ▲/▼ arrows) on its left edge — drag it
up or down to nudge the node within its own week column. Double-click the
grip to snap it back to automatic placement. This still works even after
your entries are committed — only the content itself locks, not its position.

## 8. Connecting nodes across the map

Select a node, click 🔗 **Connect**, and search for another topic to link to
it (a dashed cross-topic line, independent of the tree structure). Click any
line on the map — tree or cross-connection — to change its color/style or
(for cross-connections) remove it.

## 9. Projects

**+ Add Project** starts a second independent trail with its own 🙂 marker.
Click a project's 🙂/name and use the panel's **+ Add Node** / **✕ Delete
Project** actions.

## 10. Committing your work

Click **✅ Commit** to lock in everything you've entered so far — it becomes
read-only (marked with a 🔒 badge), protecting it from later accidental
edits. You can still add brand-new entries afterward; they stay editable
until your next commit. An admin can unlock a commit for you if you need to
go back and fix something.

## 11. Profile pictures

Click the small 📷 button on your own tab in the sidebar to set a profile
picture. Admins can set anyone's.

## 12. Undo / Redo

Every change is tracked — use the toolbar buttons or `Ctrl+Z` / `Ctrl+Y`
(`Ctrl+Shift+Z` also works for redo). Undo is per-member, tied to whichever
board you were just editing.

## 13. Your data

Everything is stored live in the lab's shared database and synced instantly
to every signed-in computer — there's no local file, no drive to map, and no
manual sync step. Only signed-in lab members can read or write anything; the
permission rules are enforced on the server, not just in this page.

Use **⬇ Export** any time to download your own board as a `.json` backup.
**⬆ Import** restores a backup into your own board (never someone else's).

## For admins

- **👥 Manage Members** (top right, visible only to admins) lets you rename a
  member, promote/demote other admins, unlock a commit, or remove a member's
  profile.
- New logins are created in the Firebase Console (Authentication → Users),
  not from inside the app — a member's profile then appears automatically
  the first time they sign in.

## Tips

- If the map looks empty or you want to reset the camera, click **Reset
  View** in the bottom-right corner.
- Changes from other members can appear while you're looking at their board
  — that's expected, it's live.
