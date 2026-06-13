# Second Brain Autonomous Agent Skill (v4.0.0)

A fully autonomous on-device agent for knowledge management based on the PARA methodology (Projects, Areas, Resources, Archives). Optimized for Gemma 4 models (E2B/E4B) and operates 100% offline, ensuring complete privacy of your data.

## Installation (Sideloading) in Google AI Edge Gallery

To install the local version, follow these steps:

1. Install the **Google AI Edge Gallery** application (requires Android 12+ or iOS 17+).
2. Copy the `second-brain` folder (including all subfolders) to the internal storage of your smartphone or tablet.
3. Open the Gallery application and navigate to the **Agent Skills** section.
4. Select the **"Import from local file"** option and specify the path to the copied skill folder.
5. When activating the skill, grant the requested file system permissions (`storage.read`, `storage.write`).

## Architecture

- **SKILL.md** — L1 metadata and role instructions for the LLM.
- **scripts/** — An isolated runtime environment (WebView) for the SQLite WASM database and business logic.
- **assets/** — JSON schemas for tool calling.