# Awesome AI Game Generation [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools, models, research, companies, and resources for generating games with AI — from prompt-to-playable-game platforms to real-time neural world models.

AI game generation spans a wide spectrum: LLM-assisted asset and code scaffolding on one end, and full **world models** that generate playable, interactive worlds frame-by-frame with no traditional game engine at all on the other. This list tracks the whole spectrum — platforms, models, engine integrations, NPC/dialogue systems, asset generators, audio tools, research, and where to learn/discuss it.

## Related Projects

- [MuAPI](https://muapi.ai) — Unified API for image, video, audio, and 3D generation that can complement AI game-asset and world-building workflows.
- [MuAPI model catalog](https://muapi.ai/docs/models) — Browse generative-media models for game art, cinematic clips, and audio.
- [MuAPI playground](https://muapi.ai/playground) — Try image, video, and audio generation models in the browser.

## Contents

- [Related Projects](#related-projects)
- [World Models & Real-Time Generation](#world-models--real-time-generation)
- [Prompt-to-Game Platforms](#prompt-to-game-platforms)
- [AI 2D/3D Asset Generators](#ai-2d3d-asset-generators)
- [AI NPC & Dialogue Systems](#ai-npc--dialogue-systems)
- [AI Audio & Music for Games](#ai-audio--music-for-games)
- [Game Engine AI Integrations](#game-engine-ai-integrations)
- [Level & Content Generation (PCG)](#level--content-generation-pcg)
- [Datasets & Benchmarks](#datasets--benchmarks)
- [Papers & Research](#papers--research)
- [Companies & Labs](#companies--labs)
- [Learning Resources & Communities](#learning-resources--communities)
- [Comparison: Full-Game Generators](#comparison-full-game-generators)
- [Glossary](#glossary)
- [Contributing](#contributing)

## World Models & Real-Time Generation

Systems that generate an interactive, playable world in real time from actions/prompts, rather than assembling a traditional game engine.

- [Genie 3](https://en.wikipedia.org/wiki/Genie_(AI_model)) — Google DeepMind's real-time interactive world model; generates playable 3D worlds frame-by-frame from a prompt, trained on 30,000+ hours of gameplay, with improved memory and resolution over Genie 2.
- [Genie 2](https://en.wikipedia.org/wiki/Genie_(world_model)) — DeepMind's prior-generation model, first to extend interactive world generation from 2D to 3D environments.
- [GameNGen](https://anthemcreation.com/en/artificial-intelligence/gamengen-and-doom-ai-video-games-real-time-generation/) — Google research showing a diffusion model can run DOOM in real time as a neural game engine, with no explicit game logic, engine, or renderer.
- [Oasis](https://github.com/etched-ai/open-oasis) — Open-weights real-time generative Minecraft-like world model; one of the first publicly runnable neural game engines.
- [Matrix-Game](https://arxiv.org/abs/2506.18701) — Interactive world foundation model for controllable, action-conditioned game world generation.
- [HunyuanWorld 1.0](https://github.com/Tencent-Hunyuan/HunyuanWorld-1.0) — Generates immersive, explorable, interactive 3D worlds from text or images.
- [Yan](https://arxiv.org/abs/2508.08601) — Tencent's foundational interactive video generation model for game-like worlds.
- [Mineworld](https://arxiv.org/abs/2504.08388) — Real-time, open-world Minecraft-style interactive world model.
- [LingBot-World](https://github.com/robbyant) — Open-source interactive world model effort (2026).
- [IPR-1 (Interactive Physical Reasoner)](https://arxiv.org/pdf/2511.15407) — World model research focused on physical plausibility in generated interactive environments.

## Prompt-to-Game Platforms

Tools where you describe a game in natural language and get a playable, shippable result.

- [Rosebud AI](https://rosebud.ai/) — The most mature prompt-to-game platform; generates playable 2D/3D games (Phaser-based) with an in-browser chat editor, exportable code, and free hosting. Best for fast arcade/prototype loops.
- [Summer Engine](https://www.summerengine.com/) — In-engine AI agent for Godot 4 that builds the game with you; most generous free tier for a game you can actually ship to Steam.
- [Ludo.ai](https://ludo.ai/) — Ideation/research tool for game designers combining text/image generation with AI-powered market and trend search.
- [the9bit](https://the9bit.com/) — AI game creation platform focused on rapid iterative prototyping.
- [Promethean AI](https://www.prometheanai.com/) — AI co-creator for populating and building 3D game environments through natural-language commands.

## AI 2D/3D Asset Generators

Purpose-built generators for game-ready art, textures, and 3D models (not full games).

- [Meshy](https://www.meshy.ai/) — Covers the most steps of the 3D pipeline in one platform: text/image-to-3D, auto-rigging, and 500+ animation presets.
- [Tripo3D](https://www.tripo3d.ai/) — Fast text/image-to-3D generation (~8s average) with topology auto-optimized for game engines and built-in character rigging.
- [Luma AI / Genie](https://lumalabs.ai/) — Strong at photorealistic environment generation; Luma Genie is a fast, generous free tier for 3D prototyping.
- [Scenario](https://www.scenario.com/) — Game-engine-aware asset generation built specifically for 2D game art and textures.
- [Layer](https://layer.ai/) — AI creative pipeline for 2D game art and consistent style asset generation.

## AI NPC & Dialogue Systems

Engines that give in-game characters LLM-driven conversation, memory, and behavior.

- [Inworld AI](https://inworld.ai/) — Mature Character Engine combining an LLM dialogue core with personality, memory, emotion, and safety layers; direct Unity/Unreal integration.
- [Convai](https://convai.com/) — Optimized for low-latency, real-time in-engine dialogue — built for multiplayer and action games where response speed matters.
- [Charisma.ai](https://charisma.ai/) — Specializes in dialogue-driven, branching narrative storytelling with emotionally adaptive delivery.

## AI Audio & Music for Games

- [ElevenLabs](https://elevenlabs.io/) — AI voice generation commonly used for NPC dialogue and narration in AI-generated games.
- [Suno](https://suno.com/) — AI music generation used for game soundtracks and adaptive audio prototyping.

## Game Engine AI Integrations

- [Unity MCP Plugin](https://github.com/CoplayDev/unity-mcp) — MCP server/editor bridge letting Claude, Cursor, and other MCP-compatible AI agents control the Unity Editor directly (200+ tools).
- Unity Muse — Unity's first-party generative AI toolset for texture, animation, and behavior authoring inside the editor.
- Godot + AI agent workflows — a fast-growing category; see GitHub topic [`ai-game-development`](https://github.com/topics/ai-game-development) for active open-source projects.
- Unreal Engine AI assistants — emerging first- and third-party copilots for Blueprint/C++ scripting and asset placement.

## Level & Content Generation (PCG)

Classic and AI-driven procedural content generation — level layouts, quests, loot, and worlds.

- Procedural Content Generation via Machine Learning (PCGML) — academic umbrella term for using ML models (not hand-authored rules) to generate levels, maps, and content.
- GitHub topic [`procedural-generation`](https://github.com/topics/procedural-generation) — active open-source PCG projects across engines and languages.

## Datasets & Benchmarks

- Gameplay video corpora used to train world models (e.g. the 30,000+ hour internal dataset behind Genie 3) — mostly proprietary; watch for public releases as the field matures.
- Benchmark suites for evaluating interactive world models on action-consistency, memory/persistence, and visual fidelity are still nascent — no standardized public leaderboard yet as of 2026.

## Papers & Research

- Genie 3: A new frontier for world models — Google DeepMind (2025)
- [Generative AI in Game Development: A Qualitative Research Synthesis](https://arxiv.org/html/2509.11898v1) (2025)
- [From Masks to Worlds: A Hitchhiker's Guide to World Models](https://arxiv.org/pdf/2510.20668) (2025)
- [Simulating the Visual World with Artificial Intelligence: A Roadmap](https://arxiv.org/pdf/2511.08585) (2025)
- [Visual Generation in the New Era: An Evolution from Atomic Mapping to Agentic World Modeling](https://arxiv.org/pdf/2604.28185) (2026)
- Generative Games: Positioning, Progress and Prospects — [Preprints.org](https://www.preprints.org/manuscript/202412.1531) (2024)
- IPR-1: Interactive Physical Reasoner — [arXiv](https://arxiv.org/pdf/2511.15407) (2025)

## Companies & Labs

Organizations actively building AI game generation products or foundational models.

- **Google DeepMind** — Genie series, GameNGen research.
- **Rosebud AI** — prompt-to-game consumer platform.
- **Etched** — Oasis open-weights world model.
- **Tencent** — HunyuanWorld, Yan interactive world models.
- **Inworld AI**, **Convai**, **Charisma.ai** — AI NPC/dialogue infrastructure.
- **Meshy**, **Tripo3D**, **Scenario**, **Layer**, **Luma AI** — AI asset generation for game pipelines.

## Learning Resources & Communities

- GitHub topic [`ai-game-development`](https://github.com/topics/ai-game-development) — actively populated, good source for finding new open-source projects as they appear.
- GitHub topic [`game-generator`](https://github.com/topics/game-generator) — projects specifically generating playable games via AI/LLMs.
- GitHub topic [`world-models`](https://github.com/topics/world-models) — research and open implementations of interactive world models.
- [RespawnStack](https://respawnstack.com) — Free reference for pricing, commercial-use terms, and output ownership across 30+ AI game-dev tools (vendor-quoted with source links).

## Comparison: Full-Game Generators

| Platform | Output | Engine | Free tier | Best for |
|---|---|---|---|---|
| Rosebud AI | Playable 2D/3D game, exportable code | Phaser (browser) | Yes, generous | Fast arcade/prototype loops |
| Summer Engine | Shippable game | Godot 4 | Most generous (Steam-ready) | Full, shippable indie games |
| the9bit | Playable prototype | Proprietary | Limited | Rapid iteration |
| Ludo.ai | Design docs, concepts, market research | N/A (ideation, not runtime) | Free tier for ideas | Pre-production ideation |

*Table reflects public info as of mid-2026 — capabilities and pricing change quickly in this space; PRs to correct/update welcome.*

## Glossary

- **World model** — a generative model trained to predict future frames/states of an environment conditioned on actions, effectively acting as a neural game engine.
- **Prompt-to-game** — describing a game concept in natural language and receiving a playable build, as opposed to hand-coding it.
- **PCG / PCGML** — Procedural Content Generation (and its ML-driven variant) for levels, maps, quests, and loot.
- **Action-conditioned generation** — generating the next frame/state of a world based on a player's input action, the core mechanism behind real-time neural game engines.

## Contributing

Contributions welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first. Make sure your addition is genuinely relevant to **AI-driven game generation** — full game generators, world models, and the AI tooling that directly powers them (asset/NPC/audio generation used in AI-built games) — rather than general game development or general game AI (e.g. reinforcement learning agents playing existing games).

## License

[CC0](LICENSE) — public domain.
