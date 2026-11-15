# Taskforge

A lightweight, local-first project management workspace for organizing tasks across a customizable workflow. Taskforge combines a Kanban-style board with table, progress, and activity views in a restrained interface inspired by Microsoft Fluent 2.

## Preview

The application opens on the Board view with sample tasks so the interface is immediately understandable.

## Features

- **Board view:** organize work across customizable columns and move task cards with drag and drop.
- **Grid view:** review tasks in a compact table.
- **Charts view:** see task counts grouped by workflow status.
- **Activity view:** review recent task and column changes.
- **Task management:** create, edit, complete, move, and delete tasks.
- **Column management:** add, rename, and delete workflow columns. When a column is deleted, its tasks are moved to another remaining column.
- **Task details:** descriptions, priority levels, and due dates, including overdue indicators.
- **Search and filtering:** find tasks by title or description and filter by priority.
- **Persistence:** automatically save the workspace in the browser's `localStorage`.
- **JSON export:** download a backup of tasks, columns, and activity.
- **Theme and responsive layout:** switch between light and dark themes and use the interface on smaller screens.
- **In-app dialogs:** task editing, column naming, and destructive-action confirmations use dialogs styled to match the application rather than browser-native prompts.

## Technology

- HTML5
- CSS3 (custom properties, responsive layout, and theme variables)
- Vanilla JavaScript (ES6+)
- Browser `localStorage` and the File/Blob APIs
- Inline SVG icons

There are no runtime dependencies, build tools, or package installation steps.

## To Run locally

1. Clone the repository:

   ```bash
   git clone https://github.com/WraithISC/project-taskforge.git
   cd project-taskforge
   ```

2. Open `index.html` directly in a modern browser, **or** start a local static server:

   ```bash
   python -m http.server 8000
   ```

3. Visit `http://localhost:8000`.

No Node.js installation or `npm install` is required.

## Data and privacy

Taskforge stores its workspace in the current browser profile using `localStorage`. Your tasks are not sent to a server by this version. Use **Export** to download a JSON backup before clearing browser data or moving to another device.

## Known limitations

- This is a frontend-only, single-user prototype; there is no backend, account system, team collaboration, or cross-device synchronization.
- Workspace data is browser-local. Clearing site data can remove the saved workspace; export backups regularly.
- The Charts view currently shows task counts by column rather than advanced reporting or historical trends.
- There is no import workflow for restoring an exported JSON backup yet.
- Drag and drop is designed primarily for pointer-based desktop interaction; use the task's action menu to move tasks when drag and drop is unavailable.

## Visit it as a Website.

Here "https://wraithisc.github.io/project-taskforge/" !

