# Audiobook Studio

A phone-first, 100% client-side web app for turning audio into finished audiobook videos — no server, no uploads of your files anywhere except the AI APIs you choose with your own keys.

**Live app:** https://ubaaye.github.io/audiobook-studio/

## Features

- **Audio** — upload MP3 / MP4 / M4A / WAV and more, waveform player with click-to-seek
- **Cover** — upload your own, or generate one with AI: a free no-key route, or Gemini with your own API key
- **Typography & backgrounds** — title / subtitle / author / episode text, 5 animated gradient backgrounds, or your own looping video
- **Live 16:9 preview** and a **YouTube Thumbnail Studio** (1920×1080, 6 layouts, PNG download)
- **Video export** — real-time export, plus fast WebCodecs export for gradient backgrounds
- **Narration** — text-to-speech in-app:
  - Gemini TTS with up to 3 of your own keys (automatic failover when a key hits its daily quota)
  - Edge TTS (Thiha / Nilar) — free, via a signed-in account
- **Audio shrinker** — compress long audio files (segmented processing for very long MP4/M4A files) down to Telegram-friendly sizes, MP3 or WebM output
- **Foreign audio → Burmese converter** — transcribe a foreign-language audio file (Whisper), translate it into natural spoken Burmese, review/edit the text, then narrate it
- **Project library** — projects are saved locally in your browser (IndexedDB)

## Notes

- Everything runs in the browser; projects and API keys never leave your device except to the providers you call.
- Gemini free-tier keys have small daily quotas (and no image-generation quota) — the app rotates across up to three keys automatically and offers a free route for covers.
