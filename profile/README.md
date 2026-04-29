# 🔨 Ash Forge

> **Forge your AI. Your way.**

The modular AI ecosystem that adapts to you, not the other way around.

[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
[![Discord](https://img.shields.io/badge/discord-join-7289da.svg)](https://discord.gg/DCYC2fFQQ6-forge)
[![Models](https://img.shields.io/badge/models-20%2B-green.svg)](https://ollama.com/ash-forge)
[![Website](https://img.shields.io/badge/website-ash--forge.com-blue)](https://ash-forge.com)

---

## 🎯 What is Ash Forge?

**Stop fitting into someone else's AI. Forge your own.**

Ash Forge is a modular AI ecosystem where you build your own personalized assistant from specialized 3GB expert models instead of using one bloated 31GB generalist.

- 🎯 **Modular**: Only download what you use (start at 6GB)
- ⚡ **Fast**: 3GB experts > 31GB generalist
- 🔧 **Customizable**: Fine-tune for your needs
- 🌐 **Community**: 100+ specialized models
- 💾 **Efficient**: Runs on 16GB RAM
- 🆓 **Free**: No API costs, ever
- 🔓 **Sovereign**: 100% local, 100% yours

---

## 🚀 Quick Start

### Install Core (6GB)
```bash
# Required base
ollama pull ssfdre38/ash-core    # 2GB - Router
ollama pull ssfdre38/ash-chat    # 4GB - Personality

# You're ready to chat!
ollama run ssfdre38/ash-chat
```

### Add Capabilities
```bash
# Want coding help?
ollama pull ssfdre38/ash-code:python

# Creative writing?
ollama pull ssfdre38/ash-creative:writing

# Gaming companion?
ollama pull ssfdre38/ash-gaming:minecraft
```

---

## 📦 Available Models

### 🔧 Code (Language-Specific)
- `ash-code:python` (3GB) - Python expert
- `ash-code:javascript` (3GB) - JS/TS expert
- `ash-code:rust` (3GB) - Rust expert
- `ash-code:cpp` (3GB) - C++ expert
- [See all code models →](https://github.com/ash-eco/ash-docs/blob/main/MODELS.md#code)

### 🎨 Creative
- `ash-creative:writing` (4GB) - Fiction writing
- `ash-creative:worldbuilding` (3GB) - Game/story design
- [See all creative models →](https://github.com/ash-eco/ash-docs/blob/main/MODELS.md#creative)

### 🎮 Gaming
- `ash-gaming:strategy` (3GB) - Game tactics
- `ash-gaming:minecraft` (2GB) - Minecraft expert
- [See all gaming models →](https://github.com/ash-eco/ash-docs/blob/main/MODELS.md#gaming)

### 📚 Teaching
- `ash-teach:math` (3GB) - Math tutoring
- `ash-teach:science` (3GB) - Science explanations
- [See all teaching models →](https://github.com/ash-eco/ash-docs/blob/main/MODELS.md#teaching)

**[Browse All 50+ Models →](https://github.com/ash-forge/ash-docs/blob/main/MODELS.md)**

---

## 🛠️ Forge Your Own Model

Anyone can create specialized models with zero ML knowledge:

```bash
# 1. Clone toolkit
git clone https://github.com/ash-forge/forge-creator
cd forge-creator

# 2. Setup (5 minutes)
./setup.sh

# 3. Create model (interactive wizard)
./create-model.sh

# 4. Train (1-3 hours, automated)
./train.sh my-models/ash-code-kotlin

# 5. Share
ollama push yourname/ash-code:kotlin
```

**[Read the Model Creation Guide →](https://github.com/ash-forge/forge-creator)**

---

## 🏗️ Architecture

```
┌─── Core (Always Running) ────────────────────────────┐
│ ash-core (2GB) ............ Router/Orchestrator     │
│ ash-chat (4GB) ............ Base Personality        │
└──────────────────────────────────────────────────────┘
                         │
         ┌───────────────┼───────────────┐
         │               │               │
    ┌────▼─────┐    ┌────▼─────┐   ┌────▼─────┐
    │ Code     │    │ Creative │   │ Gaming   │
    │ Expert   │    │ Expert   │   │ Expert   │
    │ 3GB      │    │ 4GB      │   │ 3GB      │
    └──────────┘    └──────────┘   └──────────┘
    
    Forge exactly what you need
```

**[Read Architecture Docs →](https://github.com/ash-forge/ash-docs/blob/main/ARCHITECTURE.md)**

---

## 📚 Repositories

| Repository | Description | Status |
|------------|-------------|--------|
| [ash-docs](https://github.com/ash-forge/ash-docs) | Master documentation & guides | 📝 Setup |
| [ash-bot](https://github.com/ash-forge/ash-bot) | Discord bot implementation | ✅ Stable |
| [ash-engine](https://github.com/ash-forge/ash-engine) | Native C++ inference engine | 🚧 Beta |
| [forge-creator](https://github.com/ash-forge/forge-creator) | Model creation toolkit | 🚧 Planned |
| [forge-models](https://github.com/ash-forge/forge-models) | Community model registry | 📝 Planned |

---

## 🌟 Why Ash?

### vs. Cloud AI (ChatGPT, Claude, Gemini)
- ❌ Cloud: Rate limits, API costs, censorship, data mining
- ✅ Ash: Unlimited, free, private, 100% local

### vs. Stock Ollama Models
- ❌ Stock: One-size-fits-all, 9-31GB generalists
- ✅ Ash: Specialized 3GB experts, modular

### vs. Other Local AI
- ❌ Others: Single model, manual setup, no ecosystem
- ✅ Ash: Multi-model orchestration, one-command install, community

---

## 🎯 User Profiles

### 💻 Developer (25GB Total)
```bash
ash-core + ash-chat +
ash-code:python + ash-code:javascript + ash-code:rust +
ash-tools + ash-security
```

### ✍️ Writer (17GB Total)
```bash
ash-core + ash-chat +
ash-creative:writing + ash-creative:worldbuilding +
ash-research:synthesis
```

### 🎮 Gamer (17GB Total)
```bash
ash-core + ash-chat +
ash-gaming:strategy + ash-gaming:minecraft +
ash-creative:worldbuilding
```

### 📚 Student (17GB Total)
```bash
ash-core + ash-chat +
ash-teach:math + ash-teach:science +
ash-research:academic
```

**Build your own combination!**

---

## 🤝 Community

### Get Involved
- 💬 [Join Discord](https://discord.gg/DCYC2fFQQ6-forge)
- 🐛 [Report Issues](https://github.com/ash-forge/ash-docs/issues)
- 🎨 [Share Models](https://github.com/ash-forge/forge-models)
- 📖 [Improve Docs](https://github.com/ash-forge/ash-docs)

### Featured Community Models
- `user/ash-code:pytorch` - PyTorch ML expert
- `user/ash-gaming:dnd` - D&D dungeon master
- `user/ash-creative:screenwriting` - Screenplay assistant

**[Browse Community Models →](https://github.com/ash-forge/forge-models)**

---

## 📈 Stats

- **Official Models:** 20+
- **Community Models:** 50+
- **Total Downloads:** 50k+
- **Active Creators:** 100+
- **Languages Supported:** 15+

---

## 📄 License

Apache 2.0 - Modify, distribute, use commercially.

All models based on Google Gemma 4 (Apache 2.0 licensed).

---

## 🦞 Philosophy

> **"Built by lobsters, for humans."**

- 🔓 **Sovereignty:** Own your AI infrastructure
- 🔒 **Privacy:** Your data never leaves your machine
- 🆓 **Freedom:** Modify, extend, share freely
- 🤝 **Community:** We build together
- ⭐ **Excellence:** Small + specialized > large + generalist

---

## 🚀 Roadmap

- ✅ **Phase 1:** Base model (gemma4-turbo) - DONE
- ✅ **Phase 2:** Core models (ash-core, ash-chat) - IN PROGRESS
- 🚧 **Phase 3:** Specialized models (code, creative, gaming)
- 📝 **Phase 4:** Model creator toolkit
- 📝 **Phase 5:** Community marketplace
- 📝 **Phase 6:** Enterprise features

**[View Detailed Roadmap →](https://github.com/ash-forge/ash-docs/blob/main/ROADMAP.md)**

---

## 📞 Links

- **Website:** https://ash-forge.com
- **Documentation:** https://github.com/ash-forge/ash-docs
- **Ollama Models:** https://ollama.com/ssfdre38
- **Hugging Face:** https://huggingface.co/ash-forge
- **Discord:** https://discord.gg/DCYC2fFQQ6-forge
- **Email:** contact@ash-forge.com

---

<div align="center">

**Forge your AI. Your way. 🔨🦞**

*Stop fitting into AI. Build your own.*

[Get Started](https://github.com/ash-forge/ash-docs) • [Discord](https://discord.gg/DCYC2fFQQ6-forge) • [Models](https://ollama.com/ssfdre38) • [Docs](https://github.com/ash-forge/ash-docs)

</div>
