# Ligus

**Ask your documents anything. Stop overpaying for tokens.**

![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11-0078D4)
![Version](https://img.shields.io/badge/version-1.0.0-brightgreen)
![Local first](https://img.shields.io/badge/local--first-private%20by%20design-blueviolet)

Ligus is a Windows application that lets you chat with your own documents —
PDFs, reports, manuals, contracts, books — while paying up to ~95% less per
question than sending the whole document to an AI service every time.

Your files never leave your machine. Ligus reads each document once, on your
own computer, and per question sends only the parts that matter to the AI
provider **you** choose, using **your own** API key. No accounts, no uploads,
no telemetry.

---

## Download

➡ **[Get the latest release](https://github.com/bharath-ui1027/ligus/releases)**

One file: `Ligus-Setup.exe` — a standard Windows installer. No admin rights
needed.

Current release: **v1.0.0**

## Install

1. Download `Ligus-Setup.exe` from the Releases page.
2. Run it and follow the installer (installs per-user, takes under a minute).
3. Open **Ligus** from the desktop or Start menu — it opens in your browser.
4. Add a document, paste your provider key into the app, and ask your first
   question.

## ⚠ Windows SmartScreen — please read

On first run, Windows may show a blue **"Windows protected your PC"**
(SmartScreen) warning. This is expected: Ligus is a brand-new, independently
published application and is not yet code-signed, so Windows cannot recognise
the publisher yet. SmartScreen shows this for almost all new indie software.

To proceed:

1. Click **More info**.
2. Click **Run anyway**.

To be extra sure your copy is genuine, verify its checksum (below) against
the value published here and in the release notes.

## Verify your download

SHA-256 of `Ligus-Setup.exe` (v1.0.0):

```
4D588C455998E0A0F08BDF1204CD7436748E93476697F145FB973C007574168F
```

Check yours in PowerShell:

```powershell
Get-FileHash .\Ligus-Setup.exe -Algorithm SHA256
```

## Why Ligus

- **Up to ~95% fewer tokens per question** — ask a 300-page document a
  hundred questions without paying for all 300 pages a hundred times.
- **Private by design** — documents are read and stored only on your PC;
  the app holds no keys on any server and sends nothing anywhere except to
  the provider you configured.
- **One-time purchase** — no subscription, no monthly fees, no seat pricing.
- **Built for real documents** — scanned pages, large files and messy
  real-world documents are first-class citizens, not edge cases.
- **Measured, not marketed** — the engine was validated on a
  1,002-question evaluation over 100 real documents before release.

## How it works (the short version)

1. You add a document. Ligus reads it **once**, locally.
2. You ask a question. Ligus works out which parts of the document are
   relevant — still locally.
3. Only those parts go to your AI provider, with your key, straight from
   your machine. You get the answer; the provider bill stays small.

## Requirements

- Windows 10 or 11 (64-bit)
- An API key from a supported provider (OpenAI, Anthropic, Gemini, or a
  compatible endpoint)
- ~400 MB free disk space

## About

Ligus is designed, built and maintained by **Bharath Sai Kondaveeti**, a
DevOps & Platform Engineer (previously with Amazon's infrastructure teams in
Hyderabad), specialising in reliable systems, cost engineering and applied
AI tooling.

Product site: [ligus.systeme.io](https://ligus.systeme.io/)

## License

Ligus is commercial software, distributed as a compiled application —
see [LICENSE.md](LICENSE.md). This repository exists so buyers can verify
the official download source and release integrity; it does not contain
the application's source code.

Third-party open-source components are credited in
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md), including components
licensed under the [Apache License 2.0](APACHE-2.0.txt).
