# Small tracker for my life / workouts easily editable tsv files with HTML Graphs for weight trends and workout consistency etc

This is a small public example of how I like to build practical tools: simple source-of-truth files, offline-first HTML, and enough structure to keep the system easy to change.

I am [Arshia Hemati](https://www.arshiahemati.com/), a full-stack developer focused on AI automation, web products, and enterprise-style systems. My larger commercial projects, including Elyt and Synth, are private, but this repo shows the same bias I use in my work: keep the data model clear, avoid unnecessary infrastructure, and make the output useful fast.

## What This Is

An offline life and workout tracker built around editable TSV files and static HTML dashboards.

The goal is not to be a SaaS app. The goal is to keep personal tracking durable, inspectable, and easy to modify without a database, server, login flow, or vendor lock-in.

## Why It Exists

Most personal trackers eventually become hard to customize. This one keeps the important data in plain text TSV files and uses HTML for readable dashboards and graphs.

That makes it easy to:

- edit logs manually
- review workout history
- track bodyweight trends
- check workout consistency
- regenerate or replace dashboards later
- keep the project fully offline

## Files

- `workout_plan.html` - read-only workout program reference.
- `session_log.tsv` - one row per gym, football, or homegym session.
- `set_log.tsv` - working strength sets and skipped strength exercises.
- `health_log.tsv` - daily health, recovery, nutrition, habits, and exercise summaries.
- `progress_dashboard.html` - offline dashboard generated from the TSV logs.
- `conversion_manifest.json` - conversion metadata.

## Design Choices

- TSV files are the source of truth.
- HTML dashboards are derived output.
- No server is required.
- No external assets or CDN are required for the dashboard.
- Data columns stay explicit and machine-readable.
- Free text is kept mostly to notes fields.

## Larger Work

Some of my main projects are private because they are commercial or still in development:

- **Elyt** - AI-powered browser automation with multi-profile orchestration, humanization technology, and multi-provider LLM integration.
- **Synth** - AI agent and workflow management platform built from the experience of Elyt, with service integrations and tenant-isolated agent state.
- **Enterprise systems** - ticketing, reservation, POS, and hardware integrations built for real business workflows.

More context is available on my portfolio: [ArshiaHemati.com](https://www.arshiahemati.com/).

## Contributing

This repository is public so people can read it and fork it.

If you want to change my version, open a pull request. The main branch is protected so changes require review before being merged.
