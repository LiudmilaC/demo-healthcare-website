# Riverside Health Center — Static Website

> **Experiment:** This site was built entirely through natural language prompts in Claude Code — Anthropic's AI-powered CLI — without writing a single line of code by hand. The original prompt was:
>
> *"Build a small website about a Healthcare organization for patients. Exactly three HTML pages: `index.html` at the top level, and two more pages each inside its own folder. One `style.css` is fine; no other files."*
>
> From that single prompt, Claude generated the full file structure, all page content, and the complete stylesheet.

A multi-page static website for a fictional medical clinic, built with plain HTML and CSS (no frameworks or build tools required).

## Structure

```
website/
├── index.html          # Home page
├── style.css           # Shared stylesheet
├── services/
│   └── index.html      # Our Services page
└── patients/
    └── index.html      # For Patients page
```

## Pages

- **Home** (`index.html`) — hero banner, about section, and a card grid highlighting the four main service categories.
- **Our Services** (`services/index.html`) — detailed descriptions of primary care, specialty services, and diagnostic offerings.
- **For Patients** (`patients/index.html`) — scheduling instructions, insurance and billing information, health records, and patient resources.

## Design

- Single shared stylesheet (`style.css`) used across all pages via relative paths.
- Color palette centered on teal/navy (`#1a5f7a`, `#0d3d52`) with a light blue background.
- Responsive card grid using CSS Grid (`auto-fill` + `minmax`) — no media queries needed.
- No JavaScript, no external dependencies — open any `.html` file directly in a browser.
