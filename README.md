Repository containing all the mnotes and examples for github actions course.This has been edited
# GitHub Actions Course Repository

This repository contains notes and practical examples for learning core GitHub Actions concepts.
Each workflow demonstrates a focused topic so you can run, inspect, and modify it while following the course.

## What you'll find

- **Hands-on workflow examples** in `.github/workflows/`.
- **A sample React application** in `04-using-actions/react-app/` used for workflow-based CI practice.
- **Topic-by-topic progression** from events and runners to expressions, variables, functions, inputs, and outputs.

## Repository structure

```text
.
├── .github/workflows/            # Course workflows
├── 04-using-actions/react-app/   # Demo app used by workflows
└── README.md
```

## Workflow lessons included

| Workflow file | Topic |
|---|---|
| `02-workflows-events.yml` | Triggering workflows with events |
| `03-workflow-runners.yml` | Running jobs on Ubuntu, Windows, and macOS runners |
| `04-using-actions.yml` | Using marketplace actions (`checkout`, `setup-node`) and running tests |
| `05-1-filter-activities-type.yml` | Filtering pull request events by activity type |
| `05-2-filter-activities-type.yml` | Additional pull request activity filtering example |
| `06-Context.yml` | Accessing GitHub and environment context values |
| `07-expressions.yml` | Conditional execution with expressions |
| `08-variables.yml` | Workflow, job, and step-level variables |
| `09-functions.yml` | Built-in functions like `contains`, `toJson`, and status checks |
| `10-execution-flow.yml` | Job execution flow and dependencies |
| `11-inputs.yml` | Workflow dispatch inputs |
| `12-outputs.yml` | Passing data through job outputs |

## Getting started

### Prerequisites

- A GitHub account
- Git installed locally
- (Optional) Node.js 20+ and npm if you want to run the sample app locally

### Clone the repository

```bash
git clone <your-fork-or-repo-url>
cd github-actions-course
```

### Run workflows

1. Push this repository to GitHub (or fork it).
2. Open the **Actions** tab in GitHub.
3. Select any workflow by name.
4. Trigger workflows that use `workflow_dispatch` with **Run workflow**.

## Running the sample React app locally

```bash
cd 04-using-actions/react-app
npm ci
npm start
```

Run tests:

```bash
npm test
```

## Learning tips

- Start with `02-workflows-events.yml` and move upward numerically.
- Open each workflow file and predict the behavior before running it.
- Use workflow logs to understand expressions, contexts, and conditional execution.

## Contributing

If you're using this repo for your own learning, feel free to add more workflow examples and improve existing ones.
