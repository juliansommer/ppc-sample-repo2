# Task Manager CI/CD Case Study

A Python task manager (`todo.py`) with unit tests (`todo-test.py`), packaged in Docker and run by GitHub Actions on every push to `main`.

The container runs both scripts, writes their output into `index.html` and commits it back to the repository.

Merging a pull request whose description contains `Closes #<issue>` moves the linked issue to **Done** on the project board via `tracker.yml`.

## Setup

Create a classic personal access token with the `repo` and `project` scopes and save it as a repository secret named `PROJECT_TOKEN`.
