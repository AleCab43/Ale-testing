# Consortium Desk

A simple project management tool for EU-funded projects (Horizon Europe, Erasmus+, Interreg, LIFE and others).
It is a single `index.html` file: there is nothing to install and no server is needed.

## Use it

Open `index.html` in any modern browser. To share it with your team, turn on GitHub Pages for this repository
(Settings → Pages → deploy from branch) and send them the link.

## What it does

- **Overview**: the current project month (e.g. *Month 10 of 36*), reporting periods, what's due next, overdue items, and progress for each work package.
- **Tasks**: a board (To do / In progress / In review / Done) with drag and drop, and filters by WP, partner or keyword.
- **Timeline**: a Gantt chart in project months (M1…Mn) showing WPs, tasks, deliverables (◆) and milestones (●).
- **Deliverables & milestones**: tables that follow Grant Agreement conventions: D-numbers, type (R, DEM, DEC, DATA…), dissemination level (PU/SEN), due month and status up to "Approved by EC".
- **Work packages** and **Partners** (coordinator, beneficiaries, affiliated entities…).
- Several projects side by side, with a project switcher.
- **IMREG proposal template**: one click on *+ IMREG proposal template* creates a proposal-preparation project for Context Romania (PIC 885595257) for the DG REGIO IMREG call: eligibility go/no-go, media concept, audience/KPI plan, Part B sections per award criterion, editorial independence, publication calendar, budget check against the funding rate and ceiling, and an evaluator review. Call dates and figures are not filled in: they are marked [TO CONFIRM] until checked against the current call document. The start month defaults to the current month; change it in *Project details*.

## Your data

Data is saved in your browser (localStorage), on your computer only. Use **Backup & restore** to download a `.json`
backup regularly, to move to another computer, or to send a project to a colleague.
The app starts with a sample project marked *Example*. Remove it, or edit it into your own.
