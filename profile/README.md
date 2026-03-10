<p align="center">
  <img src="https://img.shields.io/badge/BiamOS-v1.0.0-blueviolet?style=for-the-badge&logo=windows&logoColor=white" alt="version"/>
  <img src="https://img.shields.io/badge/Electron-Desktop-47848F?style=for-the-badge&logo=electron&logoColor=white" alt="electron"/>
  <img src="https://img.shields.io/badge/Local_First-SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white" alt="sqlite"/>
  <img src="https://img.shields.io/badge/License-AGPL--3.0-green?style=for-the-badge" alt="license"/>
</p>

<h1 align="center">
  <br/>
  BiamOS
</h1>

<p align="center">
  <strong>Base for Intent & AI Middleware</strong><br/>
  The AI-Native Workspace OS for Windows, macOS, and Linux.
</p>

<br/>

<p align="center">
  <em>[ 🎥 Insert 60-second "Holy Shit" Demo Video Here ]</em>
</p>

<br/>

**BiamOS is not just an API wrapper.** It is a proactive, self-hosted command center that redefines how you interact with the web. By combining a native Chromium webview with a local AI middleware pipeline, BiamOS reads your context, bypasses complex API authentication via **Ghost-Auth**, and generates a dynamic, modular UI dashboard in real-time. 

> *Don't give the AI context. Let the AI read your context securely.*

---

## 🔥 The Paradigm Shift: Zero-OAuth "Ghost" Integrations

Forget generating API keys, managing OAuth scopes, or begging for API access. We built a native Chromium Webview directly into the OS layer. 

**How Ghost-Auth works:**
1. Log into Gmail, Notion, Teams, or WhatsApp *normally* via the BiamOS Webview.
2. Ask the Copilot: *"Draft a polite reply to Andreas saying Friday at 12:00 works."*
3. The local AI securely reads the DOM directly from the webview, understands the context (sender name, meeting time), and drafts the perfect response. 
4. **No APIs. No tracking. Pure local magic.**

🛡️ **Smart Privacy Shield:** You are always in control. Sensitive domains (banking, email) are automatically placed on a privacy blocklist. Background auto-analysis is strictly **paused**. The AI only reads the page context when you *explicitly* ask a question in the sidebar.

---

## 🧠 Dual-Agent Architecture

BiamOS features two highly specialized AI models working in tandem to handle your entire workflow:

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>🎛️ 1. The System Assistant</h3>
      <p><strong>Your OS Controller.</strong> Lives in the main canvas workspace. Uses voice control (with native TTS output) to route your intents. It decides whether to search the web, query a local API, or manage your workspace. It translates raw data into beautiful UI blocks.</p>
    </td>
    <td width="50%" valign="top">
      <h3>🌐 2. The Web Copilot</h3>
      <p><strong>Your Browser Buddy.</strong> Lives strictly inside the webview sidebar. It is context-aware, reading <em>only</em> the specific page you are currently browsing to summarize content, extract data, or draft replies based on the active DOM.</p>
    </td>
  </tr>
</table>

---

## ✨ Features that redefine the Desktop

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>🧩 Dynamic UI Canvas</h3>
      <p>Stop reading Markdown text walls. The LLM renders completely customizable UI blocks (weather cards, metric rows, feeds, tables). Pin these blocks to your canvas to build a persistent, living dashboard that updates automatically.</p>
    </td>
    <td width="50%" valign="top">
      <h3>🔌 Integration Shop & Templates</h3>
      <p>BiamOS comes with a built-in integration shop. Toggle or filter integrations in the left sidebar. Need a custom endpoint? Create it instantly via AI Discovery, Swagger imports, or manual JSON schema.</p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>🎙️ Natural Voice Control</h3>
      <p>Speak to your OS naturally. The System Assistant processes your spoken intent, executes the necessary background routing, and replies with high-quality Text-to-Speech (TTS) audio.</p>
    </td>
    <td width="50%" valign="top">
      <h3>🕵️ 1-Click Data Audit</h3>
      <p>Transparency is a feature. The dedicated "Data Audit" panel shows you exactly what is stored locally (API keys, settings, webview cookies). Wipe your entire digital footprint with a single <strong>"Delete All Data"</strong> click.</p>
    </td>
  </tr>
</table>

---

## 🏗️ The Tech Stack

BiamOS is engineered for speed and local-first security. Built as a monorepo, it seamlessly bridges modern web tech with native desktop capabilities.

```mermaid
graph TD
    A[User Intent / Voice] -->|EXECUTE| B(Concierge Agent)
    B -->|DOM SCRAPE| C[Electron Webview]
    B -->|API CALL| D[Hono + Bun Backend]
    D --> E{Smart Router}
    E --> F[SQLite + Drizzle]
    C --> G[React + MUI Canvas]
    E --> G
    G -->|Renders| H(Dynamic UI Blocks)
