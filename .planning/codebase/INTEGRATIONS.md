# Integrations

- Hugging Face/local checkpoint loading is the model boundary; no checkpoint is downloaded during onboarding.
- Gradio app is under `apps/gradio`; CLI and Python API are local package surfaces.
- Audio files are read/written through the runtime/audio utilities.
- Upstream reference is `studio-dots-ai/dots.tts`; this repository is the `sitex/soft-dots-tts` vendor mirror.

Sources: `README.md`, `PROJECT_GOAL.md`, `apps/gradio`, `src/dots_tts/cli.py`.
