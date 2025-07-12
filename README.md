## 🚀 Community Fork Notice

**This is a community-maintained fork** of Sourcegraph's Cody, created to preserve Cody after its official sunset. This version:

- ✅ **No Sourcegraph login required** - works completely offline
- ✅ **Use your own API keys** - OpenAI, Anthropic, or any compatible provider  
- ✅ **No sunset warnings** - all deprecation messages removed
- ✅ **Enhanced stability** - timeout fixes and improvements

**Mission:** Keep Cody alive and accessible for developers who want to use their own AI API keys.

---

<div align=center>

# <img src="https://storage.googleapis.com/sourcegraph-assets/cody/20230417/logomark-default.svg" width="26"> Cody Community Fork

**AI coding agent with the best codebase understanding - Community maintained**

[\![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

</div>

## Get started

Build and run the VS Code extension locally: `pnpm install && cd vscode && pnpm run dev`

### API Configuration

Configure your API keys in VS Code settings:

**For OpenAI:**
```json
{
  "cody.experimental.openaiCompatible": {
    "provider": "openai", 
    "model": "gpt-4",
    "apiKey": "your-openai-api-key"
  }
}
```

**For Anthropic Claude:**
```json
{
  "cody.experimental.openaiCompatible": {
    "provider": "anthropic",
    "model": "claude-3-sonnet-20240229", 
    "apiKey": "your-anthropic-api-key"
  }
}
```

## What is Cody?

Cody is an open-source AI coding assistant that helps you understand, write, and fix code faster. It uses advanced search to pull context from both local and remote codebases so that you can use context about APIs, symbols, and usage patterns from across your codebase at any scale, all from within your IDE.

## What can Cody do?

- **Chat:** Ask Cody questions about your codebase. Cody will use semantic search to retrieve files from your codebase and use context from those files to answer your questions. You can @-mention files to target specific context.
- **Autocomplete:** Cody makes single-line and multi-line suggestions as you type, speeding up your coding and shortcutting the need for you to hunt down function and variable names as you type.
- **Inline Edit:** Ask Cody to fix or refactor code from anywhere in a file.
- **Prompts:** Cody has quick, customizable prompts for common actions. Simply highlight a code snippet and run a prompt, like "Document code," "Explain code," or "Generate Unit Tests."
- **Swappable LLMs:** Support for Anthropic Claude, OpenAI GPT-4o, Mixtral, Gemini 1.5, and more with your own API keys.

## Contributing

All code in this repository is open source (Apache 2).

Quickstart: `pnpm install && pnpm build && cd vscode && pnpm run dev` to run a local build of the Cody VS Code extension.

### Feedback

- [File an issue](https://github.com/cdinhoo/cody-community-fork/issues) when you encounter problems
- Submit pull requests for improvements
- Share your configurations and tips

## Usage

### Community Fork Usage

This community fork enables you to use Cody with your own API keys without requiring a Sourcegraph account. Simply configure your API keys in the VS Code settings as shown above.

### Supported Providers

- OpenAI (GPT-3.5, GPT-4, GPT-4o)
- Anthropic (Claude 3 Sonnet, Claude 3 Opus)  
- Any OpenAI-compatible API endpoint

## License

This project maintains the same Apache 2.0 license as the original Cody project.

---

**Original Cody Repository:** https://github.com/sourcegraph/cody
EOF < /dev/null