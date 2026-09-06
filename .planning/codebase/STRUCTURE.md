# Structure

- `src/dots_tts/config`: app, base, data and training configuration.
- `src/dots_tts/data`: adapters, streaming, batching, collation and tokenizing pipelines.
- `src/dots_tts/models/dots_tts`: model configuration/core/model.
- `src/dots_tts/modules`: backbone, speaker encoder and vocoder components.
- `src/dots_tts/runtime*.py`: normal and double-streaming runtime surfaces.
- `apps/gradio`: demo application; `scripts`: training and manifest helpers; `configs`: smoke training configuration.

Sources: repository tree and `README.md`.
