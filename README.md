### Hi, I'm losewayy

I build small tools and occasionally send patches upstream. Fascinated by all things AI.

#### Merged upstream

| Project | PR |
|---|---|
| [flashinfer](https://github.com/flashinfer-ai/flashinfer) | [#5914](https://github.com/flashinfer-ai/flashinfer/pull/5914) — SM120 DeepSeek-V4 NVFP4 sparse-MLA decode; my runtime page-size work from [#5763](https://github.com/flashinfer-ai/flashinfer/pull/5763) incorporated as the baseline (co-authored in main) |
| [ktransformers](https://github.com/kvcache-ai/ktransformers) | [#2243](https://github.com/kvcache-ai/ktransformers/pull/2243) — AVX2 RAWINT4 routed-expert LoRA SFT backend (non-AMX x86 tier); swiglu_limit plumbing fix |
| [stable-diffusion.cpp](https://github.com/leejet/stable-diffusion.cpp) | [#2047](https://github.com/leejet/stable-diffusion.cpp/pull/2047) — PixArt-α/Σ model family support<br>[#2062](https://github.com/leejet/stable-diffusion.cpp/pull/2062) — unblock Wan2.2 VACE GGUFs: fix 5-dim tensor loading + array metadata parsing<br>[#2074](https://github.com/leejet/stable-diffusion.cpp/pull/2074) — fix f16 overflow in Z-Image quantized matmuls on CUDA<br>[#2103](https://github.com/leejet/stable-diffusion.cpp/pull/2103) — keep MiniMax-H3 VAE weights resident across temporal chunks<br>[#2120](https://github.com/leejet/stable-diffusion.cpp/pull/2120) — halve VAE decode tiles on OOM retry instead of jumping to 256px<br>[#2119](https://github.com/leejet/stable-diffusion.cpp/pull/2119) — demote resident params to disk residency when memory reclamation fails |
| [exllamav3](https://github.com/turboderp-org/exllamav3) | [#406](https://github.com/turboderp-org/exllamav3/pull/406) — large-page memory for CPU MoE on Windows |
| [ncnn](https://github.com/Tencent/ncnn) | [#7027](https://github.com/Tencent/ncnn/pull/7027) — Vulkan implementation of the Tile operator |
| [auto-round](https://github.com/intel/auto-round) | [#2456](https://github.com/intel/auto-round/pull/2456) — keep layers the AWQ GEMM kernel cannot serve in fp16 during AWQ export |

#### In review

- [Mooncake#4569](https://github.com/kvcache-ai/Mooncake/pull/4569) — pin BatchDesc across completion callbacks: fix the UAF behind flaky TCP WRITE-ack CI (approved, awaiting merge)
- [ncnn#7026](https://github.com/Tencent/ncnn/pull/7026) / [#7047](https://github.com/Tencent/ncnn/pull/7047) / [#7078](https://github.com/Tencent/ncnn/pull/7078) — skip GPU teardown at shutdown; fold+glu Vulkan ops; faster einsum contractions
- [llama.cpp#29533](https://github.com/ggml-org/llama.cpp/pull/29533) / [#29766](https://github.com/ggml-org/llama.cpp/pull/29766) — Vulkan matmul dispatch split; concurrent first-device init
- [ik_llama.cpp#2594](https://github.com/ikawrakow/ik_llama.cpp/pull/2594) — DeepSeek-V4 in-place RoPE Windows CUDA crash fix
- [onnxruntime#32892](https://github.com/microsoft/onnxruntime/pull/32892) / [#32893](https://github.com/microsoft/onnxruntime/pull/32893) — LayerNorm fusion epsilon fix; MatmulBNFusion graph-output fix
- [onnx#8536](https://github.com/onnx/onnx/pull/8536) / [onnxscript#3055](https://github.com/microsoft/onnxscript/pull/3055) — MaxRoiPool reference evaluator; linalg_solve_triangular converter
- [flashinfer#6012](https://github.com/flashinfer-ai/flashinfer/pull/6012) / [#6139](https://github.com/flashinfer-ai/flashinfer/pull/6139) — packed FP4 KV in BatchAttention; rank-invariant CuTe-DSL MoE autotune keys
- [stable-diffusion.cpp#2124](https://github.com/leejet/stable-diffusion.cpp/pull/2124) — iGPU/UMA Vulkan memory accounting fix
- [sherpa-onnx#3984](https://github.com/k2-fsa/sherpa-onnx/pull/3984) / [#3985](https://github.com/k2-fsa/sherpa-onnx/pull/3985) / [#3986](https://github.com/k2-fsa/sherpa-onnx/pull/3986) — Qwen3-ASR word timestamps; provider config forwarding; Dolphin attention decoder
- [sglang#41391](https://github.com/sgl-project/sglang/pull/41391) — MiniCPMV `__getattr__` chaining fix

#### Things I've built

- **spawnfate** — predicts Windows process-spawn failures before they happen (argv/PATH/PATHEXT/cmd.exe simulator, MCP-ready)
- **compose-mica** — wallpaper-aware window backdrop for Compose Desktop
- **bililens** — browser extension that turns Bilibili videos into long-form notes
- **flutter_liquid_glasses** — liquid glass material for Flutter
- **uniwill-ec-charge-limit** — battery charge-limit fix for Uniwill laptops
