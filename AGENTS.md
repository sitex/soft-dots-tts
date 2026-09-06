<!-- GSD:project-start source:PROJECT.md -->

## Project

**soft-dots-tts**

`soft-dots-tts` is the personal `sitex` fork of dots.tts for local integration work around its autoregressive and flow-matching TTS pipeline. It preserves pretrained inference, streaming, cloning, Gradio, and fine-tuning surfaces while the local project first establishes bounded no-download checks.

**Core Value:** The operator can reproduce the package and CLI readiness boundary without downloading weights or mistaking configuration checks for speech generation.

### Constraints

- **Runtime**: Python below 3.13, PyTorch, audio tooling, and large checkpoints — environment checks must avoid implicit downloads.
- **Hardware**: practical inference requires significant accelerator memory — model-free checks cannot prove runtime performance.
- **Output**: documented 48 kHz audio behavior remains an upstream claim until locally observed.
- **Verification**: no `scripts/verify` exists — Phase 1 must create a deterministic project gate.

<!-- GSD:project-end -->

<!-- GSD:stack-start source:codebase/STACK.md -->

## Technology Stack

- Python 3.10–3.12 package managed by `pyproject.toml` and setuptools.
- PyTorch/torchaudio runtime with optional Gradio, Accelerate and training extras.
- `src/` layout; console entry point `dots.tts = dots_tts.cli:main`.
- Audio output is 48 kHz; model/runtime code uses continuous AudioVAE latents.

<!-- GSD:stack-end -->

<!-- GSD:conventions-start source:CONVENTIONS.md -->

## Conventions

Conventions not yet established. Will populate as patterns emerge during development.
<!-- GSD:conventions-end -->

<!-- GSD:architecture-start source:ARCHITECTURE.md -->

## Architecture

# Architecture

Text enters tokenizer/data preprocessing and the semantic encoder/LLM path. The autoregressive flow-matching head predicts continuous AudioVAE patches, while the speaker encoder supplies x-vector conditioning and the vocoder decodes 48 kHz audio. `DotsTtsRuntime` composes loading and generation; `cli.py` is the command boundary and Gradio wraps the same runtime for a web surface.

Sources: `README.md`, `src/dots_tts/runtime.py`, `src/dots_tts/models`, `src/dots_tts/modules`.
<!-- GSD:architecture-end -->

<!-- GSD:skills-start source:skills/ -->

## Project Skills

No project skills found. Add skills to any of: `.claude/skills/`, `.agents/skills/`, `.cursor/skills/`, `.github/skills/`, or `.codex/skills/` with a `SKILL.md` index file.
<!-- GSD:skills-end -->

<!-- GSD:workflow-start source:GSD defaults -->

## GSD Workflow Enforcement

Before using Edit, Write, or other file-changing tools, start work through a GSD command so planning artifacts and execution context stay in sync.

Use these entry points:

- `$gsd-quick` for small fixes, doc updates, and ad-hoc tasks
- `$gsd-debug` for investigation and bug fixing
- `$gsd-execute-phase` for planned phase work

Do not make direct repo edits outside a GSD workflow unless the user explicitly asks to bypass it.
<!-- GSD:workflow-end -->

<!-- GSD:profile-start -->

## Developer Profile

> Profile not yet configured. Run `$gsd-profile-user` to generate your developer profile.
> This section is managed by `generate-claude-profile` -- do not edit manually.
<!-- GSD:profile-end -->
