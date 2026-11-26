# playground

Scratch space for experiments and prototypes built with AndroidHarness.

## What's here

- `.github/workflows/demo.yml` — a small demo GitHub Actions workflow:
  - triggers on push/PR to `main` and manual `workflow_dispatch`
  - matrix build on macOS and Ubuntu
  - writes `dist/report.txt` and uploads it as a per-OS artifact
  - a final summary job reports the matrix result

## Running the demo workflow

1. Push to `main` (or open a pull request) — the workflow runs automatically.
2. Or go to **Actions → Demo workflow → Run workflow** and optionally pass a `greeting`.

## Notes

- Action versions are pinned to `v4`; they currently run on GitHub's Node.js 20 runtime.
- macOS arm64 runners may queue longer under capacity constraints.
