# Small tracker for my life / workouts easily editable tsv files with HTML Graphs for weight trends and workout consistency etc

Offline life and workout tracker built around simple TSV source files and static HTML dashboards.

## Files

- `workout_plan.html` - read-only workout program reference.
- `session_log.tsv` - one row per gym, football, or homegym session.
- `set_log.tsv` - working strength sets and skipped strength exercises.
- `health_log.tsv` - daily health, recovery, nutrition, habits, and exercise summaries.
- `progress_dashboard.html` - offline dashboard generated from the TSV logs.
- `conversion_manifest.json` - conversion metadata.

## Notes

The TSV files are the source of truth. The HTML dashboard is derived output and can be opened locally without a server.
