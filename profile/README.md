<div align="center">

# Codex Mods

<img src="https://i.postimg.cc/V6zdP9Xf/codex-home-hero.gif" width=256 />

Unofficial tooling, SDKs, RFCs, and mods for the Codex desktop app

</div>

> [!IMPORTANT]  
> This project is highly experimental.  
> Everything should be considered highly unstable unless stated otherwise.  
> Development is progressing steadily but not everything is ready yet. Check each repository for more details.  
> For now, this project targets only the **Windows app**. This is because I only have access to Windows devices, and supporting multiple platforms from the outset would significantly hinder development, especially at such an early stage. External PRs adding MacOS or Linux support will be accepted once the project is fully functional **and** they prove it's working too on those platforms.  
> I started this project while the Codex app was being merged into the ChatGPT app. Support for both the former and the latter will be available from day one. Minimum version will be communicated at a later date (likely `26.715.4045.0`).  
> Content isn't public yet as it is not usable as-is. Source will be synced from the private monorepo as it gets stable.

> [!NOTE]  
> A large portion of the `reverse` & `auto-reverse` projects is now in halt while I work around the absurdly high pricing it occurs.  
> In the meantime, work on the SDK & RFCs is prioritized to let the modding happen faster, even if that means less convenient DX & few breaking changes later :)

## Projects
- [`reverse`](https://github.com/CodexMods/reverse) : A complete toolkit for creating a locally running development version of the Codex app from its APPX package (generic enough to eventually work for virtually all Electron-based apps)
  - Status : Started internally, paused
    - Details : The app launches from both the packed and unpacked sources and exposes the Debug menus. Partial decompilation have been achieved. Recovery from minified source is still progressing and takes most of my time and money. Repacking as a singular binary with new assets haven't been started.
  - Progress : 70%
- [`auto-reverse`](https://github.com/CodexMods/auto-reverse) : A plugin for `reverse` that aims to reduce the time between an upstream app update and a working local version
  - Status : Started internally, paused
    - Details : Partially validated with the next version, still have to walk through the releases history. Recovery still has to be stabilized.
  - Progress : 45%
- [`RFCs`](https://github.com/CodexMods/RFCs) : Specifications describing how the tooling and mod SDK should behave, heavily inspired by the PEP system
  - Status : Started internally
    - Details : First drafts are underway. Work towards standardizing reverse checkpoints & recovered mappings is being done mainly at the research step.
  - Progress : 10%
- [`SDK`](https://github.com/CodexMods/SDK) : A modding SDK for the Codex app that lets you easily create your own mods in minutes, also including AI-oriented skills to help bootstrap development
  - Status : Started internally
  - Progress : 5%
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
- [`mod-multi-accounts`](https://github.com/CodexMods/mod-multi-accounts) : Use the same app with multiple accounts, separate plugins & skills, mods installed, auto balance the usage & more !
  - Status : Not started
  - Progress : 0%

## Pricing
This project is free ! (and will always be 😀)  
However some of the steps will cost you some money (current estimates are around 60M tokens, equating to ~250$ at current API pricing, and spanning over 55+ hours non-stop, still to be confirmed), and it might compound with app updates.  
Work is underway to both dramatically reduce pricing needed between updates (<5$/update given you did the full run at some point) and make mod development need **no** API calls as you could derive recovered names from provided bindings. Pricing optimizations have also been made (ex Flex pricing).  
However that still means that *someone* have to pay for that, and for now that someone is me.  
Current count of expenses are as follows : Pro 5x Plan for July ($120), Pro 20x Plan for August ($240), $280 in raw API costs (a great part have been covered by the "complimentary daily tokens" obtained through [sharing inputs/outputs with OpenAI](https://platform.openai.com/settings/organization/data-controls/sharing)).  
This project is currently wrecking my budget so any support helps ! Here's how you can donate :
- [GitHub Sponsors](https://github.com/sponsors/EDM115)
- [PayPal](https://paypal.me/8EDM115)
- [BuyMeACoffee](https://www.buymeacoffee.com/edm115)
- [Pay with any card or crypto with the Telegram `@tribute` bot](https://t.me/EDM115bots/698)

> [!TIP]  
> Anyone who donates during the early phase (where the main repos are private/the project is not stable) will be refunded once CodexMods is fully working !

## If an OpenAI employee stumbles upon this project
Hello :)  
This project contains neither your original source code nor any reconstructed source code.  
Our tools solely aim to help people perform this process locally on their own computers, using only the files that *you* already provide.  
Users are responsible for how they use these tools.
