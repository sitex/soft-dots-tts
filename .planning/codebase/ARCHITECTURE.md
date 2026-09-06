# Architecture

Text enters tokenizer/data preprocessing and the semantic encoder/LLM path. The autoregressive flow-matching head predicts continuous AudioVAE patches, while the speaker encoder supplies x-vector conditioning and the vocoder decodes 48 kHz audio. `DotsTtsRuntime` composes loading and generation; `cli.py` is the command boundary and Gradio wraps the same runtime for a web surface.

Sources: `README.md`, `src/dots_tts/runtime.py`, `src/dots_tts/models`, `src/dots_tts/modules`.
