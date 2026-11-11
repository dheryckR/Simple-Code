# Simple-Code
# Simple Code

> **An AI-powered coding agent that compiles applications into distributable formats, reverse engineers existing binaries, and imports agents, APIs, and code into your project — all from one tool, in plain language or from the command line.**

**Simple Code** bridges the gap between natural language intent and low-level execution. Whether you are packaging an app for release, inspecting compiled binaries, or bootstrapping integrations into an existing codebase, Simple Code handles the heavy lifting through a unified CLI and conversational interface.

---

## ✨ Key Features

* **📦 One-Step Compilation & Packaging:** Automatically build and bundle your source code into ready-to-distribute formats (executables, containers, installers, or packages) without wrestling with complex build scripts.
* **🔍 AI-Assisted Reverse Engineering:** Analyze, decompile, and inspect existing binaries to understand program behavior, recover logic, or audit dependencies using plain language queries.
* **🔌 Seamless Asset & Code Importing:** Pull external AI agents, third-party APIs, SDKs, and reusable code snippets directly into your project structure with automatic wiring and dependency resolution.
* **💬 Dual Interface (Plain Language & CLI):** Interact conversationally for complex, multi-step workflows, or execute fast, scriptable commands directly from your terminal and CI/CD pipelines.

---

## 🚀 Quick Start

### Prerequisites
* [Node.js](https://nodejs.org) v18+ or [Python](https://python.org) 3.10+ *(adjust based on your stack)*
* An API key for your preferred LLM provider (e.g., OpenAI, Anthropic, or local models via Ollama)

### Installation

```bash
# Install globally via npm (or pip/cargo/brew)
npm install -g simple-code
```

### Configuration

Set your AI provider credentials in your environment:

```bash
export SIMPLE_CODE_API_KEY="your-api-key-here"
```

---

## 💻 Usage Examples

### Interactive Mode (Plain Language)
Launch the interactive agent inside any project directory:

```bash
simple-code
```

Then simply type what you need:
> *"Compile this project into a standalone Windows and Linux executable."*
> *"Reverse engineer `./bin/legacy-service` and document its network endpoints."*
> *"Import the Stripe API and set up a webhook handler in `src/routes`."*

### Command Line Mode (Direct Execution)
Run specific tasks directly from your terminal:

```bash
# Compile an application into a distributable format
simple-code compile --target linux-x64,win-x64 --output ./dist

# Reverse engineer an existing binary
simple-code inspect ./path/to/binary --explain

# Import an agent, API, or external module into your current project
simple-code import api:openai --into ./src/services
```

---

## 🛠️ Project Workflow

1. **Context Scan:** Simple Code indexes your project structure, dependencies, and target environment.
2. **Plan & Verify:** For destructive or complex operations (like compilation or file injection), the agent outlines its execution plan before modifying files.
3. **Execute & Validate:** Runs the underlying compilers, disassemblers, or package managers and verifies the output.

---

## 🤝 Contributing

Contributions are what make the open-source community thrive. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.
