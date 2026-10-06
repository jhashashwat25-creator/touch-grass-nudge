# Touch Grass Nudge

Pick how long you have, where you are and how you feel. A small open-weight language model running **inside your browser tab** writes you one tiny outdoor mission.

Built for the **Hacktoberfest Open-Source AI Challenge: Week 1 (Touch Grass)** on DEV.

**Live demo:** https://YOUR-USERNAME.github.io/touch-grass-nudge/

## The open-source AI at its core

- **Model:** [Qwen2.5-0.5B-Instruct](https://huggingface.co/Qwen/Qwen2.5-0.5B-Instruct) (ONNX build: [onnx-community/Qwen2.5-0.5B-Instruct](https://huggingface.co/onnx-community/Qwen2.5-0.5B-Instruct)), released under the Apache-2.0 license.
- **Runtime:** [Transformers.js](https://github.com/huggingface/transformers.js) (Apache-2.0), using WebGPU when available and falling back to WebAssembly on CPU.
- **Local inference:** no API key, no backend, no server. Your choices never leave your device.

## Why open innovation matters here

A "go outside" nudge should not need an account or a data plan. Because the model weights are open, the whole app can be one static page that anyone can host for free, read, fork and change.

## Run it locally

```bash
git clone https://github.com/YOUR-USERNAME/touch-grass-nudge.git
cd touch-grass-nudge
python -m http.server 8000
```

Open http://localhost:8000. The first run downloads the model (a few hundred MB). After that your browser caches it.

Works best in recent Chrome or Edge on a laptop or desktop.

## Files

- `index.html`: the whole app (UI and model code)
- `README.md`: this file
- `LICENSE`: MIT

## License

MIT for this project's code. The model and Transformers.js keep their own Apache-2.0 licenses.
