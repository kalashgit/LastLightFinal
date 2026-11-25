# Mechanics engineering workflow

## Objective
Turn the supplied mechanics references into original, tested, playable Godot features incrementally. Preserve the existing playable game and the iPhone/Xogot path.

## Before coding
1. Read root AGENTS.md, ROADMAP_CODEX.md, CODEX_V04_V08.md, ASSET_SOURCES.md and docs/mechanics/README.md. Inspect project.godot, main.tscn, relevant scripts and tests.
2. For the assigned feature, identify source documents, exact stated requirements, present code and gaps. Distinguish implemented, partial, missing and unverified features. Check overlapping references together.
3. Explicitly log missing formulas, schemas and contradictions. Do not invent source requirements. For reversible missing implementation details, document proposed defaults separately and test them; request founder decisions for material design changes.
4. Follow the root version sequence and feature-branch mandate. Pick a small runnable vertical slice within the active version; do not attempt the entire library in one change.

## Implementation
- Use original assets, terminology and code; external game references are inspiration, not permission to copy proprietary assets, code, or branding.
- Separate data, simulation, presentation and touch input. Keep configurable balancing values outside unrelated gameplay code.
- Preserve res://main.tscn, offline play, compatible Godot 4 rendering and touch UX. Do not switch to 3D or change orientation merely because a reference mentions a different presentation; record conflicts with the existing project.
- Protect save compatibility, deterministic simulation where applicable, and mobile memory/frame-time. Test interactions with existing systems rather than isolated demos.
- Keep reference files unchanged. Place proposed decisions and implementation tracking in separate docs.

## Verification and handoff
For each slice, report source filenames, requirements addressed, code paths, tests (commands and observed results), save compatibility, remaining limitations, and commit SHA. Run headless import, smoke test and relevant mechanics tests when available. Never claim iPhone validation without actual Xogot testing. Do not merge/deploy without permission. If blocked, leave a runnable baseline and document the blocker.

## Suggested first task
Audit the active version and current implementation against the mechanics library. Produce a traceability table: source, requirement, code path, status, evidence, next slice. Select the smallest missing foundational mechanic consistent with the existing roadmap and implement it end to end with tests. Do not treat the proposed ordering as replacing the existing version sequence.
