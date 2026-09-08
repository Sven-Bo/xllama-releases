# XLlama

Local AI for Microsoft Excel on Windows, powered by Ollama.

**[Download XLlama for Windows](https://github.com/Sven-Bo/xllama-releases/releases/latest/download/XLlama-Setup.exe)**

This repository contains official installers and release notes. Application source code is not published here.

## Install

1. Download `XLlama-Setup.exe` from the link above.
2. Save your work and close Excel.
3. Run setup and follow its instructions. Setup checks the required components and provides download links if any are missing.
4. Open Excel and select **XLlama** in the ribbon. Start Ollama and choose or download a local model in XLlama.

Requires desktop Excel on 64-bit Windows, the matching .NET 10 Windows Desktop Runtime, WebView2, and [Ollama](https://ollama.com/download/windows). Both 32-bit and 64-bit Excel payloads are included; native ARM64 Excel, Mac, and Excel for the web are not supported. Live Excel verification has covered 64-bit Excel.

## Included

- Automatic Ollama connection status and model management.
- Streaming chat, Markdown formatting, saved conversations and compact worksheet attachments.
- `XLLAMA.PROMPT`, `XLLAMA.EXTRACT`, and Pro `XLLAMA.STREAM` formulas.
- Free: **10 chat responses per day** and **5 XLlama formula cells per workbook**. The chat shows your remaining allowance. A request that produces no answer does not use a response; stopping after answer text appears counts once.

Inference runs through local Ollama. Model downloads require internet access. Selected worksheet data can be retained in your saved chats on your computer.

## Release status

**1.0.0 is the first public release. The installer is unsigned**, so Windows or company security policies may block it.

**Paid activation is awaiting a required licensing-server update.** Free mode can be tested now; this release is not yet verified for paid customer rollout. See the release notes for the tested scope.

## Update and uninstall

The download link above stays the same for future releases. Save and close Excel, then run the new installer to update. Saved conversations and settings are preserved.

To uninstall, close Excel and go to **Windows Settings → Apps → Installed apps → XLlama → Uninstall**. Uninstall preserves your local chats, settings and license/usage records, along with Ollama and its models.

The installer checksum is provided as `SHA256SUMS.txt` in each release. A checksum verifies file integrity; it is not a publisher signature.
