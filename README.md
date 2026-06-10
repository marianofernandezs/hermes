# Hermes

Hermes is a local-first, privacy-first desktop app for recording, transcribing, summarizing and organizing work meetings.

The initial target platform is macOS on Apple Silicon.

## Goals

- Record meetings from Zoom, Microsoft Teams, Google Meet and similar apps.
- Capture screen, window, system audio and microphone audio.
- Store recordings locally.
- Transcribe locally using Whisper / whisper.cpp.
- Summarize locally using Ollama-compatible models.
- Export to Markdown, TXT, JSON, SRT, VTT and PDF.
- Avoid mandatory cloud dependencies.
- Provide a serious open source foundation for privacy-preserving meeting notes.

## Status

OpenMinutes is in early architecture and foundation development.

Do not use it yet for sensitive or production meetings.

## Stack

- Desktop: Tauri v2
- Core: Rust
- UI: React, TypeScript, Tailwind
- Local transcription: whisper.cpp
- Local LLM runtime: Ollama
- Storage: SQLite + FTS5
- Initial platform: macOS Apple Silicon

## Repository structure

```text
apps/desktop    Tauri desktop app
crates/         Rust modules
docs/           Product and technical documentation
.github/        GitHub workflows and community filess
