# GitHub Copilot Custom Instructions

## How should GitHub Copilot behave in this repository?

- Read `plan.md` first when it exists, and treat it as the current source of truth for scope, priorities, and acceptance criteria.
- Check the project brief or task template in `docs/templates/` when requirements or constraints are unclear.
- Keep changes mapped to a single plan item or GitHub issue whenever possible.
- When finishing work, update status, validation notes, and follow-up items in the related issue or pull request.
- Default new project work to Python or R based on the task requirements.
- Use Python for data processing, automation, pipelines, and integrations unless the plan says otherwise.
- Use R for statistics, modeling, visualization, and reporting when it is the better fit.
- When adding dependencies, update the project environment files in the relevant language (`requirements.txt`, `pyproject.toml`, `environment.yml`, `renv.lock`, or similar).
- Keep notebooks and scripts reproducible: document required inputs, outputs, and execution steps in the related task or plan item.
- Follow the established folder structure and naming conventions for the files already in the repository.
- Use existing formatting and linting tools where available.
- Add comments only when needed to explain non-obvious logic.
- Use environment files for secrets and configuration values rather than hardcoding them.
- If a task explicitly targets the existing Next.js starter in `web/`, follow the conventions already used in that application.

## What language style and formatting should Copilot use?

- Prefer Python and R for new project work.
- Use clear, concise variable and function names.
- Follow the formatter/linter that matches the files being edited.
- Add docstrings or inline comments when they help explain non-obvious behavior.

## Example prompts for this repository

- Read `plan.md` and implement the next unchecked task with tests.
- Turn a plan item into a scoped GitHub issue using the task template.
- Add a Python data-cleaning script for the next plan item.
- Create an R analysis script that produces a summary table and chart.
- Turn a notebook workflow into a reproducible Python or R task with validation steps.

---

For more details, see the main [README.md](../README.md).
