# Awesome-AI-Audio-Recording-Enhancement

## Top AI Audio Recording & Enhancement Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Noise Suppression, Speech Restoration & Self-Hosted Audio Processing*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **AI Audio Recording & Enhancement**. These tools use machine learning to clean up recordings—removing background noise, echo, and room reverb, restoring clarity to speech, and automating post-production tasks—transforming raw recordings into broadcast-ready audio.



**Examples** include Adobe Podcast, Descript, Riverside.fm, Auphonic, Krisp, and the open-source leaders DeepFilterNet, Resemble Enhance, and ANR (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, avoiding per-minute or per-seat SaaS fees, and controlling the audio processing pipeline. The open-source landscape is anchored by **DeepFilterNet** (the real-time speech enhancement standard with MIT licensing), **Resemble Enhance** (the speech denoising and enhancement toolkit with 1,895+ stars), and **ANR** (the Rust-based noise reduction library with cross-platform GPU backends), with **RNNoise** providing a lightweight, battle-tested alternative.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

| Product | Description | Company Size (Revenue / Valuation) | Pricing | Free Tier Limit |
| :--- | :--- | :--- | :--- | :--- |
| **[Adobe Podcast (Enhance Speech)](https://podcast.adobe.com/)** | AI-powered speech enhancement that removes noise and echo, making recordings sound studio-quality. | **~$21.5B+ ARR / ~$100B–$150B Market Cap** (Public: NASDAQ: ADBE) | Starts at **$19.99/month** (Adobe Firefly Pro / Podcast Premium tier) | **Free plan**: Audio only, one file at a time, up to **30 minutes and 500 MB per file**, **1 hour of enhancement per day**, 2 Studio project downloads per day (up to 30 min each). |
| **[Descript](https://www.descript.com/)** | All-in-one audio/video editor with AI features including Studio Sound, Overdub, and AI clip generation. | **~$55M ARR / $550M Valuation** (Series C funded) | Hobbyist tier starts at **$16/seat/month** (billed annually) or **$19/month** (billed monthly) | **Free plan**: **60 media minutes/month**, **100 one-time AI credits**, 1 seat, 720p watermarked exports. |
| **[Krisp](https://krisp.ai/)** | Real-time AI noise cancellation for calls and meetings, with transcription and AI notes. | **~$38M–$41M ARR / ~$70M–$100M+ Valuation** (Series A-1 funded) | Pro tier starts at **$8/month** (billed annually) or **$16/month** (billed monthly) | **Free plan**: **60 minutes/day** of noise cancellation, unlimited meeting transcriptions, 2 AI note summaries/day, 7-day history. |
| **[Riverside.fm](https://riverside.fm/)** | Remote recording platform with local capture per participant, Magic Audio enhancement, and AI transcription. | **~$35M–$56M ARR / ~$200M–$450M Valuation** (Series C funded) | Pro tier starts at **$24/month** (billed annually) or **$29/month** (billed monthly) | **Free plan**: **2 hours of separate-track recording (one-time trial, not monthly)**, unlimited single-track recording, 720p watermarked exports. |
| **[Auphonic](https://auphonic.com/)** | Automatic audio post-production with loudness normalization, noise reduction, and leveling. | **~$380K–$1M+ ARR** (Bootstrapped / Indie) | Recurring plans start at **$11/month** (for 9 hours/month; 20% discount on yearly billing) | **Free plan**: **2 hours of processed audio per month** (includes Auphonic audio jingle mark). |

## Open-Source GitHub Projects



- **[DeepFilterNet](https://github.com/Rikorose/DeepFilterNet)** [![GitHub Stars](https://img.shields.io/github/stars/Rikorose/DeepFilterNet?style=social&color=white)](https://github.com/Rikorose/DeepFilterNet/stargazers)  

  **The real-time speech enhancement standard.** **MIT licensed**. Uses deep filtering for perceptually motivated noise suppression. **Models**: DeepFilterNet (original) and DeepFilterNet2 (improved). **Usage**: install via `pip install deepfilternet`, then run `deepFilter path/to/noisy_audio.wav` for command-line enhancement, or call `init_df()` and `enhance()` within a Python script . **Strengths**: actively used in production pipelines; supports training on custom datasets; well-documented installation for CPU and CUDA . Best for developers and audio engineers wanting a proven, MIT-licensed enhancement engine that runs locally.



- **[Resemble Enhance](https://github.com/resemble-ai/resemble-enhance)** [![GitHub Stars](https://img.shields.io/github/stars/resemble-ai/resemble-enhance?style=social&color=white)](https://github.com/resemble-ai/resemble-enhance/stargazers)  

  **The speech denoising and enhancement toolkit.** ~1,895 stars, Python-based . Combines denoising (removing background noise) with enhancement (restoring clarity and fullness to speech). **Positioning**: part of Resemble AI's ecosystem, which focuses on voice synthesis and cloning. Best for teams wanting a modern, actively developed alternative to DeepFilterNet with a focus on speech restoration quality.



- **[ANR (Audio Noise Reduction)](https://github.com/lona-cn/anr)** [![GitHub Stars](https://img.shields.io/github/stars/lona-cn/anr?style=social&color=white)](https://github.com/lona-cn/anr/stargazers)  

  **The Rust-based noise reduction library.** Uses the **DFN3** model with **multiple compute backends**: ONNX Runtime (CPU/CUDA/TensorRT/DirectML/CoreML/XNNPACK), native OpenGL/OpenGL ES/Vulkan/wgpu/Direct3D 12 compute shaders—**no ORT required for GPU backends** . **Strengths**: cross-platform (Windows, Linux, macOS, mobile); can run without Python or external shader compilers; SHA-256 model validation . Best for Rust developers and systems engineers wanting to embed noise reduction into applications with minimal dependencies.



### Additional Strong Open-Source Options



- **RNNoise** — Lightweight, real-time noise suppression library based on recurrent neural networks. C-based, extremely fast, and widely embedded in VoIP and conferencing tools. Best for real-time applications where CPU overhead must be minimal.

- **Demucs** — Music source separation (vocals, drums, bass) from Meta. Not speech enhancement per se, but useful for isolating voice tracks from mixed audio before enhancement . Best for podcasters and musicians needing to extract clean vocals.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- **Free tiers are for evaluation, not production**: Adobe Podcast's free plan limits files to **30 minutes and 1 hour/day** ; Descript's free plan is **60 media minutes/month with watermarked exports** ; Riverside's free plan is a **one-off 2-hour allowance, not monthly** .

- **DeepFilterNet is the most mature open-source option**: MIT licensed, actively maintained, and installable via pip. It's the practical default for self-hosted speech enhancement.

- **Real-time vs. file-based processing are different use cases**: Krisp and RNNoise excel at real-time call noise suppression; DeepFilterNet and Resemble Enhance are optimized for file-based post-production enhancement. Choose based on whether you need live filtering or after-the-fact cleanup.

- **SaaS pricing scales with usage**: Riverside's Pro plan includes 5 hours/month of separate-track recording; overages push you to higher tiers . Auphonic charges by processed hours beyond the free 2 hours .



---



**Made for podcasters, video creators, and developers building audio processing pipelines.**  

Let's make AI audio enhancement more open, accessible, and self-hostable.
