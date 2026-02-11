# Video → Code

A single-file HTML tool that converts reference videos + natural language prompts into complete [Remotion](https://remotion.dev) composition code using Claude AI.

## Features

- **Drag & drop videos** — accepts mp4/mov/webm, extracts keyframes as thumbnails
- **Natural language prompts** — describe overlays, music, animations, text in plain English
- **Visual timeline** — markers for each requested element with timestamps
- **AI-powered code generation** — Claude Opus 4.6 generates production-ready Remotion code
- **Format presets** — Vertical (9:16), Landscape (16:9), Square (1:1)
- **Export options** — Copy code, download .tsx, copy as Cursor prompt

## Usage

1. Open `index.html` in a browser (or visit the [GitHub Pages deployment](https://0xmikey-ooze.github.io/video-to-code/))
2. Enter your Anthropic API key (stored in localStorage)
3. Drop in reference video(s)
4. Write a prompt describing what you want
5. Click **Generate** — get complete Remotion code

## Tech

- Single `index.html` file, no build step
- Calls Anthropic API directly from the browser
- Remotion code is output only (needs Node.js + Remotion CLI to render)

## License

MIT
