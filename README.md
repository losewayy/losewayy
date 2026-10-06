### Hi, I'm losewayy

I build small tools and occasionally send patches upstream. Fascinated by all things AI.

#### Merged upstream

| Project | PR |
|---|---|
| [flashinfer](https://github.com/flashinfer-ai/flashinfer) | [#5914](https://github.com/flashinfer-ai/flashinfer/pull/5914) — SM120 DeepSeek-V4 NVFP4 sparse-MLA decode; my runtime page-size work from [#5763](https://github.com/flashinfer-ai/flashinfer/pull/5763) incorporated as the baseline (co-authored in main) |
| [stable-diffusion.cpp](https://github.com/leejet/stable-diffusion.cpp) | [#2047](https://github.com/leejet/stable-diffusion.cpp/pull/2047) — PixArt-α/Σ model family support<br>[#2062](https://github.com/leejet/stable-diffusion.cpp/pull/2062) — unblock Wan2.2 VACE GGUFs: fix 5-dim tensor loading + array metadata parsing<br>[#2074](https://github.com/leejet/stable-diffusion.cpp/pull/2074) — fix f16 overflow in Z-Image quantized matmuls on CUDA<br>[#2103](https://github.com/leejet/stable-diffusion.cpp/pull/2103) — keep MiniMax-H3 VAE weights resident across temporal chunks |
| [exllamav3](https://github.com/turboderp-org/exllamav3) | [#406](https://github.com/turboderp-org/exllamav3/pull/406) — large-page memory for CPU MoE on Windows |

#### In review

- [ncnn#7027](https://github.com/Tencent/ncnn/pull/7027) / [#7026](https://github.com/Tencent/ncnn/pull/7026) — Vulkan Tile operator; skip GPU teardown during Windows process shutdown
- [llama.cpp#29533](https://github.com/ggml-org/llama.cpp/pull/29533) / [#29766](https://github.com/ggml-org/llama.cpp/pull/29766) — Vulkan matmul dispatch split; concurrent first-device init
- [ik_llama.cpp#2594](https://github.com/ikawrakow/ik_llama.cpp/pull/2594) — DeepSeek-V4 in-place RoPE Windows CUDA crash fix
- [onnxruntime#32892](https://github.com/microsoft/onnxruntime/pull/32892) / [#32893](https://github.com/microsoft/onnxruntime/pull/32893) — LayerNorm fusion epsilon fix; MatmulBNFusion graph-output fix
- [onnx#8536](https://github.com/onnx/onnx/pull/8536) — MaxRoiPool reference evaluator
- [flashinfer#6012](https://github.com/flashinfer-ai/flashinfer/pull/6012) — packed FP4 KV support in `BatchAttentionWithAttentionSinkWrapper`

#### Things I've built

- **spawnfate** — predicts Windows process-spawn failures before they happen (argv/PATH/PATHEXT/cmd.exe simulator, MCP-ready)
- **compose-mica** — wallpaper-aware window backdrop for Compose Desktop
- **bililens** — browser extension that turns Bilibili videos into long-form notes
- **flutter_liquid_glasses** — liquid glass material for Flutter
- **uniwill-ec-charge-limit** — battery charge-limit fix for Uniwill laptops
