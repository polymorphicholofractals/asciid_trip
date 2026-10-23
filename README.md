# ASCIID TRIP — ASCII Motion Encoder

**ARMTEK LABS — turn video into moving character art.**

A Windows desktop app with live ASCII previews, customizable character combinations, original-color or optional monochrome/duotone rendering, and video export up to 3840 pixels wide (4K UHD for 16:9 video).

## Download

Installer downloads will appear under **Releases** after the first testing release is published.

Choose **ASCII-Motion-Encoder-Setup-0.1.1.zip**, extract it, and run the included installer. Alternatively, choose **ASCII-Motion-Encoder-Setup-0.1.1.exe** under the release's **Assets** section. The automatic GitHub “Source code” ZIPs contain this download-page repository, not the application source or installer.

## Requirements

- Windows 10/11, 64-bit.
- FFmpeg and ffprobe installed separately. Python is not needed to run the installed app.

You can install the command-line tools in PowerShell:

```powershell
winget install --id Gyan.FFmpeg --exact
```

Reopen the app after installing FFmpeg.

## Use

1. Open a video or drag one into the app.
2. Choose a character preset or add your own combination. Adjust density and tones while previewing.
3. Press **CONVERT VIDEO**. Choose a new filename and output folder every time.
4. Review the destination and estimated duration, then confirm.
5. Watch the percentage meter; open the converted file or its folder after saving.

Video export supports **MKV, MP4, and MOV**. The original audio is copied without audio effects; some source audio formats need MKV instead of MP4/MOV. AVI export is not currently supported.

## Current status

Early Windows testing release. Short conversion, audio-copy, cancellation, and startup checks have passed in development. Additional testing on other computers and with long movies is ongoing.

This repository hosts downloads and documentation. Application source code is maintained in a separate private repository. Third-party library notices are included with the installed app in `_internal/licenses`.
