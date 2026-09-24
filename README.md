### Building AMD ROCm tooling for single-GPU LLM work

Real, working tools and upstream contributions — no mocks, no LoRA, everything
verified on actual gfx942/MI300X hardware before it's called done.

---

**[single-gpu-llm-toolkit](https://github.com/hamstergamerszhang-ops/single-gpu-llm-toolkit)** — ✅ active
Standalone AMD ROCm/PyTorch tools for pruning, expanding, and continued-pretraining
an LLM checkpoint on a single MI300X GPU. Twenty Python + two shell tools covering
the full path from a base checkpoint to a trained one.

**[cuda2rocm](https://github.com/hamstergamerszhang-ops/cuda2rocm)** — ✅ active
CUDA→ROCm compatibility toolkit: shim headers, a cuCollections port, and a cuCascade
port. Verified compiling with 0 errors on real gfx942/ROCm 7.2.1.

**[sirius-rocm](https://github.com/hamstergamerszhang-ops/sirius-rocm)** — 🚧 work in progress
Standalone ROCm/HIP backend for [Sirius](https://github.com/sirius-db/sirius), spun out of
the upstream PR at the maintainer's request. Shim compile-test green in CI; end-to-end
hardware build pending.

**[sirius](https://github.com/hamstergamerszhang-ops/sirius)** (fork) — 🔧 upstream PR open
AMD ROCm/HIP backend for [sirius-db/sirius](https://github.com/sirius-db/sirius), now maintained
standalone in sirius-rocm (above). PR: [sirius-db/sirius#1153](https://github.com/sirius-db/sirius/pull/1153).

**[LMCache](https://github.com/hamstergamerszhang-ops/LMCache)** (fork) — 🔧 upstream PR open
Pipeline-parallelism fix for LMCache's multi-server MP mode.
PR: [LMCache/LMCache#4082](https://github.com/LMCache/LMCache/pull/4082).

---

Status legend: ✅ active/verified · 🔧 in review · 🚧 work in progress
