# Stack

- Python 3.10–3.12 package managed by `pyproject.toml` and setuptools.
- PyTorch/torchaudio runtime with optional Gradio, Accelerate and training extras.
- `src/` layout; console entry point `dots.tts = dots_tts.cli:main`.
- Audio output is 48 kHz; model/runtime code uses continuous AudioVAE latents.

Sources: `pyproject.toml`, `README.md`, `src/dots_tts/runtime.py`.
