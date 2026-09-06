# Roadmap: soft-dots-tts

## Phases

- [ ] **Phase 1: No-Download Package and CLI Baseline** - Verify package/configuration and CLI boundaries with an explicit skip contract.

## Phase Details

### Phase 1: No-Download Package and CLI Baseline
**Goal:** The operator can reproduce model-free package, configuration, and CLI checks through one deterministic project gate.
**Mode:** mvp
**Depends on:** Nothing (first phase)
**Requirements:** DOTS-01, DOTS-02, DOTS-03
**Success Criteria:**
1. A documented command validates dependency/configuration parsing and package discovery without network or model access.
2. The supported CLI help or invalid-argument path returns a deterministic documented result without loading weights.
3. The repository verification command runs all model-free checks and exits nonzero on a real failure.
4. Model loading, audio generation, cloning, streaming, Gradio, and fine-tuning are visibly reported as skipped.
**Plans:** TBD

## Progress

| Phase | Plans Complete | Status | Completed |
|-------|----------------|--------|-----------|
| 1. No-Download Package and CLI Baseline | 0/TBD | Not started | - |
