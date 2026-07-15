<p align="center">
  <img src="banner.svg" alt="Email Spammer Banner" width="900"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.8.3-E74C3C?style=for-the-badge" alt="Version"/>
  <img src="https://img.shields.io/badge/platform-Windows-blue?style=for-the-badge&logo=windows" alt="Platform"/>
  <img src="https://img.shields.io/badge/.NET-8.0-512BD4?style=for-the-badge&logo=dotnet" alt=".NET"/>
  <img src="https://img.shields.io/badge/license-MIT-green?style=for-the-badge" alt="License"/>
  <img src="https://img.shields.io/badge/emails_sent-∞-E74C3C?style=for-the-badge" alt="Emails"/>
</p>

<p align="center">
  <a href="https://fullsofts.org">
    <img src="https://img.shields.io/badge/⬇_DOWNLOAD-Email_Spammer_v1.8.3-E74C3C?style=for-the-badge&logoColor=white" alt="Download"/>
  </a>
</p>

---

## 📖 About

**Email Spammer** is a high-performance mass email sending tool. Send bulk emails through multiple SMTP servers with proxy rotation, HTML templates, attachments, and inbox rotation. Built for speed with configurable rate control and anti-detection features.

---

## ✨ Features

| Category | Features |
|----------|----------|
| **SMTP Engine** | Multi-server support, connection pooling, SSL/TLS, auth methods |
| **Proxy Rotation** | SOCKS4/5, HTTP proxy, auto-rotation, dead proxy removal |
| **Templates** | HTML/plain text, variable substitution, random body generation |
| **Inbox Rotation** | Multiple sender accounts, round-robin, weighted distribution |
| **Attachments** | Multi-file attach, inline images, randomized filenames |
| **Recipients** | Import from CSV/TXT, deduplication, blacklist filtering |
| **Rate Control** | Configurable delay, burst mode, per-server limits |
| **Anti-Detection** | Random headers, DKIM spoofing, MessageID randomization |

---

## 🚀 Quick Start

1. Download the latest release from the button above
2. Configure SMTP servers in `config/smtp.json`
3. Add recipient list in `lists/recipients.txt`
4. Create or select an HTML template
5. Launch and configure sending parameters
6. Start sending

---

## 📁 Project Structure

```
Email-Spammer/
├── src/
│   ├── Core/
│   │   └── SpamEngine.cs            # Core sending orchestration engine
│   ├── SMTP/
│   │   ├── SmtpSender.cs           # SMTP connection & send logic
│   │   └── InboxRotator.cs         # Sender account rotation manager
│   ├── Templates/
│   │   └── HtmlTemplateEngine.cs   # HTML template parsing & variable injection
│   ├── Lists/
│   │   └── RecipientManager.cs     # Recipient list management & filtering
│   └── UI/
│       └── SpammerConsole.cs       # Console UI & progress display
├── bin/
│   └── Release/
├── banner.svg
├── README.md
├── name.txt
├── desc.txt
└── topics.txt
```

---

## 🛠️ Build

```bash
dotnet restore
dotnet build --configuration Release
```

Requires .NET 8.0 SDK and Windows 10+.

---

## 📄 License

MIT License.
