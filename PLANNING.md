
### Ethos-MD5SUM Project Awareness and Context
- **Always read `README.md`** at the start of a new conversation to understand the project's architecture, goals, style, and constraints.
- **Always read `UI.md`** at the start of a new conversation to understand the components and information related to the Project UI.
- **Check `TASK.md`** before starting a new task.  If the task isn't listed, add it with a brief description and today's date.  
- **Check for any additional Markdown files and if they exist read these after the `README.md`, and `UI.md` files for more understanding.**
- **Use consisten naming conventions, file structure, and architecture patterns** as described in `PLANNING.md`.

### Code Structure & Modularity
- **Never create a file longer than 500 lines of code.** if a file approaches this limit, refactor by splitting it into modules or helper files.
- **Organize code into clearly separated modules**, grouped by feature or responsibility.
- **Use clear, consisten imports** (prefer relative imports within packages).

### Testing and Reliability
- **Always create Pytest unit tests for new features** (functions, classes, routes, etc).
- **After updating any logic**, check whether existing unit tests need to be updated.  If so, do it.
- **Tests should live in a `/tests` folder** mirroring the main app structure.
  - Include at least:
    - 1 test for expected use
    - 1 edge case
    - 1 failure case

### Task Completion
- **Mark completed tasks in  `TASK.md`** immediately after finishing them.
- Add new sub-tasks or TODOs disocverd during development to `TASK.md` under a `Discovered During Work` section.

### Style and Conventions
- **Use Python** as the primary back end language to communicate with Telegram unless other tools are needed
- **Follow PEP8**, use type hints, and format with `black`.
- **Use `pydantic` for data validation**.

### Documentation & Explainability
- **Update `README.md`** when new features are added, dependencies change, or setup steps are modified.
- **Comment non-obvious code** and ensure everything is understandable to a mid-level developer.
- When writing complex logic, **add an inline `# Reason:` comment** explaining the why, not just the what.

### AI Behavior Rules
- **Never assume missing context. Ask questions if uncertain.**
- **Never hallucinate libraries or functions** – only use known, verified Python packages.
- **Always confirm file paths and module names** exist before referencing them in code or tests.
- **Never delete or overwrite existing code** unless explicitly instructed to or if part of a task from `TASK.md`.
