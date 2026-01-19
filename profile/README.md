
<div align="center">
<img src="assets/brightdeveloper-banner.png" alt="BrightDeveloper - Build for BrightSign" width="100%">

**Build on BrightSign. Ship in hours, not weeks.**

[![BrightSign](https://img.shields.io/badge/brightsign.biz-8A2BE2?style=for-the-badge)](https://brightsign.biz)
[![BSN.cloud](https://img.shields.io/badge/BSN%20Cloud-49C0FF?style=for-the-badge)](https://www.bsn.cloud/)

</div>

---

## What is BrightDeveloper?

**BrightDeveloper** is BrightSign's developer program—clear documentation, working code, and starter projects ready to customize. Whether you're building a CMS, a kiosk application, or an AI-powered analytics solution, we want you to go from idea to production as fast as possible.

Our goal: **your first successful API call in under 15 minutes**, and a clear path from "Hello World" to a fully working application.

This program is for software developers building on BrightSign. If you just need to create presentations and manage players without writing code, check out [BrightAuthor:connected](https://www.brightsign.biz/brightauthor-connected/) and [BSN.cloud](https://www.brightsign.biz/bsn-cloud/).

---

## Vision & Mission

### Mission
Inspire and empower software developers to build innovative solutions on the BrightSign platform (and enabling AI assistance)

### Vision
Make BrightSign the platform developers choose first. Clear docs, working code, and a complete SDK that AI assistants can use to generate correct, working integrations. Ship in hours, not weeks.

### AI-First Approach
Developers increasingly use LLMs to accelerate their work. **This is the future, and we're building for it.** Every piece of documentation, every code example, and especially our SDK is designed to work seamlessly with AI assistants. When a developer pastes our docs into Claude, Copilot, or Cursor, the generated code should work on the first try.

---

## How We Think About Developer Experience

We've designed everything here for both **humans and AI assistants**. Every guide explains the *why*, not just the *what*. Every code example runs without modification. Paste any of our documentation into Claude, Copilot, or Cursor and get working code.

**Our priorities:**

1. **Cloud-first** — BSN.cloud APIs for managing players, content, and schedules at scale
2. **On-player development** — Chromium (HTML/JavaScript) and Node.js for local applications
3. **Edge AI** — NPU development on XS6 for computer vision and analytics
4. **Extensions** — For capabilities that require going deeper

---

## MCP Server for AI Assistants

Connect your AI coding assistant directly to BrightSign documentation. The **BrightDeveloper MCP Server** gives Claude Code, GitHub Copilot, and other MCP-compatible tools access to our complete technical docs—player APIs, BSN.cloud, BrightScript, and more.

```bash
# Claude Code quick setup
claude mcp add brightdeveloper --transport http https://brightdeveloper-mcp.bsn.cloud/mcp
```

[**MCP Server Setup Guide →**](MCP-SERVER-HOWTO.md)

---

## The Go SDK: gopurple

**[gopurple](https://github.com/BrightDevelopers/gopurple)** is our reference implementation for BSN.cloud—a complete, tested SDK designed to teach AI agents how to interface with BrightSign.

```go
client, _ := gopurple.New()
client.Authenticate(ctx)
devices, _ := client.Devices.List(ctx, nil)
```

**What it includes:**
- OAuth2 authentication with automatic token refresh
- Device management, content management, B-Deploy provisioning
- Remote DWS: screenshots, reboots, file operations—all remotely
- **73 working example programs** (not snippets—complete CLI tools)

**Why Go?** Go is exceptionally easy for AI to understand. Its explicit types, minimal syntax, and straightforward patterns make gopurple an ideal reference implementation. AI agents can study this SDK and generate correct BrightSign integration code in any language they're proficient in—Python, TypeScript, C#, or anything else.

---

## Repositories

| Repository | Description |
|------------|-------------|
| [**gopurple**](https://github.com/BrightDevelopers/gopurple) | Go SDK for BSN.cloud — start here for cloud integrations |
| [**technical-documentation**](https://github.com/BrightDevelopers/technical-documentation) | Technical documentation, API references, and developer guides |
| [**player-examples**](https://github.com/BrightDevelopers/player-examples) | On-player development examples for Chromium, Node.js, and local APIs |

---

## Getting Started

**Building a cloud integration?** Start with **[gopurple](https://github.com/BrightDevelopers/gopurple)**. The SDK handles authentication, pagination, error handling—everything you need to integrate with BSN.cloud.

**Building an on-player application?** Start with [player-examples](https://github.com/BrightDevelopers/player-examples). Interactive kiosks, data-driven displays, and local device control.

**Want to understand the platform?** The [technical-documentation](https://github.com/BrightDevelopers/technical-documentation) repo has comprehensive documentation covering BrightScript, JavaScript, BSN.cloud integration, and advanced topics like NPU development.

---

## Support

Need help? BrightSign provides comprehensive support resources:

- **Discussions**: [GitHub Discussions](https://github.com/orgs/BrightDevelopers/discussions) — Ask questions and share ideas
- **Developer Community**: [BrightSign Community Forums](https://github.com/orgs/BrightDevelopers/discussions)
- **Product Documentation**: [docs.brightsign.biz](https://docs.brightsign.biz/)
- **Product Support**: [brightsign.biz/support](https://www.brightsign.biz/support/)

---

## Contributing

We welcome contributions from the community! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to participate.

---

<div align="center">

**Brought to Life by BrightSign®**

© 2025-2026 BrightSign LLC. All rights reserved.

</div>
