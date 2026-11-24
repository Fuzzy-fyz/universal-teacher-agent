# Changelog

Notable project changes are recorded here in reverse chronological order.

## 2026-11-24

### Improved

- Expanded the agent from a general-purpose tutor into an adaptive teaching system that first considers each learner's goals, prior experience, constraints, and feedback.
- Added an evidence-based five-level mastery scale, multidimensional progress checks, and a practical error-analysis loop.
- Added flexible teaching modes, learner-centered plans, spaced-review recommendations, and conversational shortcuts for common study tasks.
- Added workspace-local study memory in `study/` for learner goals, plans, progress, session history, recurring errors, and review topics.
- Clarified memory boundaries: records are not shared across workspaces, must remain in the learner's workspace, and are not a guarantee of perfect recall or scheduled reminders.
- Added a source hierarchy and verification protocol: prioritize learner/course materials and authoritative sources, cite only material actually checked, distinguish verified evidence from model knowledge, and disclose when browsing is unavailable.
- Added optional `study/SOURCES.md` tracking for reusable references with their last-checked dates.
- Updated the README to describe the expanded learning workflow and its boundaries.
