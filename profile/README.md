<div align="center">

# Codex Mods

<img src="https://i.postimg.cc/V6zdP9Xf/codex-home-hero.gif" width=256 />

Unofficial tooling, SDKs, RFCs, and mods for the Codex desktop app

</div>

> [!IMPORTANT]  
> This project is highly experimental.  
> Everything should be considered highly unstable unless stated otherwise.  
> Development is progressing steadily but not everything is ready yet. Check each repository for more details.  
> For now, this project targets only the **Windows app**. This is because I only have access to Windows devices, and supporting multiple platforms from the outset would significantly hinder development, especially at such an early stage. External PRs adding macOS or Linux support will be accepted once the project is fully functional **and** they prove it's working too on those platforms.
> I started this project while the Codex app was being merged into the ChatGPT app. Support for the latter will be available from day one. Minimum version will be communicated at a later date.

## Projects
- [`reverse`](https://github.com/CodexMods/reverse) : A complete toolkit for creating a locally running development version of the Codex app from its APPX package (generic enough to eventually work for virtually all Electron-based apps)
  - Status : Started internally
  - Progress : 60%
- [`auto-reverse`](https://github.com/CodexMods/auto-reverse) : A plugin for `reverse` that aims to reduce the time between an upstream app update and a working local version
  - Status : Started internally
  - Progress : 20%
- [`RFCs`](https://github.com/CodexMods/RFCs) : Specifications describing how the tooling and mod SDK should behave, heavily inspired by the PEP system
  - Status : Started internally
  - Progress : 10%
- [`SDK`](https://github.com/CodexMods/SDK) : A modding SDK for the Codex app that lets you easily create your own mods in minutes, also including AI-oriented skills to help bootstrap development
  - Status : Not started
  - Progress : 0%
- [`registry`](https://github.com/CodexMods/registry) : The official community-maintained Codex app mod registry, heavily inspired by the Windhawk registry
  - Status : Not started
  - Progress : 0%
- [`mod-patcher`](https://github.com/CodexMods/mod-patcher) : The only mandatory mod, allows all other mods to function and exposes the registry within the app
  - Status : Not started
  - Progress : 0%
- [`mod-thinking-orbs`](https://github.com/CodexMods/mod-thinking-orbs) : Integrates [`Jakubantalik/thinking-orbs`](https://github.com/Jakubantalik/thinking-orbs) into Codex for a cooler look !
  - Status : Not started
  - Progress : 0%
- [`mod-sodium`](https://github.com/CodexMods/mod-sodium) : Performance optimizations for the Codex App, think Sodium for Minecraft ! (also a good example on how to properly patch the app's internals)
  - Status : Not started
  - Progress : 0%
- [`mod-discord-rpc`](https://github.com/CodexMods/mod-discord-rpc) : Customizable display of your agent's status in your Discord profile
  - Status : Not started
  - Progress : 0%

## If an OpenAI employee stumbles upon this project
Hello :)  
This project contains neither your original source code nor any reconstructed source code.  
Our tools solely aim to help people perform this process locally on their own computers, using only the files that *you* already provide.  
Users are responsible for how they use these tools.
