<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.svg">
  <img alt="IxMxAMAR: GPU kernels, ComfyUI nodes, local AI tooling, hypervisors" src="assets/header-light.svg" width="100%">
</picture>

<p align="center">
  <a href="https://github.com/IxMxAMAR">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1200&color=3987E5&center=true&vCenter=true&width=750&lines=AMD+RDNA4+Attention+Kernels+(HIP%2FROCm);Type-1+Hypervisors+in+C+%26+Rust+(UEFI%2FVT-x);ComfyUI+Ecosystem+(68%2B+Production+Nodes);Optimized+RunPod+Cloud+%26+Serverless+Images;Hardware-Aware+Local+AI+Tooling+(Rigma+%26+Raggity)" alt="IxMxAMAR Focus Areas" />
  </a>
</p>

# Hi, I'm IxMxAMAR

I like making generative models run faster, and run on hardware people actually own. That means hand-written attention kernels for AMD's RX 9070 XT, ComfyUI node packs, one-click RunPod images, and tools for running LLMs locally. On the side, I write hypervisors.

---

## 🏆 Flagship Engineering Highlights

<table width="100%">
<tr>
<td width="50%" valign="top">

### 🚀 [SageAttention-RDNA4](https://github.com/IxMxAMAR/SageAttention-RDNA4)
> **Quantized Attention Kernels for AMD RDNA4 (`gfx1201` / RX 9070 & 9070 XT)**

- **Hand-written HIP Attention Kernels**: Custom FP16 and BF16 attention implementations designed specifically for RDNA4 compute units and memory hierarchy.
- **Fused Video Model Workloads**: Handles native fused Q/K/V tensors sent by modern video diffusion architectures (Wan 2.2, HunyuanVideo, LTX-Video).
- **Extreme Speedup**: Up to **2.3× faster** than generic gfx12 ports, matching **0.87–0.94×** execution latency over upstream PR #368 across production batch sizes.
- **Drop-in ComfyUI Integration**: Seamless plug-and-play drop-in for local diffusion inference pipelines without recompilation hurdles.

```
Stack: ROCm / HIP • C++ • PyTorch • RDNA4 gfx1201 • Video Diffusion
```
<p align="right"><a href="https://github.com/IxMxAMAR/SageAttention-RDNA4"><img src="https://img.shields.io/github/stars/IxMxAMAR/SageAttention-RDNA4?style=flat-square&label=%E2%98%85%20Stars" alt="Stars"></a></p>

</td>
<td width="50%" valign="top">

### 🛡️ [Aria](https://github.com/IxMxAMAR/Aria)
> **Type-1 Bare-Metal Hypervisor with In-Place OS Virtualization**

- **UEFI Bootloader Architecture**: Boots directly from UEFI firmware prior to OS initialization, taking full hardware control before Windows boots.
- **In-Place Windows Virtualization**: Dynamically transforms the running Windows kernel into a guest VM without rebooting or disconnecting hardware.
- **Nested VMX Engine**: Full Intel VT-x hardware-assisted virtualization with comprehensive VMCS configuration and nested virtualization support.
- **Advanced EPT & Shadowing**: Extended Page Tables for transparent physical memory virtualization, stealth page hiding, and VMCALL dispatch control.

```
Stack: C • x86_64 ASM • UEFI / EDK2 • Intel VT-x • EPT Paging
```
<p align="right"><a href="https://github.com/IxMxAMAR/Aria"><img src="https://img.shields.io/github/stars/IxMxAMAR/Aria?style=flat-square&label=%E2%98%85%20Stars" alt="Stars"></a></p>

</td>
</tr>
</table>

---

## 🛠️ Technical Stack & Expertise

### 💻 Low-Level Systems & Hypervisors
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![x86_64 ASM](https://img.shields.io/badge/x86__64%20ASM-3572A5?style=flat-square)
![UEFI / EDK2](https://img.shields.io/badge/UEFI%20%2F%20EDK2-00599C?style=flat-square)
![Intel VT-x](https://img.shields.io/badge/Intel%20VT--x-0071C5?style=flat-square&logo=intel&logoColor=white)
![Windows Kernel](https://img.shields.io/badge/Windows%20Kernel-0078D6?style=flat-square&logo=windows&logoColor=white)
![Linux Kernel](https://img.shields.io/badge/Linux%20Kernel-FCC624?style=flat-square&logo=linux&logoColor=black)

### ⚡ AI Acceleration & GPU Compute
![AMD ROCm](https://img.shields.io/badge/AMD%20ROCm-ED1C24?style=flat-square&logo=amd&logoColor=white)
![HIP Kernels](https://img.shields.io/badge/HIP%20Kernels-FF4500?style=flat-square&logo=amd&logoColor=white)
![RDNA4 gfx1201](https://img.shields.io/badge/RDNA4%20(gfx1201)-990000?style=flat-square&logo=amd&logoColor=white)
![NVIDIA CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![SageAttention](https://img.shields.io/badge/SageAttention-3987E5?style=flat-square)
![FlashAttention](https://img.shields.io/badge/FlashAttention-FF6F00?style=flat-square)
![bitsandbytes](https://img.shields.io/badge/bitsandbytes-008080?style=flat-square)
![ComfyUI](https://img.shields.io/badge/ComfyUI-1f2328?style=flat-square)

### ☁️ Cloud & Infrastructure
![RunPod](https://img.shields.io/badge/RunPod-673AB7?style=flat-square&logo=serverless&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Serverless GPUs](https://img.shields.io/badge/Serverless%20Workflows-FD5750?style=flat-square)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

### 🔧 Languages & Applied Tooling
![Python](https://img.shields.io/badge/Python%203.11+-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Vector DBs](https://img.shields.io/badge/Vector%20DBs%20(LanceDB%20%2F%20Qdrant)-DC382D?style=flat-square)
![Claude Agent SDK / MCP](https://img.shields.io/badge/Claude%20MCP%20%2F%20SDK-D97706?style=flat-square&logo=anthropic&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

---

## ⚡ GPU & Performance

| Project | What it is | |
|---|---|---|
| [SageAttention-RDNA4](https://github.com/IxMxAMAR/SageAttention-RDNA4) | SageAttention for the RX 9070 / 9070 XT (`gfx1201`), with hand-written HIP attention kernels for fp16 and bf16. Up to 2.3× faster than generic gfx12 ports, handling fused q/k/v views for video models, and a drop-in for ComfyUI. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/SageAttention-RDNA4?style=flat-square&label=%E2%98%85) |
| [bitsandbytes](https://github.com/IxMxAMAR/bitsandbytes) | Accessible large language models via k-bit quantization for PyTorch with ROCm / AMD GPU acceleration enhancements. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/bitsandbytes?style=flat-square&label=%E2%98%85) |
| [comfyui-mossdype](https://github.com/IxMxAMAR/comfyui-mossdype) | DyPE-M dynamic position extrapolation for MOSS-Image — render past the 4MP training range without retraining. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/comfyui-mossdype?style=flat-square&label=%E2%98%85) |

## 🧩 ComfyUI Node Ecosystem

| Project | What it is | |
|---|---|---|
| [ComfyUI-API-Toolkit](https://github.com/IxMxAMAR/ComfyUI-API-Toolkit) | Kling AI, ElevenLabs, and Google Gemini in one extensible package: 68 production nodes. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-API-Toolkit?style=flat-square&label=%E2%98%85) |
| [ComfyUI-Utility-MegaPack](https://github.com/IxMxAMAR/ComfyUI-Utility-MegaPack) | Comprehensive utility pack featuring 156 operations condensed across 7 nodes, with 11 custom visual graph themes. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-Utility-MegaPack?style=flat-square&label=%E2%98%85) |
| [ComfyUI-IxMxAMAR-Masterworks](https://github.com/IxMxAMAR/ComfyUI-IxMxAMAR-Masterworks) | 12 production-ready masterwork workflow templates orchestrating multimodal generation pipelines end-to-end. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-IxMxAMAR-Masterworks?style=flat-square&label=%E2%98%85) |
| [ComfyUI-NanoBanana2](https://github.com/IxMxAMAR/ComfyUI-NanoBanana2) | Full-parameter Google Gemini API node pack for ComfyUI: text, vision, high-res image generation, audio, music, video, and embeddings. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-NanoBanana2?style=flat-square&label=%E2%98%85) |
| [ComfyUI-NanoBanana-FaceSwap](https://github.com/IxMxAMAR/ComfyUI-NanoBanana-FaceSwap) | Zero-shot face and head replacement powered by Gemini multimodal semantic image editing. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-NanoBanana-FaceSwap?style=flat-square&label=%E2%98%85) |
| [ComfyUI-ElevenLabs-Pro](https://github.com/IxMxAMAR/ComfyUI-ElevenLabs-Pro) | Full-featured ElevenLabs in ComfyUI: voice cloning, low-latency TTS, speech-to-speech, sound effects, and generative music. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-ElevenLabs-Pro?style=flat-square&label=%E2%98%85) |
| [ComfyUI-Kling-Direct](https://github.com/IxMxAMAR/ComfyUI-Kling-Direct) | Native Kling AI API integration for ComfyUI: video, image, and audio generation using your own API key. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-Kling-Direct?style=flat-square&label=%E2%98%85) |

## ☁️ Cloud & RunPod

| Project | What it is | |
|---|---|---|
| [ComfyUI-Ultimate](https://github.com/IxMxAMAR/ComfyUI-Ultimate) | Batteries-included ComfyUI Docker image for RunPod: 29 curated node packs, SageAttention and FlashAttention, pinned dependencies, CI-gated builds. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-Ultimate?style=flat-square&label=%E2%98%85) |
| [ComfyUI-Ultimate-ST](https://github.com/IxMxAMAR/ComfyUI-Ultimate-ST) | All-in-one RunPod image combining ComfyUI-Ultimate generation with SillyTavern AI chat. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-Ultimate-ST?style=flat-square&label=%E2%98%85) |
| [runpod-wan22-serverless](https://github.com/IxMxAMAR/runpod-wan22-serverless) | Serverless Wan 2.2 14B text-to-video and image-to-video worker endpoints for RunPod, with desktop client integration. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/runpod-wan22-serverless?style=flat-square&label=%E2%98%85) |
| [ComfyUI-Serverless-FaceSwap](https://github.com/IxMxAMAR/ComfyUI-Serverless-FaceSwap) | Scalable ComfyUI face-swap workflows served as an on-demand RunPod serverless API. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/ComfyUI-Serverless-FaceSwap?style=flat-square&label=%E2%98%85) |
| [rigma-runpod](https://github.com/IxMxAMAR/rigma-runpod) | Hardware-tuned RunPod pod template, Dockerfile, and container startup spec for instant Rigma LLM deployments. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/rigma-runpod?style=flat-square&label=%E2%98%85) |

## 🖥️ Local AI Tooling

| Project | What it is | |
|---|---|---|
| [rigma](https://github.com/IxMxAMAR/rigma) | Hardware-aware local LLM deployment: `rigma up` probes your GPU and RAM and serves the best-tuned model setup for that exact machine. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/rigma?style=flat-square&label=%E2%98%85) |
| [rigma-registry](https://github.com/IxMxAMAR/rigma-registry) | Community registry of verified, benchmarked model + quant + flag combinations for Rigma hardware-aware deployments. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/rigma-registry?style=flat-square&label=%E2%98%85) |
| [raggity](https://github.com/IxMxAMAR/raggity) | Local-first search and Q&A over notes, docs, and PDFs: hybrid retrieval, cross-encoder reranking, and verified citations powered by Claude Agent SDK (CLI & FastAPI). | ![stars](https://img.shields.io/github/stars/IxMxAMAR/raggity?style=flat-square&label=%E2%98%85) |
| [LoRA-Dataset-Forge](https://github.com/IxMxAMAR/LoRA-Dataset-Forge) | Two photos in, a captioned, aspect-bucketed LoRA training set out, with review step, Gemini face validation, and one-click export. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/LoRA-Dataset-Forge?style=flat-square&label=%E2%98%85) |

## 🛠️ Systems & Hypervisors

| Project | What it is | |
|---|---|---|
| [Aria](https://github.com/IxMxAMAR/Aria) | A Type-1 hypervisor in C that boots through UEFI and virtualizes a running Windows in place, with a full nested VMX engine and EPT paging. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/Aria?style=flat-square&label=%E2%98%85) |
| [Visor](https://github.com/IxMxAMAR/Visor) | Personal hypervisor experiment in Rust: UEFI loader, Windows kernel driver, VMCALL dispatch, and EPT page hiding. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/Visor?style=flat-square&label=%E2%98%85) |
| [barevisor](https://github.com/IxMxAMAR/barevisor) | Personal fork of tandasat's barevisor in Rust with experimental modifications and stealth enhancements. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/barevisor?style=flat-square&label=%E2%98%85) |
| [SimpleVisor](https://github.com/IxMxAMAR/SimpleVisor) | Modified SimpleVisor, ionescu007's minimal Intel VT-x hypervisor in C with custom telemetry and hooks. | ![stars](https://img.shields.io/github/stars/IxMxAMAR/SimpleVisor?style=flat-square&label=%E2%98%85) |

## 🔬 Research & Innovation

| Project | What it is | |
|---|---|---|
| [Research-and-Innovation](https://github.com/IxMxAMAR/Research-and-Innovation) | A living compilation of research papers and ideas organized by domain. First entry: *The x16 Ceiling* (PCIe memory bandwidth and host-to-device streaming saturation). | ![stars](https://img.shields.io/github/stars/IxMxAMAR/Research-and-Innovation?style=flat-square&label=%E2%98%85) |

---

## 🐍 Contribution Activity

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/IxMxAMAR/IxMxAMAR/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/IxMxAMAR/IxMxAMAR/output/github-contribution-grid-snake.svg">
  <img alt="Contribution Snake" src="https://raw.githubusercontent.com/IxMxAMAR/IxMxAMAR/output/github-contribution-grid-snake.svg" width="100%">
</picture>

---

## 📊 Activity & Statistics

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=IxMxAMAR&show_icons=true&hide_rank=true&hide_border=true&disable_animations=true&theme=tokyonight&bg_color=0d1117&title_color=3987e5&icon_color=3987e5&text_color=9198a1">
    <source media="(prefers-color-scheme: light)" srcset="https://github-readme-stats.vercel.app/api?username=IxMxAMAR&show_icons=true&hide_rank=true&hide_border=true&disable_animations=true">
    <img height="175" alt="GitHub Stats" src="https://github-readme-stats.vercel.app/api?username=IxMxAMAR&show_icons=true&hide_rank=true&hide_border=true&disable_animations=true&theme=tokyonight&bg_color=0d1117&title_color=3987e5&icon_color=3987e5&text_color=9198a1">
  </picture>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-streak-stats.herokuapp.com/?user=IxMxAMAR&theme=tokyonight&background=0D1117&border=30363D&stroke=30363D&ring=3987E5&fire=3987E5&currStreakNum=F0F6FC&sideNums=F0F6FC&currStreakLabel=3987E5&sideLabels=9198A1&dates=9198A1&hide_border=true">
    <source media="(prefers-color-scheme: light)" srcset="https://github-readme-streak-stats.herokuapp.com/?user=IxMxAMAR&hide_border=true">
    <img height="175" alt="GitHub Streak" src="https://github-readme-streak-stats.herokuapp.com/?user=IxMxAMAR&theme=tokyonight&background=0D1117&border=30363D&stroke=30363D&ring=3987E5&fire=3987E5&currStreakNum=F0F6FC&sideNums=F0F6FC&currStreakLabel=3987E5&sideLabels=9198A1&dates=9198A1&hide_border=true">
  </picture>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=IxMxAMAR&layout=compact&hide_border=true&disable_animations=true&theme=tokyonight&bg_color=0d1117&title_color=3987e5&text_color=9198a1">
    <source media="(prefers-color-scheme: light)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=IxMxAMAR&layout=compact&hide_border=true&disable_animations=true">
    <img height="175" alt="Top Languages" src="https://github-readme-stats.vercel.app/api/top-langs/?username=IxMxAMAR&layout=compact&hide_border=true&disable_animations=true&theme=tokyonight&bg_color=0d1117&title_color=3987e5&text_color=9198a1">
  </picture>
</p>

---

## 🌐 Connect & Collaborate

<p align="center">
  <a href="https://github.com/IxMxAMAR"><img src="https://img.shields.io/badge/GitHub-IxMxAMAR-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"></a>
  <a href="mailto:officialamrendrasingh@gmail.com"><img src="https://img.shields.io/badge/Email-Get%20in%20Touch-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://huggingface.co/IxMxAMAR"><img src="https://img.shields.io/badge/HuggingFace-IxMxAMAR-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" alt="HuggingFace"></a>
  <a href="https://runpod.io"><img src="https://img.shields.io/badge/RunPod-Cloud%20GPU-673AB7?style=for-the-badge&logo=serverless&logoColor=white" alt="RunPod"></a>
</p>
