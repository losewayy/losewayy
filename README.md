### Hi, I'm losewayy

I build small tools and occasionally send patches upstream. Fascinated by all things AI.

#### Merged upstream

| Project | PR |
|---|---|
| [llama.cpp](https://github.com/ggml-org/llama.cpp) | [#29533](https://github.com/ggml-org/llama.cpp/pull/29533) — split Vulkan matmul dispatch when it would exceed maxComputeWorkGroupCount<br>[#29766](https://github.com/ggml-org/llama.cpp/pull/29766) — serialise concurrent Vulkan first-device init so a second thread cannot use a half-built device |
| [flashinfer](https://github.com/flashinfer-ai/flashinfer) | [#5914](https://github.com/flashinfer-ai/flashinfer/pull/5914) — SM120 DeepSeek-V4 NVFP4 sparse-MLA decode; my runtime page-size work from [#5763](https://github.com/flashinfer-ai/flashinfer/pull/5763) incorporated as the baseline (co-authored in main)<br>[#6139](https://github.com/flashinfer-ai/flashinfer/pull/6139) — keep CuTe-DSL MoE autotune cache keys rank-invariant |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) | [#4569](https://github.com/kvcache-ai/Mooncake/pull/4569) — pin BatchDesc across completion callbacks before freeBatchID to fix TransferEngine UAF<br>[#4839](https://github.com/kvcache-ai/Mooncake/pull/4839) — restore caller CUDA context after plugin copies |
| [ktransformers](https://github.com/kvcache-ai/ktransformers) | [#2243](https://github.com/kvcache-ai/ktransformers/pull/2243) — AVX2 RAWINT4 routed-expert LoRA SFT backend (non-AMX x86 tier); swiglu_limit plumbing fix |
| [stable-diffusion.cpp](https://github.com/leejet/stable-diffusion.cpp) | [#2047](https://github.com/leejet/stable-diffusion.cpp/pull/2047) — PixArt-α/Σ model family support<br>[#2062](https://github.com/leejet/stable-diffusion.cpp/pull/2062) — unblock Wan2.2 VACE GGUFs: fix 5-dim tensor loading + array metadata parsing<br>[#2074](https://github.com/leejet/stable-diffusion.cpp/pull/2074) — fix f16 overflow in Z-Image quantized matmuls on CUDA<br>[#2103](https://github.com/leejet/stable-diffusion.cpp/pull/2103) — keep MiniMax-H3 VAE weights resident across temporal chunks<br>[#2120](https://github.com/leejet/stable-diffusion.cpp/pull/2120) — halve VAE decode tiles on OOM retry instead of jumping to 256px<br>[#2119](https://github.com/leejet/stable-diffusion.cpp/pull/2119) — demote resident params to disk residency when memory reclamation fails<br>[#2124](https://github.com/leejet/stable-diffusion.cpp/pull/2124) — reclaim before accepting wrapped Vulkan iGPU memory estimates<br>[#2167](https://github.com/leejet/stable-diffusion.cpp/pull/2167) — fix `/v1/images/edits` routing for reference-conditioned models<br>[#2164](https://github.com/leejet/stable-diffusion.cpp/pull/2164) — add ADetailer support to server image generation<br>[#2196](https://github.com/leejet/stable-diffusion.cpp/pull/2196) — allow grouped temporal decoding for Wan2.2 TI2V 5B<br>[#2197](https://github.com/leejet/stable-diffusion.cpp/pull/2197) — balance singleton tails in short Wan decode plans |
| [exllamav3](https://github.com/turboderp-org/exllamav3) | [#406](https://github.com/turboderp-org/exllamav3/pull/406) — large-page memory for CPU MoE on Windows<br>[#521](https://github.com/turboderp-org/exllamav3/pull/521) — fix disk cache model load on Windows (os.statvfs is POSIX-only) |
| [ncnn](https://github.com/Tencent/ncnn) | [#7027](https://github.com/Tencent/ncnn/pull/7027) — Vulkan implementation of the Tile operator |
| [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) | [#3985](https://github.com/k2-fsa/sherpa-onnx/pull/3985) — forward provider config keys to the CUDA execution provider |
| [mimalloc](https://github.com/microsoft/mimalloc) | [#1432](https://github.com/microsoft/mimalloc/pull/1432) — pprof allocation failure handling and backtrace re-entrancy |
| [auto-round](https://github.com/intel/auto-round) | [#2456](https://github.com/intel/auto-round/pull/2456) — keep layers the AWQ GEMM kernel cannot serve in fp16 during AWQ export |

#### Approved, pending merge

- [ncnn#7026](https://github.com/Tencent/ncnn/pull/7026) — skip GPU instance teardown at Windows process shutdown
- [Mooncake#4840](https://github.com/kvcache-ai/Mooncake/pull/4840) — distinguish CUDA pointer errors from host memory errors

#### Things I've built

- **spawnfate** — predicts Windows process-spawn failures before they happen (argv/PATH/PATHEXT/cmd.exe simulator, MCP-ready)
- **compose-mica** — wallpaper-aware window backdrop for Compose Desktop
- **bililens** — browser extension that turns Bilibili videos into long-form notes
- **flutter_liquid_glasses** — liquid glass material for Flutter
- **uniwill-ec-charge-limit** — battery charge-limit fix for Uniwill laptops
