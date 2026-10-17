# SnapDown — releases

Downloads for **SnapDown**, the local-first media studio for macOS. This
repository holds the releases only; the app checks it for updates.

## Download

Get the latest `.dmg` from **[Releases](../../releases/latest)**, open it, and
drag SnapDown into Applications. It's signed with a Developer ID and notarized
by Apple, so it opens like any other app.

Requires macOS 11 or later on Apple Silicon.

## Updates

SnapDown updates itself from here. Each release carries a `.dmg.sig`: an
Ed25519 signature the app checks against a key built into it before it
installs anything, so a release can't be swapped for another build even by
someone who could edit it.

## Open-source software in the app

SnapDown ships these programs unmodified and runs them as separate tools.
Their license texts are inside the app (`SnapDown.app/Contents/Resources/tools`),
and every release here carries the source of the GPL ones that came with it.

| Program | License | Source |
|---|---|---|
| [yt-dlp](https://github.com/yt-dlp/yt-dlp) | Unlicense | [GitHub](https://github.com/yt-dlp/yt-dlp) |
| [gallery-dl](https://github.com/mikf/gallery-dl) | GPL-2.0 | attached to each release, and [GitHub](https://github.com/mikf/gallery-dl) |
| [FFmpeg](https://ffmpeg.org) (ffmpeg, ffprobe), [Martin Riedl's static build](https://ffmpeg.martin-riedl.de) | GPL-3.0-or-later | attached to each release (FFmpeg and the build script), and [ffmpeg.org](https://ffmpeg.org/download.html#releases) |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp), for transcribing on the Mac | MIT | [GitHub](https://github.com/ggml-org/whisper.cpp) |
| [Whisper](https://github.com/openai/whisper) models, downloaded when chosen | MIT | [GitHub](https://github.com/openai/whisper) |
| Python (inside yt-dlp and gallery-dl) | PSF-2.0 | [python.org](https://www.python.org/downloads/source/) |
