# AI Code Assistant Playground

This repository serves as playground and testbed for evaluating and comparing various AI-powered code assistants. 

## Table of Contents

*   [Purpose](#purpose)
*   [Assistants (Front-Ends)](#assistants-front-ends)
*   [Local Model Backends & Setups](#local-model-backends--setups)
*   [Repository Structure](#repository-structure)
*   [Testing Workflow](#testing-workflow)
  
## Purpose

*   Experiment with different AI coding tools (IDE extensions, plugins) hands-on.
*   Evaluate and compare cloud-based assistants (like GitHub Copilot) and assistants capable of using **locally hosted models** (like Continue.dev).
*   Assess the setup, management, and performance of various **local LLM runners** (Ollama, LM Studio, etc.).
*   Compare the quality and relevance of code suggestions from different models (cloud and local).
*   Evaluate features like code completion, generation, refactoring, debugging, and explanation across different setups.
*   Document setup processes, configurations, hardware requirements (for local models), and personal observations.

## Assistants (Front-Ends)

This section lists the primary AI code assistant tools (often IDE extensions or plugins) being evaluated. These are the interfaces used for interacting with the AI, whether the backend is cloud-based or local.

*   ✅ **Continue.dev:** [Website](https://continue.dev/) / [GitHub](https://github.com/continuedev/continue) - *Key tool for easily connecting to various local backends.*
*   ✅ **Windsurf(formerly Codeium):** [Website](https://codeium.com/) - *Primarily cloud-based.*
*   🔄 **GitHub Copilot:** [Website](https://github.com/features/copilot) - *Cloud-based (OpenAI models).*
*   📝 **Tabnine:** [Website](https://www.tabnine.com/) - *Offers both cloud and local (self-hosted) options.*
*   📝 **Amazon Q Developer (CodeWhisperer):** [Website](https://aws.amazon.com/q/developer/) - *Cloud-based (AWS models).*
*   📝 **Cody (Sourcegraph):** [Website](https://sourcegraph.com/cody) - *Cloud-based, context-aware.*
*   📝 **Cursor:** [Website](https://cursor.sh/) - *AI-first IDE (cloud models).*
*   📝 **Pieces for Developers:** [Website](https://pieces.app/) - *Offers local processing options.*
*   *(any other new discovered front-end tools to test)*

**Legend:**
*   ✅ = Actively Testing / Tested
*   🔄 = In Progress / Setting Up
*   📝 = Planned / To Do

## Local Model Backends & Setups
*   **Ollama:** [ollama.com](https://ollama.com/)
*   **LM Studio:** [lmstudio.ai](https://lmstudio.ai/)
*   **GPT4All:** [gpt4all.io](https://gpt4all.io/)
*   **Jan:** [jan.ai](https://jan.ai/)
*   **llama.cpp:** [GitHub](https://github.com/ggerganov/llama.cpp)
*   **aider:** [GitHub](https://github.com/Aider-AI/aider)


**Local Models Tested:**
*   *(specific models locally tested, e.g., `codestral`, `codellama:7b-instruct-gguf`, `starcoder2:3b`, `deepseek-coder:6.7b-base`, `Mistral-7B-Instruct-v0.2.Q5_K_M.gguf`)*

## Repository Structure
```
/
│
├── windsurf/            # Tests and notes for Codeium (Cloud)
│   └── notes.md
│
├── continue_dev/       # Tests and notes for Continue.dev
│   ├── ollama_tests/     # Examples using Ollama backend
│   ├── lm_studio_tests/  # Examples using LM Studio backend
│   ├── config_examples/  # Sample config.json files
│   └── notes.md          # Observations (incl. local backend comparisons)
│
├── github_copilot/     # Tests and notes for GitHub Copilot (Cloud)
│   └── notes.md
│
└── (other_assistant_or_backend_folders...)/
    ├── ...
    └── notes.md
```

## Testing workflow

*   **Setup & Configuration:** Ease of installing assistants and setting up local backends (Ollama, LM Studio, etc.).
*   **Resource Usage:** Monitoring CPU, RAM, and VRAM consumption for local models.
*   **Performance:** Speed and responsiveness of suggestions/chat.
*   **Code Completion:** Quality and relevance of single/multi-line completions.
*   **Code Generation:** Creating functions, classes, tests based on prompts/comments.
*   **Refactoring & Debugging:** Usefulness of suggestions for improving or fixing code.
*   **Chat & Explanation:** Quality of interaction for explaining code or answering questions.
*   **Context Awareness:** How well the assistant uses project context (especially relevant for local models with limited context windows vs tools like Cody/Copilot).
