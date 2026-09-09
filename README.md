# XLlama

Local AI chat and worksheet formulas for Microsoft Excel on Windows, powered by Ollama.

## Downloads

- **[XLlama Windows installer](https://pythonandvba.com/go/excel-xllama-add-in-download)** — recommended for most users.
- **[IT deployment ZIP](https://pythonandvba.com/go/excel-xllama-add-in-it-download)** — compiled add-in files and PowerShell deployment scripts for administrators.
- [Getting started](https://pythonandvba.com/go/excel-xllama-add-in-getting-started)
- [IT deployment guide](https://pythonandvba.com/docs/xllama-add-in/guides/xllama-add-in-it-deployment/)

Both downloads are attached to the [latest release](https://github.com/Sven-Bo/xllama-releases/releases/latest). The redirected download links stay the same for future releases.

## Install

Save your work and close Excel. Run `XLlama-Setup.exe`, then reopen Excel and select **XLlama** in the ribbon. Setup checks the required components. Start Ollama and choose or download a local model in XLlama.

IT administrators can extract `XLlama-IT-Deployment.zip` and run `Deploy-XLlama.ps1 -Action Install` as the intended Windows user in 64-bit Windows PowerShell 5.1. SYSTEM deployment is refused. Follow the included README for prerequisites, updates, detection and removal. Do not register the EXE and IT editions for the same user.

Requires desktop Excel 2016 or newer on 64-bit Windows, the matching .NET 10 Desktop Runtime, WebView2, and Ollama. The bundle contains x86/x64 Excel payloads; actual Excel testing has covered 64-bit Excel. EXTRACT requires dynamic arrays. Native ARM64 Excel, Mac and Excel for the web are unsupported.

## Features

- Local Ollama chat, streamed Markdown answers and saved conversations.
- Compact spreadsheet attachments, including separate selected ranges.
- `XLLAMA.PROMPT` and `XLLAMA.EXTRACT` worksheet formulas.
- Connection status, model management and Help → Diagnostics.
- Free: 10 chat responses per day and five formula cells per workbook. Optional Pro licensing unlocks unlimited chat and formulas, plus conversion to values.

## Updates and removal

Close Excel before updating or uninstalling. Most users update with the latest EXE installer. IT-managed users should receive the next ZIP from their administrator.

Remove **XLlama** or **XLlama (IT deployment)** through Windows Settings → Apps → Installed apps. The ZIP also includes `Deploy-XLlama.ps1 -Action Uninstall`. Saved chats, settings, license and usage records remain in place, along with Ollama and its models.

## Distribution and source visibility

This repository contains distribution information, not the application source project. GitHub's automatic **Source code** archives contain this release repository's contents; the C# application source is not included.

Downloads contain compiled XLL/DLL files and the interface assets needed to run XLlama. IT deployment scripts and interface HTML/CSS/JavaScript are readable. Compiled .NET assemblies can be decompiled; neither packaging format guarantees source secrecy. Developer credentials and customer data are not included.

Version **1.0.0** is unsigned. Windows and company policies may block scripts or add-ins; a ZIP does not bypass those rules. `SHA256SUMS.txt` on the release verifies download integrity, not publisher identity. See release notes for the tested scope.
