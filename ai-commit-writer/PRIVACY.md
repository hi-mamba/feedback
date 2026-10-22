# AI Commit Writer — Privacy Policy

_Last updated: 2026-10-10_

AI Commit Writer ("the plugin") is a JetBrains IDE plugin that generates git
commit messages with an AI model **you** configure. This policy explains what
data the plugin handles.

## Summary

- The plugin has **no server of its own** and the author receives **no data**.
- No telemetry, analytics, tracking, or advertising.
- Data leaves your machine **only** when you explicitly trigger generation (or
  click "Test Connection"), and **only** to the AI endpoint you configured.

## Data sent to your configured AI endpoint

When you trigger "Generate Commit Message", the plugin sends to the API base
URL you entered in *Settings | Tools | AI Commit Writer*:

- the diff of the changes you selected in the commit window (truncated to the
  "max diff chars" setting), including the list of changed file paths;
- up to 5 recent commit subjects from the repository (to match your style);
- the prompt text, chosen model name, and language setting.

"Test Connection" sends a minimal test request to the same endpoint.

That endpoint is operated by the provider **you** chose (e.g. OpenAI, DeepSeek,
a self-hosted server, or a local Ollama instance). How it processes the data is
governed by **that provider's** privacy policy and terms, not this one. If you
use a local model, no data leaves your machine.

## Data stored locally

- **Settings** (endpoint URL, model, language, limits) are stored in the IDE's
  standard configuration directory on your computer.
- **API key** is stored in the IDE's PasswordSafe (the OS keychain / credential
  store), never in plain-text config files. Error messages redact the key.

Nothing is shared with the plugin author or any third party other than the
endpoint you configured.

## Removing your data

Uninstalling the plugin stops all processing. To remove stored data, clear the
API key in the plugin settings (or your OS credential manager) and delete the
plugin's settings file from the IDE configuration directory.

## Contact

Questions: open an issue at https://github.com/hi-mamba/feedback/issues
