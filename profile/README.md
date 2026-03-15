<p align="center">
  <img src="https://img.shields.io/badge/Status-Alpha_v1.0.1-FF6B35?style=for-the-badge" alt="status"/>
  <img src="https://img.shields.io/badge/Platform-Windows_|_macOS_|_Linux-47848F?style=for-the-badge&logo=electron&logoColor=white" alt="platform"/>
  <img src="https://img.shields.io/badge/Local_First-SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white" alt="sqlite"/>
  <img src="https://img.shields.io/badge/License-AGPL--3.0-green?style=for-the-badge" alt="license"/>
</p>

<h1 align="center">🧬 BiamOS</h1>

<p align="center">
  <strong>The Browser is Dead. Welcome to the Autonomous Workspace.</strong><br/>
  An experimental AI-Native Workspace OS that doesn't just read the web — it acts on it.
</p>

<p align="center">
  <br/>
  <b><a href="https://github.com/BiamOS/BiamOS">👉 VIEW THE MAIN REPOSITORY (CODE & INSTALL) 👈</a></b>
  <br/><br/>
</p>

---

## 🤯 See the "Wow" in Action

Forget scripts. Forget Selenium. Watch the **BiamOS Autonomous Agent** navigate the web like a human. 

<table>
<tr>
<td align="center" width="33%">

**🚀 V2: NASA → X Autonomous Post**

[![AI Agent Demo](https://img.youtube.com/vi/ycjD5EDTw28/maxresdefault.jpg)](https://youtu.be/ycjD5EDTw28?si=M-HOXTNraJhX0mXI)

*One prompt: Reads a NASA article, takes notes, navigates to X.com, writes a tweet, and posts it.*

</td>
<td align="center" width="33%">

**📧 Zero-Click Email Research**

[![Workflow Demo](https://img.youtube.com/vi/hPPa_Wx1dnM/maxresdefault.jpg)](https://youtu.be/hPPa_Wx1dnM?si=vc1Fww9B7nuwzoEV)

*Opens Gmail, searches YouTube in the background, writes a briefing, and drafts the email.*

</td>
<td align="center" width="33%">

**👻 The Ghost-Auth Magic**

[![Overview Demo](https://img.youtube.com/vi/QOKNlAsJjyw/maxresdefault.jpg)](https://youtu.be/QOKNlAsJjyw?si=ZfFY957UVoGrVQ5o)

*No OAuth. No API keys. BiamOS reads your authenticated webview DOM directly.*

</td>
</tr>
</table>

> **👆 Click any thumbnail to watch the raw, unedited demos on YouTube.**

---

## 🔥 Why BiamOS changes everything

**BiamOS is not an API wrapper.** It is a proactive, self-hosted command center. By combining a native Chromium webview with a local AI middleware pipeline, we bypass the biggest bottlenecks of modern software.

### 🤖 1. The Autonomous Web Agent (`/act`)
Type `/act` and watch the magic happen. The AI takes control of the built-in browser. It clicks, types, scrolls, and navigates. It performs background web searches (without changing your tab!) to gather real-time data, then executes complex workflows across multiple websites. 
*It’s an employee, not a chatbot.*

### 👻 2. "Ghost-Auth" (Zero-OAuth Integrations)
Stop begging for API access. Log into Gmail, Notion, or WhatsApp *normally* via the BiamOS Webview. Ask the Copilot: *"Draft a polite reply to Andreas."* The local AI securely reads the DOM, understands the context, and drafts the response. **No APIs. No tracking. Pure local magic.**

### 🧩 3. Dynamic UI Canvas
Stop reading Markdown text walls. BiamOS translates AI responses into beautiful, interactive UI blocks (weather cards, charts, data tables). Pin them to your dashboard, and they become a living, auto-updating workspace.

---

### 📝 A Note from the Creator

Hi, I'm Gabor, an Automation Engineer based in Vienna. 👋 

I built BiamOS because the current digital workspace is broken. I was tired of the constant context-switching, managing endless API keys, and dealing with AI chatbots that are completely blind to my actual workflow. 

I didn't just want another AI wrapper — I wanted an **Autonomous Operating Layer**. With the recent explosion of Vision LLMs and local processing, I realized I could finally build the exact system I've been dreaming of. 

**To be completely honest:** My head is still buzzing with ideas. I have a massive backlog on how to push this architecture even further. But instead of building in secret, I wanted to get this Alpha out to the community *now*. 

**⭐ Support a Solo Developer**
Building this entire architecture alone took countless nights of intense engineering. If you believe that the future of the desktop is intent-driven, autonomous, and open-source, **please consider dropping a ⭐️ Star on the [Main Repository](https://github.com/BiamOS/BiamOS)!** It gives this project the visibility it needs to grow.

---

## 🏗️ The Engine Under the Hood

Built for speed and local-first security. A seamless bridge between modern web tech and native desktop capabilities.

```mermaid
graph TD
    A[User Prompt / Voice] -->|EXECUTE| B(Intent Router)
    B -->|DOM SCRAPE & VISION| C[Electron Webview Agent]
    B -->|API ROUTING| D[Hono + Bun Backend]
    C -->|Simulates| K[Human Clicks & Typing]
    D --> E{Local SQLite}
    C --> G[React + MUI Canvas]
    D --> G
    G -->|Renders| H(Dynamic UI Dashboards)
