---
document: gsd-brownfield-bootstrap
project: soft-dots-tts
git_root: /home/rocky/projects/soft-dots-tts
github_repository: sitex/soft-dots-tts
generated_at: 2026-09-06T02:03:45Z
thoughts_status: available
github_status: repository resolved; Issues API unavailable or disabled for this fork
include_personal: false
---

# Purpose

Vendor fork and integration base for dots.tts, a continuous 2B-parameter autoregressive multilingual TTS system with CLI, Python API, Gradio demo, cloning, and training entry point. [T1]

# Implemented Capabilities

- Source package, configuration, data pipelines, model modules, runtime and audio utilities exist. [T2]
- `dots.tts` CLI and `DotsTtsRuntime` API are documented and wired. [T2]
- Gradio app and training/manifest scripts exist. [T2]

# Current Milestone

Active v1: local reproducible CLI/inference smoke baseline without model download. This is an onboarding target, not proof of model inference. [T1]

# Open Requirements

- Validate the no-download CLI/inference boundary smoke. [T1]
- Later validate real checkpoint loading, audio generation, cloning, Gradio startup and fine-tuning separately. [T1]

# Accepted Decisions

- Treat this as a vendor fork and preserve upstream boundary. [T1]
- Do not download models during onboarding. [T1]

# Constraints

- Python 3.10–3.12; PyTorch/torchaudio 2.8+; real inference expects GPU resources. [T1]
- Upstream sync, license changes and publication require human direction. [T1]

# Unresolved Conflicts

None identified from available sources.

# Source Thoughts

- T1: `/home/rocky/thoughts/repos/soft-dots-tts/shared/research/2026-09-06-project-baseline.md`
- T2: `/home/rocky/projects/soft-dots-tts/README.md`, `PROJECT_GOAL.md`, `pyproject.toml`

# Source Issues

None included; the Issues API is unavailable or disabled for this fork.

# Source Limitations

No model download or real inference was performed; no code-verification claim is made.
