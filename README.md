# Chakraborty Research Lab — Mind Map Guide

A shared, live lab notebook. Sign in with your account and your entries sync
instantly to every other computer in the lab — no drive to map, no manual
sync step.

---

## 1. Signing in

Open the site URL and enter the email and password your admin set up for you.
Accounts are not self-registered — ask your admin to create one.

- **Forgot password?** Click the link below Sign In and a reset email will be sent.
- **First sign-in:** you'll be asked for the display name that will appear on your
  member tab.

---

## 2. The layout

| Area | What it is |
|---|---|
| **Left sidebar** | Member tabs — one per lab member, showing their photo or initials. Click any tab to view that person's board. Toggle between **Current** and **Past** members at the top. |
| **Week columns** | The main canvas, split into calendar weeks (Sunday–Saturday). Every entry lands in the column that matches its date. |
| **Toolbar** | Runs across the top of the canvas — add nodes, filter, commit, undo/redo, export/import. |
| **Detail panel** | Slides in from the right when you click a node — shows its date, week, creation time, and connections. |
| **Header** | Lab name, Sign Out button, and (for admins) Admin Controls and Admin/Member view toggle. |

---

## 3. Adding entries

Three node shapes are available from the toolbar, each a different depth:

| Button | Shape | Color | Use for |
|---|---|---|---|
| ● **Node** | Ribbon / banner | Green | Top-level milestones and major topics |
| ■ **Sub Node** | Octagon | Blue | Smaller items under a Node |
| ◆ **Micro Node** | Parallelogram | Orange | Fine-grained details under a Sub Node |

**Attaching a new entry:**

1. Click an existing node or your project's 🙂 icon to select it (a gold ring appears).
2. Click the shape button — a popup asks for the entry's **text (max 5 words)** and **date**.
3. The new entry appears in the week column matching its date, connected to its parent.

The toolbar hint (beside Undo/Redo) always shows what your next entry will attach to.

---

## 4. Projects

Each member can run multiple independent projects on their board, each with its
own 🙂 root marker.

- **+ Add Project** opens a modal where you set the project name and an optional
  opening description.
- Project descriptions are editable bullet-point lists — hover the project's root
  circle to see and edit them.
- Click a project's 🙂 or name to open its detail panel, where you can add
  description points, add the first node, or delete the project (admin password
  required).

---

## 5. Editing

| Action | How |
|---|---|
| **Rename inline** | Click a node's text directly on the map, type, then press Enter or click away. Esc cancels. |
| **Full edit** | Click the node once to select it, then click **✎ Edit** in the toolbar. Edit the text, date, or switch the node type (Node / Sub Node / Micro Node) using the small shape buttons inside the modal. |
| **Delete** | Select the node, click **✕ Delete**. Child nodes move up and reconnect to the deleted node's parent — nothing downstream is lost. Admins must re-enter their password to confirm. |

---

## 6. Connecting nodes

Select a node, then click **🔗 Connect** in the toolbar. Search for any other
topic on the board and select it — a dashed cross-topic line links the two,
independent of the tree structure.

Click any line on the map (tree or cross-connection) to open the **line editor**:
- Switch between **Solid** and **Dotted** styles
- Pick a color from the palette or enter a custom hex
- **✕ Remove connection** deletes a cross-connection

---

## 7. Filters

Click **🔍 Filters** in the toolbar to show or hide specific projects on the map.
Useful when a board has many projects and you want to focus on one.

---

## 8. Whose board you're on

- **Your own board** — fully editable.
- **Someone else's board** — read-only. Edit controls are disabled.
- **Admins** — can edit anyone's board, including committed/locked entries.

---

## 9. Committing your work

Click **✅ Commit** (visible to admins only) to lock all current entries on a
board. Locked entries show a 🔒 badge and cannot be edited. New entries added
after a commit remain editable until the next commit.

An admin can unlock a commit via **Manage Members → Unlock**.

---

## 10. Undo / Redo

Every change is tracked. Use **↶ Undo** / **↷ Redo** in the toolbar, or
`Ctrl+Z` / `Ctrl+Y` (also `Ctrl+Shift+Z`). Undo history is per-member.

---

## 11. Export / Import

- **⬇ Export** — downloads your board as a `.json` backup file.
- **⬆ Import** — restores a backup onto your own board. You must re-enter your
  password to confirm, as importing permanently overwrites everything currently
  on the board.

---

## 12. Profile pictures

Click the small 📷 button on your own member tab to upload a photo. The image
is cropped and stored as your avatar. Admins can set or update anyone's photo.

---

## 13. Your data

All data is stored in the lab's shared Firebase database and syncs instantly to
every signed-in device. Access is enforced server-side — only authenticated lab
members can read or write anything.

---

## For admins

### Header controls

| Button | What it does |
|---|---|
| **⚙ Admin Controls ▾** | Opens a dropdown with member-level data entry settings |
| **🔓 Admin** (badge) | Toggle between your full admin view and a regular-member preview of the board |
| **🚪 Sign Out** | Signs you out |

### ⚙ Admin Controls menu

- **📅 Data entry controls** — restrict which dates a member can use for new
  entries. Options: this week and next, no restriction, from their last commit
  onward, or a custom date range. Can be applied to one member or all at once.

### 👥 Manage Members

Click **⚙ Admin Controls ▾ → Manage Members** to:

| Action | What it does |
|---|---|
| **Rename** | Change a member's display name |
| **Make admin / Remove admin** | Promote or demote admin status |
| **Mark as current / past** | Controls which sidebar tab (Current or Past) the member appears under |
| **Unlock** | Remove a commit lock so a member can edit their previous entries again |
| **Remove** | Delete the member's profile and all their data from Firestore |
| **Create Account** | Add a new member by email + display name — they receive a password-setup email automatically; nobody sees their password |

> **Note:** Removing a member's profile here does not remove their Firebase
> Authentication login. Delete that separately in the Firebase Console
> (Authentication → Users) if needed.

### Destructive actions require password confirmation

Admins must re-enter their password before:
- Deleting a node
- Deleting a project
- Deleting a description point
- Importing a backup (overwrites the board)

---

## Tips

- If the map looks empty or the camera drifted, click **Reset View** in the
  bottom-right corner.
- Live updates from other members appear while you're viewing their board —
  that's expected behavior.
- The sidebar's **Current / Past** toggle lets you archive members who have left
  the lab without deleting their data.
