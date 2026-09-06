# soft-dots-tts

## What This Is

`soft-dots-tts` is the personal `sitex` fork of dots.tts for local integration work around its autoregressive and flow-matching TTS pipeline. It preserves pretrained inference, streaming, cloning, Gradio, and fine-tuning surfaces while the local project first establishes bounded no-download checks.

## Core Value

The operator can reproduce the package and CLI readiness boundary without downloading weights or mistaking configuration checks for speech generation.

## Requirements

### Validated

- ✓ The `dots_tts` package, CLI, configuration, Gradio demo, streaming, cloning, and fine-tuning surfaces exist — existing code and documentation
- ✓ AudioVAE, language-model backbone, flow-matching head, and speaker-embedding components are represented in source and configuration — existing repository
- ✓ The personal fork publishes portfolio work separately from the vendor `upstream` remote — onboarding

### Active

- [ ] Reproduce environment/configuration parsing and package discovery without downloading or loading model weights.
- [ ] Run the CLI's model-free help or argument-validation boundary with deterministic exit behavior.
- [ ] Add one repository verification command that reports model-backed checks as explicit skips.

### Out of Scope

- Downloading checkpoints during onboarding — asset acquisition remains operator-controlled.
- Claiming generated audio, voice-cloning quality, streaming latency, or fine-tuning behavior without model-backed execution.
- Filling upstream package metadata placeholders outside the verification milestone.

## Context

The fork originates from `studio-dots-ai/dots.tts`. A divergent local commit was preserved through the fork's `portfolio` branch without rewriting upstream history. Source-linked evidence lives in `GSD-BOOTSTRAP.md`, `.planning/codebase/`, and canonical HumanLayer Thoughts.

## Constraints

- **Runtime**: Python below 3.13, PyTorch, audio tooling, and large checkpoints — environment checks must avoid implicit downloads.
- **Hardware**: practical inference requires significant accelerator memory — model-free checks cannot prove runtime performance.
- **Output**: documented 48 kHz audio behavior remains an upstream claim until locally observed.
- **Verification**: no `scripts/verify` exists — Phase 1 must create a deterministic project gate.

## Key Decisions

| Decision | Rationale | Outcome |
|----------|-----------|---------|
| Keep a personal fork and explicit upstream remote | Preserve vendor lineage and local ownership | ✓ Good |
| Start with package/config/CLI boundaries | Produce evidence without unbounded model downloads | — Pending |
| Treat model-backed behaviors as deferred | No compatible model was loaded during onboarding | — Pending |

## Evolution

This document evolves at phase transitions and milestone boundaries.

**After each phase transition**:
1. Move verified requirements to Validated with command evidence.
2. Keep model-backed skips explicit until assets and hardware are available.
3. Record new constraints and decisions.
4. Recheck the maintained-fork description and core value.

**After each milestone**:
1. Review requirement and asset status.
2. Reconfirm the upstream/fork boundary.
3. Define the next evidence-backed milestone.

---
*Last updated: 2026-09-06 after brownfield initialization*
