# Consortium Desk

A simple project management tool for EU-funded projects (Horizon Europe, Erasmus+, Interreg, IMREG, LIFE and others).
It is a single `index.html` file: there is nothing to install and no server is needed.

## Open it

1. Download this repository (green **Code** button → **Download ZIP**) and unzip it, or download just `index.html`.
2. Double-click `index.html`. It opens in your default browser (Chrome, Edge, Firefox or Safari).
3. You start with a sample project marked *Example*. Click **Start my project** to create your own, or **Remove example**.

It also works offline. Without internet the page uses your system fonts instead of the web fonts, and nothing else changes.

To share it with your team, turn on GitHub Pages for this repository
(Settings → Pages → deploy from branch) and send them the link. Each person still keeps their own data (see below).

## What it does

- **Overview**: the current project month (e.g. *Month 10 of 36*), reporting periods, what's due next, overdue items, and progress for each work package.
- **Tasks**: a board (To do / In progress / In review / Done) with drag and drop, and filters by WP, partner or keyword.
- **Timeline**: a Gantt chart in project months (M1…Mn) showing WPs, tasks, deliverables (◆) and milestones (●).
- **Deliverables & milestones**: tables that follow Grant Agreement conventions: D-numbers, type (R, DEM, DEC, DATA…), dissemination level (PU/SEN), due month and status up to "Approved by EC".
- **Work packages** and **Partners** (coordinator, beneficiaries, affiliated entities…).
- Several projects side by side, with a project switcher.

## Your data

Data is saved in your browser (localStorage), on your computer only. It stays there when you close the tab,
but it is lost if you clear your browser data, and a different browser or computer will not see it.

Use **Backup & restore** (bottom of the sidebar; on a phone, at the top under the menu) to download a `.json` backup regularly,
to move to another computer, or to send a project to a colleague. Restoring adds the projects from the backup next to the ones you have.

## Edit the tool itself

Everything is in `index.html`: the styles in the `<style>` block at the top, and the app in the `<script>` block at the bottom.
Open the file in any text editor (VS Code, Notepad++, TextEdit in plain-text mode), save, and reload the page in the browser.

Common changes, all near the top of the `<script>` block:

| To change | Edit |
| --- | --- |
| Programmes in the project form | `PROGRAMMES` |
| Partner roles | `ROLES` |
| Task board columns | `TASK_STATUS` |
| Deliverable statuses, types, dissemination levels | `DEL_STATUS`, `DEL_TYPES`, `DISS` |
| Work package colours | `WP_COLORS` |
| The sample project | `sampleProject()` |
| Colours of the interface | the `--…` variables in `:root` at the top of `<style>` |

If you rename the values (the first item in each pair, such as `'todo'`), existing saved items that use the old value
will no longer match. Changing only the labels (the second item, such as `'To do'`) is always safe.
Make a backup before you edit the file, in case something goes wrong.
