### Hi, I'm losewayy

I build small tools and occasionally send patches upstream.

#### Merged upstream

| Project | PR |
|---|---|
| [flashinfer](https://github.com/flashinfer-ai/flashinfer) | [#5914](https://github.com/flashinfer-ai/flashinfer/pull/5914) — SM120 DeepSeek-V4 NVFP4 sparse-MLA decode; my runtime page-size work from [#5763](https://github.com/flashinfer-ai/flashinfer/pull/5763) incorporated as the baseline (co-authored in main) |
| [stable-diffusion.cpp](https://github.com/leejet/stable-diffusion.cpp) | [#2047](https://github.com/leejet/stable-diffusion.cpp/pull/2047) — PixArt-α/Σ model family support |
| [stable-diffusion.cpp](https://github.com/leejet/stable-diffusion.cpp) | [#2062](https://github.com/leejet/stable-diffusion.cpp/pull/2062) — unblock Wan2.2 VACE GGUFs: fix 5-dim tensor loading + array metadata parsing |
| [exllamav3](https://github.com/turboderp-org/exllamav3) | [#406](https://github.com/turboderp-org/exllamav3/pull/406) — large-page memory for CPU MoE on Windows |

#### In review

- [flashinfer#6012](https://github.com/flashinfer-ai/flashinfer/pull/6012) — packed FP4 KV support in `BatchAttentionWithAttentionSinkWrapper`
- [llama.cpp#29533](https://github.com/ggml-org/llama.cpp/pull/29533) / [#29766](https://github.com/ggml-org/llama.cpp/pull/29766) — Vulkan matmul dispatch split; concurrent first-device init
- [onnxruntime#32892](https://github.com/microsoft/onnxruntime/pull/32892) / [#32893](https://github.com/microsoft/onnxruntime/pull/32893) — LayerNorm fusion epsilon fix; MatmulBNFusion graph-output fix

#### Things I've built

- **spawnfate** — predicts Windows process-spawn failures before they happen (argv/PATH/PATHEXT/cmd.exe simulator, MCP-ready)
- **compose-mica** — wallpaper-aware window backdrop for Compose Desktop
- **bililens** — browser extension that turns Bilibili videos into long-form notes
- **flutter_liquid_glasses** — liquid glass material for Flutter
- **uniwill-ec-charge-limit** — battery charge-limit fix for Uniwill laptops
