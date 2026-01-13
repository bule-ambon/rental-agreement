# AGENT Rules

These rules define the workflow and constraints an AGENT must follow in this repository.

## 1) Initial Analysis and Planning
- AGENT must read relevant files before coding.
- AGENT must write a task plan to `tasks/todo.md` before making changes.

## 2) Design Inspiration (Do Not Modify)
- A directory named `design/` (or similar) may contain CSS/Bootstrap templates.
- AGENT is **forbidden** from modifying anything inside `design/`.

## 3) To-do List Structure
- The plan in `tasks/todo.md` must use checkboxes (markdown task list items), e.g.:
  - [ ] Step
  - [x] Done

## 4) Plan Verification
- After drafting the plan, AGENT must ask the user to verify/approve the plan **before** beginning work.

## 5) Task Execution
- AGENT must work through the to-do items in order.
- AGENT must mark items complete as they are finished so work can resume after interruptions.

## 6) Communication
- At every step, AGENT must provide a high-level explanation of changes made.

## 7) Simplicity Principle
- Every change must be as simple as possible.
- Minimize surface area: touch as little code as possible to achieve the goal.

## 8) Process Documentation
- AGENT must append a log of actions and the user’s prompts to `docs/activity.md`.

## 9) Git Repository Hygiene
- Successful changes must be committed and pushed immediately.
- Use small commits with clear messages so it’s easy to revert.

## 10) The HTML Folder (LAMP Stack Projects)
- All deployable files must reside within the `html/` folder or its subfolders.

## 11) ID Tags in HTML
- Every `<div>` tag must have a unique `id` attribute.
- This enables precise UI edits by referencing specific elements.

## 12) Review Process
- AGENT must add a short summary of changes to `tasks/todo.md`.
- Full documentation belongs in `docs/activity.md`.

---
## Notes / Defaults
- If `tasks/` or `docs/` do not exist, AGENT should create them.
- If `tasks/todo.md` or `docs/activity.md` do not exist, AGENT should create them.
