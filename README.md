<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
  <img alt="IxMxAMAR: GPU kernels, ComfyUI nodes, local AI tooling, hypervisors" src="assets/banner-light.svg" width="100%">
</picture>

# Hi, I'm IxMxAMAR

I like making generative models run faster, and run on hardware people actually own. That means
hand-written attention kernels for AMD's RX 9070 XT, ComfyUI node packs, one-click RunPod images
and tools for running LLMs locally. On the side I write hypervisors.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![ROCm / HIP](https://img.shields.io/badge/ROCm%20%2F%20HIP-ED1C24?style=flat-square&logo=amd&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![ComfyUI](https://img.shields.io/badge/ComfyUI-1f2328?style=flat-square)

## ⚡ GPU and performance

| Project | What it is | |
|---|---|---|
| [SageAttention-RDNA4](https://github.com/IxMxAMAR/SageAttention-RDNA4) | SageAttention for the RX 9070 / 9070 XT, with hand-written HIP attention kernels for fp16 and bf16. Up to 2.3× faster than the existing gfx12 port, and a drop-in for ComfyUI. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/SageAttention-RDNA4?style=flat-square&label=%E2%98%85) |

## 🧩 ComfyUI nodes

| Project | What it is | |
|---|---|---|
| [ComfyUI-Kling-Direct](https://github.com/IxMxAMAR/ComfyUI-Kling-Direct) | Kling video, image and audio generation inside ComfyUI, with your own API key. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-Kling-Direct?style=flat-square&label=%E2%98%85) |
| [ComfyUI-NanoBanana2](https://github.com/IxMxAMAR/ComfyUI-NanoBanana2) | The full Gemini API as nodes: text, vision, image, audio, music, video and embeddings. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-NanoBanana2?style=flat-square&label=%E2%98%85) |
| [ComfyUI-NanoBanana-FaceSwap](https://github.com/IxMxAMAR/ComfyUI-NanoBanana-FaceSwap) | Face and head replacement through Gemini image editing. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-NanoBanana-FaceSwap?style=flat-square&label=%E2%98%85) |
| [ComfyUI-ElevenLabs-Pro](https://github.com/IxMxAMAR/ComfyUI-ElevenLabs-Pro) | ElevenLabs in ComfyUI: text-to-speech, speech-to-speech, sound effects, music and voice cloning. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-ElevenLabs-Pro?style=flat-square&label=%E2%98%85) |
| [ComfyUI-API-Toolkit](https://github.com/IxMxAMAR/ComfyUI-API-Toolkit) | Kling, ElevenLabs and Gemini in one package: 68 nodes. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-API-Toolkit?style=flat-square&label=%E2%98%85) |
| [ComfyUI-Utility-MegaPack](https://github.com/IxMxAMAR/ComfyUI-Utility-MegaPack) | 156 utility operations in 7 nodes, with 11 visual themes. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-Utility-MegaPack?style=flat-square&label=%E2%98%85) |
| [ComfyUI-IxMxAMAR-Masterworks](https://github.com/IxMxAMAR/ComfyUI-IxMxAMAR-Masterworks) | 12 ready-made workflows that combine the packs above. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-IxMxAMAR-Masterworks?style=flat-square&label=%E2%98%85) |

## ☁️ Cloud and RunPod

| Project | What it is | |
|---|---|---|
| [ComfyUI-Ultimate](https://github.com/IxMxAMAR/ComfyUI-Ultimate) | A batteries-included ComfyUI image for RunPod: 29 curated node packs, SageAttention and FlashAttention, pinned dependencies, CI-gated builds. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-Ultimate?style=flat-square&label=%E2%98%85) |
| [ComfyUI-Ultimate-ST](https://github.com/IxMxAMAR/ComfyUI-Ultimate-ST) | ComfyUI-Ultimate plus SillyTavern in one pod image. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-Ultimate-ST?style=flat-square&label=%E2%98%85) |
| [runpod-wan22-serverless](https://github.com/IxMxAMAR/runpod-wan22-serverless) | Serverless Wan 2.2 14B text-to-video and image-to-video endpoints, with a desktop client. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/runpod-wan22-serverless?style=flat-square&label=%E2%98%85) |
| [ComfyUI-Serverless-FaceSwap](https://github.com/IxMxAMAR/ComfyUI-Serverless-FaceSwap) | ComfyUI face-swap workflows served as a RunPod API. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-Serverless-FaceSwap?style=flat-square&label=%E2%98%85) |

## 🖥️ Local AI tooling

| Project | What it is | |
|---|---|---|
| [rigma](https://github.com/IxMxAMAR/rigma) | Hardware-aware local LLM deployment: `rigma up` probes your GPU and RAM and serves the best-tuned model setup for that exact machine. Community-verified setups live in [rigma-registry](https://github.com/IxMxAMAR/rigma-registry). | ![stars](https://img.shields.io/github/stars/IxMxAMAR/rigma?style=flat-square&label=%E2%98%85) |
| [raggity](https://github.com/IxMxAMAR/raggity) | Local-first search and Q&A over your notes, docs and PDFs: hybrid retrieval, reranking and verified citations, as a CLI or an API. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/raggity?style=flat-square&label=%E2%98%85) |
| [LoRA-Dataset-Forge](https://github.com/IxMxAMAR/LoRA-Dataset-Forge) | Two photos in, a captioned, aspect-bucketed LoRA training set out, with a review step and one-click export. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/LoRA-Dataset-Forge?style=flat-square&label=%E2%98%85) |

## 🛠️ Systems

| Project | What it is | |
|---|---|---|
| [Aria](https://github.com/IxMxAMAR/Aria) | A Type-1 hypervisor in C that boots through UEFI and virtualizes a running Windows in place, with a full nested VMX engine. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/Aria?style=flat-square&label=%E2%98%85) |
| [Visor](https://github.com/IxMxAMAR/Visor) | A hypervisor experiment in Rust: UEFI loader plus Windows driver, VMCALL dispatch and EPT. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/Visor?style=flat-square&label=%E2%98%85) |
| [barevisor](https://github.com/IxMxAMAR/barevisor) | Experiments on top of tandasat's barevisor (Rust). | ![stars](https://img.shields.io/github/stars/IxMxAMAR/barevisor?style=flat-square&label=%E2%98%85) |
| [SimpleVisor](https://github.com/IxMxAMAR/SimpleVisor) | A modified SimpleVisor, ionescu007's minimal Intel VT-x hypervisor (C). | ![stars](https://img.shields.io/github/stars/IxMxAMAR/SimpleVisor?style=flat-square&label=%E2%98%85) |

## 📊 Stats

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=IxMxAMAR&show_icons=true&hide_rank=true&hide_border=true&disable_animations=true&theme=github_dark&bg_color=0d1117">
  <img height="165" alt="GitHub stats" src="https://github-readme-stats.vercel.app/api?username=IxMxAMAR&show_icons=true&hide_rank=true&hide_border=true&disable_animations=true">
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=IxMxAMAR&layout=compact&hide_border=true&disable_animations=true&theme=github_dark&bg_color=0d1117">
  <img height="165" alt="Top languages" src="https://github-readme-stats.vercel.app/api/top-langs/?username=IxMxAMAR&layout=compact&hide_border=true&disable_animations=true">
</picture>
