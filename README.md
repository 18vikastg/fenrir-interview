


# 💻🔥 VS Code Reinvented with Built-in Wingman AI — Native AI-Powered IDE Experience

What if your IDE didn't *just* support AI — what if it was **built with it**?

This project is a **native integration of [Wingman AI](https://github.com/RussellCanfield/wingman-ai)** (an open-source coding assistant) directly into the heart of **[Visual Studio Code](https://github.com/microsoft/vscode)** (also open-source) — creating a **custom VS Code build** where **AI is part of the editor**, not an afterthought.

> ⚡️ Forget extensions. This is AI as a **core IDE feature** — seamless, invisible, and always-on.

---

## ✨ Key Highlights

✅ Wingman AI is **baked in** — no user install, no uninstall, no UI clutter  
✅ Works **offline or with APIs** (OpenAI, Ollama, Anthropic, Azure, etc.)  
✅ Preserves all core VS Code functionality  
✅ Works like magic on first launch (portable binary, cross-platform)  
✅ Built from 100% open-source code (MIT-licensed)  
✅ Plug-and-play for developers building **AI-native IDEs, agents, or distros**  

---

## 🌍 Why This Matters

VS Code is the most popular IDE in the world.  
Wingman AI is one of the most powerful open-source coding copilots.

Together, this project shows how the **next generation of developer tools** could look — where **AI is not an addon**, but a **core system-level capability** of your IDE.

> 🔧 Built by developers, for developers — to inspire forks, experiments, and future AI-native tooling.

---

## 📦 Tech Stack & Open Source Attribution

This project proudly builds upon:

- [Visual Studio Code](https://github.com/microsoft/vscode) (MIT License)
- [Wingman AI Extension](https://github.com/RussellCanfield/wingman-ai) (MIT License)
- [Ollama](https://ollama.com/) / [OpenAI](https://platform.openai.com/) / [Anthropic](https://www.anthropic.com/) SDKs
- Custom build, packaging & shell scripting (Linux/Unix-first)

---

## 🛠 How to Build It Yourself (Developers Welcome!)

```bash
# Clone the VS Code source
git clone https://github.com/microsoft/vscode.git
cd vscode
yarn install

# Add Wingman as a built-in extension
cd extensions
git clone https://github.com/RussellCanfield/wingman-ai.git
cd wingman-ai
pnpm install && pnpm compile

# Back to root, patch product.json
nano product.json
# Add Wingman to "builtInExtensions"

# Compile everything
cd ..
yarn gulp compile
yarn gulp vscode-linux-x64-min

# Package it
tar -czvf vscode-custom-linux.tar.gz .build/linux-x64/*
````

✅ On launch: Wingman AI is available instantly
❌ Not visible in Extensions tab
💯 Ready for deep coding with real-time suggestions, doc generation, refactoring, and more

---

## 🎬 Live Demo (Video)

> ⏯ `demo.mkv` includes:

* First launch of custom VS Code
* Wingman’s intelligent composer in action
* Hidden extension status proven

---

## 📁 Repo Structure

```
fenrir-wingman-submission/
├── vscode/                      # VS Code open-source codebase
├── wingman-ai/                  # AI extension source
├── source/                      # Combined custom codebase
├── demo.mkv                     # Screen recording
├── vscode-custom-linux.tar.gz  # Prebuilt binary (tar.gz format)
├── build-instructions.md        # Dev setup guide
├── upgrade-guide.md             # How to sync with upstream
└── README.md                    # This file
```

---

## 🔄 Upgrade Friendly

Want to track future updates?

* Sync VS Code with `git pull upstream master`
* Pull latest Wingman AI releases
* Recompile and repackage

See [`upgrade-guide.md`](./upgrade-guide.md) for full steps.

---

## 🧠 What You Can Do With This

* Build your own **AI-powered IDE** on top of VS Code
* Distribute AI-native portable dev environments
* Build commercial/private forks with full LLM integration
* Replace Copilot with an OSS/LLM provider of your choice

---

## 🧑‍💻 Author

**Vikas T G**
CSE Student | Full-Stack Developer | OSS Enthusiast
🔗 [GitHub](https://github.com/18vikastg) • 📬 [Email](mailto:vikastg2000@gmail.com)

---

## ⭐️ Like It? Fork It. Build With It. Push AI Forward.

---

## 🪪 License

MIT License
(Covers this repo. Dependencies are MIT or permissively licensed.)

---

> 🧬 AI isn't just a feature — it's infrastructure. This is the future of IDEs. Build with it.

```

---




