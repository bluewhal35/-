# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project overview

A static, framework-free personal portfolio page for a middle school student — plain HTML/CSS only. No React, Next.js, or other framework is to be introduced.

## Development

There is no build tool, package manager, linter, or test suite in this repository (no `package.json`). To "run" the site, open `index.html` directly in a browser — there is no dev server or build step.

## File structure

- `index.html` — all page structure and content
- `style.css` — all styling (CSS custom properties defined in `:root`, plus a `@media (max-width: 480px)` block for mobile)

## Page structure

`index.html` is a single-page scrolling layout. The sticky header nav links to sections via same-page anchors, matching these section `id`s in order: `#home`, `#about`, `#interests`, `#activities`, `#projects`, `#contact`. When adding a new section, add both the `<section id="...">` and a corresponding nav link.

## Privacy convention

The student's name (김지후) and age (16) are included because the student explicitly asked for them. School name, contact info (email/SNS), and photos remain generic placeholder text (e.g. a CSS-drawn initial avatar instead of a real photo, "담당 선생님을 통해 연락" instead of a real contact method, "중학교 졸업을 앞둔 학생" instead of a specific school name). Preserve this pattern when editing content — don't fill in a real school name, contact details, or photos unless the user explicitly asks to change this convention.
