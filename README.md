# PlanChat 🚀

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![VS Code Marketplace Version](https://img.shields.io/visual-studio-marketplace/v/YOUR_PUBLISHER.planchat?label=VS%20Marketplace&style=flat-square&color=blue)](https://marketplace.visualstudio.com/items?itemName=YOUR_PUBLISHER.planchat) [![Downloads](https://img.shields.io/visual-studio-marketplace/d/YOUR_PUBLISHER.planchat?style=flat-square)](https://marketplace.visualstudio.com/items?itemName=YOUR_PUBLISHER.planchat) [![Build Status](https://img.shields.io/github/actions/workflow/status/mikl0s/PlanChat/YOUR_CI_WORKFLOW.yml?branch=main&style=flat-square)](https://github.com/mikl0s/PlanChat/actions) <!-- TODO: Update badge URLs after publishing and CI setup -->

**PlanChat is a VS Code extension that revolutionizes project planning by integrating a conversational AI directly into your development environment.** Chat with an LLM to define goals, break down tasks, and generate project plans, all stored in your chosen backend (Supabase or Firebase) for easy access and collaboration.

---

<!-- TODO: Add a compelling GIF or screenshot of PlanChat in action here! -->
<!-- <p align="center">
  <img src="./path/to/your/demo.gif" alt="PlanChat Demo" width="700"/>
</p> -->

## ✨ Key Features

*   💬 **Conversational Planning:** Interact with an LLM through an integrated chat window to brainstorm, define, and refine your project plans.
*   🧠 **Guided Intelligence:** Benefit from guided prompts and iterative questioning designed to extract key project information, even if you're unsure or non-technical.
*   🔧 **Flexible Backend Integration:** Choose your preferred backend! PlanChat supports Supabase and Firebase, allowing you to own your data.
*   📝 **Structured Output:** Automatically generate milestones, tasks, and project vision statements from your conversations.
*   📤 **Versatile Export Options:** Export your plans to Markdown, JSON, or even directly to GitHub Issues.
*   🔑 **OpenAI Powered:** Leverages the power of OpenAI models (bring your own API key).
*   🎨 **Sleek UX/UI:** A clean, minimal, and theme-aware (light/dark) interface, including a split view for chat and structured plan output.
*   💖 **Open Source:** Community-driven and open for contributions!

## 🤔 Why PlanChat?

Traditional project planning tools can be cumbersome, disconnected from the development workflow, or overly complex for many users. PlanChat aims to simplify this by:

*   **Lowering the Barrier:** Making project planning accessible to everyone, regardless of technical expertise, through natural language.
*   **Integrating with Your Workflow:** Plan directly within VS Code, where you already spend your time coding.
*   **Empowering with AI:** Using LLMs to assist in brainstorming, structuring thoughts, and generating actionable plans.
*   **Giving You Control:** Allowing you to use your own backend infrastructure for data storage.

## 🚀 Getting Started

### Prerequisites

*   Visual Studio Code (latest version recommended)
*   An OpenAI API Key
*   A Supabase or Firebase project (if you want to store your plans and conversations)

### Installation

1.  **From VS Code Marketplace (Recommended - once published):**
    *   Open VS Code.
    *   Go to the Extensions view (`Ctrl+Shift+X` or `Cmd+Shift+X`).
    *   Search for "PlanChat".
    *   Click **Install**.
    <!-- TODO: Update this section once published with the correct publisher ID -->

2.  **From GitHub (for latest development version or contributing):**
    *   Clone the repository: `git clone https://github.com/mikl0s/PlanChat.git`
    *   Navigate to the extension directory: `cd PlanChat/planchat` (or just `cd PlanChat` if you cloned into `PlanChat/PlanChat`)
    *   Install dependencies: `npm install`
    *   Open the `planchat` folder in VS Code.
    *   Press `F5` to open a new Extension Development Host window with PlanChat running.

### Initial Configuration

Upon first launch, or via the command palette, PlanChat will guide you to:

1.  **Enter your OpenAI API Key.** This is required for the conversational AI features.
2.  **Configure your Backend (Optional but Recommended):**
    *   Choose between Supabase or Firebase.
    *   Provide the necessary connection details (e.g., Supabase URL & Anon Key, Firebase project config).
    *   This will enable saving your project plans and conversation history.

## 📖 How to Use

1.  Open the PlanChat view from the VS Code Activity Bar (a PlanChat icon will appear).
2.  If you haven't configured it yet, set up your OpenAI API Key and preferred backend.
3.  Start a new project plan by chatting with the AI. For example:
    *   "Let's plan a new mobile app for pet owners."
    *   "I need to outline the features for a new e-commerce website."
4.  The AI will guide you through defining:
    *   Project Vision (Purpose, Audience, Problems Solved)
    *   Key Milestones
    *   Individual Tasks
5.  As you chat, the structured plan (milestones, tasks) will appear in the dedicated view panel, where you can also edit them.
6.  Use commands (accessible via the command palette `Ctrl+Shift+P` or `Cmd+Shift+P` and searching for "PlanChat") to:
    *   Export your plan (Markdown, JSON, GitHub Issues).
    *   Manage settings.
    *   Start new plans or load existing ones (if backend is configured).

## ⚙️ Extension Settings

PlanChat may contribute the following settings to VS Code (accessible via `File > Preferences > Settings` and searching for "PlanChat"):

*   `planchat.openai.apiKey`: Your OpenAI API Key.
*   `planchat.backend.type`: `none`, `supabase`, or `firebase`.
*   `planchat.backend.supabaseUrl`: Your Supabase project URL.
*   `planchat.backend.supabaseAnonKey`: Your Supabase project Anon Key.
*   `planchat.backend.firebaseConfig`: Your Firebase project configuration (JSON string).

*(Note: Specific setting keys might differ; refer to the extension's contribution points in `package.json` or the settings UI for exact names.)*

## 🛠️ Tech Stack

*   **Language:** TypeScript
*   **Frameworks/APIs:**
    *   VS Code Extension API
    *   Node.js
    *   OpenAI API
    *   Supabase SDK / Firebase SDK
*   **Bundler:** esbuild
*   **Linting/Formatting:** ESLint, Prettier
*   **CI/CD:** GitHub Actions (planned)

## 🗺️ Roadmap

We have an exciting future planned for PlanChat! Check out our detailed project plan to see what's coming next:

➡️ **[View Project Plan](./../docs/projectplan.md)**

Key upcoming features include:
*   Full backend abstraction layer for easier addition of new backends.
*   UI polish and enhanced theme support.
*   More robust AI-powered suggestions and plan refinement.
*   (v2.0+) Multi-platform support, voice-to-text, real-time collaboration, and modular LLM support.

## 🤝 Contributing

Contributions are welcome and greatly appreciated! We aim to build a vibrant community around PlanChat.

Please read our [CONTRIBUTING.md](./CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

Ways to contribute:

*   Report bugs and suggest features by opening issues.
*   Improve documentation.
*   Submit pull requests with bug fixes or new features.
*   Help improve prompt quality and planning templates.

## 📜 License

This project is licensed under the MIT License - see the [LICENSE.md](./LICENSE.md) file for details.

## 🙏 Acknowledgements (Optional)

*   Thanks to the VS Code team for the amazing extensibility platform.
*   To all contributors and users who help make PlanChat better!

---

Happy Planning! ✨
