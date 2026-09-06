# Requirements: soft-dots-tts

**Defined:** 2026-09-06
**Core Value:** Reproduce package and CLI readiness without downloading weights or implying speech generation.

## v1 Requirements

### No-Download Baseline

- [ ] **DOTS-01**: Operator can validate dependency/configuration parsing and discover the `dots_tts` package without downloading or loading model weights.
- [ ] **DOTS-02**: Operator can invoke the supported CLI help or invalid-argument path and observe deterministic model-free exit behavior.
- [ ] **DOTS-03**: Operator can run one repository verification command that executes model-free checks and reports model-backed checks as explicit skips.

## v2 Requirements

### Model-Backed Runtime

- **DOTS-04**: Operator can generate a valid 48 kHz audio sample from an approved local model.
- **DOTS-05**: Operator can verify voice cloning, streaming, Gradio, and fine-tuning on compatible hardware.

## Out of Scope

| Feature | Reason |
|---------|--------|
| Automatic model downloads | Asset acquisition is operator-controlled. |
| Generated-audio claims from model-free checks | Configuration readiness does not prove inference. |
| Fine-tuning execution during baseline work | It requires separate datasets, hardware, and acceptance criteria. |

## Traceability

| Requirement | Phase | Status |
|-------------|-------|--------|
| DOTS-01 | Phase 1 | Pending |
| DOTS-02 | Phase 1 | Pending |
| DOTS-03 | Phase 1 | Pending |

**Coverage:** 3 total, 3 mapped, 0 unmapped ✓

---
*Requirements defined: 2026-09-06*
*Last updated: 2026-09-06 after brownfield initialization*
