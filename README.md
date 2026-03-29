# low-vram-llm

Practical notes, configs, and experiments for running local LLMs on low-end consumer GPUs.

This repository is focused on a simple question:

**How far can you push local LLMs on constrained hardware like a GTX 1660 Super or other low-VRAM GPUs?**

## Why this repo exists

A lot of local AI tooling assumes:
- high-end GPUs
- lots of VRAM
- Linux-first setups
- cloud fallback when things get hard

That is not the reality for many developers.

This repo documents practical local-first LLM setups for people using older consumer hardware, especially on Windows.

## Focus areas

- Running coding-capable local LLMs on low-VRAM GPUs
- Comparing ExLlamaV2 and llama.cpp tradeoffs
- Real-world context/window limitations
- Basic benchmark notes
- Reproducible setup notes instead of theory-heavy guides

## Current hardware tested

- GPU: GTX 1660 Super 6GB
- RAM: 16GB
- OS: Windows

## Goals

- Help people choose realistic models for weak hardware
- Share working setups and limits honestly
- Reduce trial-and-error for local coding assistants
- Explore ways to improve long-context usability on constrained machines

## Early findings

- Small coding models can be usable locally if expectations are realistic
- VRAM is usually the main bottleneck, not raw interest in local AI
- Many guides overstate what older GPUs can do comfortably
- Good documentation for low-end hardware is still underserved

## Repository structure

- `docs/` → setup notes and hardware observations
- `configs/` → example backend-specific configurations
- `scripts/` → benchmark prompts and testing templates
- `results/` → personal test logs and measured behavior

## Intended audience

- Developers with older NVIDIA GPUs
- People experimenting with local coding assistants
- Users trying to avoid cloud/API dependence
- Anyone who wants realistic local AI notes without hype

## Status

Early but active. This repository is being updated as new tests and configurations are validated.

## Contributing

Issues, corrections, and low-VRAM test reports are welcome.
