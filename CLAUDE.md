# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a personal CV/resume repository for Nguyễn Thế Hội. It contains two files that must stay in sync:

- `cv.json` — the canonical source of truth for all CV data (structured data)
- `cv.md` — the rendered Markdown presentation of the CV (derived from `cv.json`)

## Workflow

When updating CV content, always update `cv.json` first, then reflect those changes in `cv.md`. The Markdown file uses a formatted, human-readable layout with emoji section headers and inline code formatting for technology names.

## Data Structure (`cv.json`)

Top-level keys: `personal_info`, `work_experience`, `skills`, `projects`, `education`.

- `skills` has sub-keys: `languages`, `project_management`, `soft_skills`, `tools_and_frameworks`
- Each `projects` entry includes: `name`, `duration`, `team_size`, `description`, `responsibilities[]`, `technologies[]`
