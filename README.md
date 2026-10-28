# Awesome Project Epoch Reborn

A curated list of Project Epoch Reborn resources: official links, client setup, addons, client enhancements, community and tools.

The community-run continuation of Project Epoch, a custom Classic+ server on the 3.3.5a client (build 12340), live since 23 October 2026.

## Contents

- [Official](#official)
- [Client](#client)
- [Addons](#addons)
- [Client enhancements](#client-enhancements)
- [Community](#community)
- [Tools](#tools)
- [Contributing](#contributing)
- [Notes](#notes)

## Official

- [Website](https://project-epoch.org/) / [Create account](https://project-epoch.org/register.html)
- [Forums](https://project-epoch.org/forums/?view=latest) – [Announcements](https://project-epoch.org/forums/?board=announcements), [Patch notes](https://project-epoch.org/forums/?board=patch-notes), [Help & Support](https://project-epoch.org/forums/?board=support), [Guild Recruitment](https://project-epoch.org/forums/?board=guild-recruitment), plus class boards
- [Bug tracker](https://project-epoch.org/bugs.html)
- [Talent calculator](https://project-epoch.org/talents/)
- [Class overview](https://project-epoch.org/classes/overview/) – every class has its own page and calculator
- [Features](https://project-epoch.org/features/) – [challenges](https://project-epoch.org/features/challenges/), [PvP](https://project-epoch.org/features/pvp/), [dungeons](https://project-epoch.org/features/instances/dungeons/) and [raids](https://project-epoch.org/features/instances/raids/), [racial knowledge](https://project-epoch.org/features/racial/), [professions](https://project-epoch.org/features/professions/overview/), [combos](https://project-epoch.org/features/combos/)
- [Server rules](https://project-epoch.org/rules.html) / [Donate](https://project-epoch.org/donate.html)

Realm status sits in the site header or grab it raw from `https://project-epoch.org/api/realm-status`.

Official chat runs on [Fluxer](https://chat.project-epoch.org), not Discord. The team migrated off Discord in September 2026, so community Discords are fan-run.

## Client

Use a clean enUS 3.3.5a client (build 12340). Epoch does not distribute it, but the original team's trimmed client (~12 GB) is still on their CDN: [3.3.5-enUS-minified.zip](https://epoch-cdn.com/client/3.3.5-enUS-minified.zip). If that ever dies, [ChromieCraft's downloads](https://chromiecraft.com/en/downloads/) serve the same build. Budget about 20 GB with Epoch's patches on top.

Extract it into a folder you own, then point the [official launcher](https://project-epoch.org/how-to-connect.html) (connection issues? see [Notes](#notes)) at the folder holding `Wow.exe`, press Update, then Play. Connection setup is built in: no access key, no editing `realmlist.wtf`.

- **Windows 10/11**: run `ProjectEpochLauncher.exe`. SmartScreen may warn because the exe is unsigned: More info, then Run anyway.
- **Linux**: run the Windows launcher through Steam with Proton (Experimental is personally tested and working), use another Wine frontend such as Lutris or Bottles or run the native Linux launcher (`epoch-launcher`), which the site labels a preview build. Either way, point the launcher at your extracted client folder.

## Addons

Most WotLK 3.3.5a addons work as-is. Addons built on static game data (quest helpers, loot tables, boss mods) show wrong or missing data without an Epoch version, so check the AddOns board and wiki before calling something broken.

### Where to get them

- [Epoch Forums – AddOns](https://project-epoch.org/forums/?board=addons) – pinned Addons Mega Thread lives here
- [Warperia – Project Epoch](https://warperia.com/server-addons/project-epoch/) – Epoch-tagged addons, with a desktop installer and update checker
- [Community wiki – AddOns](https://project-epoch-wow.fandom.com/wiki/AddOns) – community addon list, install notes and troubleshooting
- [GitHub search](https://github.com/search?q=project+epoch+addon&type=repositories&s=updated&o=desc) – most Epoch addons live in personal repos, sorted by recency
- [NoM0Re/WoW-3.3.5a-Addons](https://github.com/NoM0Re/WoW-3.3.5a-Addons) – big pack of general 3.3.5a addons
- [Felbite](https://felbite.com/) – long-running WotLK addon archive
- [LegacyWoW](https://legacy-wow.com/wotlk-addons/) / [wowgaming addon archive](https://wowgaming.github.io/addon-archive/) – older 3.3.5 collections

### Epoch-specific

- [pfQuest Epoch](https://github.com/Bennylavaa/pfQuest-epoch) – Epoch quest and item data, extending [pfQuest-WotLK](https://github.com/shagu/pfQuest)
- [Questie for Epoch](https://github.com/NeticSoul/questie-335-epoch) – if you would rather stay on Questie, this fork merges pfQuest Epoch's data in
- [Zygor Guides Viewer](https://github.com/SimonGaufreteau/ZygorGuidesViewer) – 1-60 leveling guide ported to Epoch
- [What's Training? Epoch](https://github.com/ZythDr/Whats-Training-Epoch) – every spell your class learns, in a spellbook tab
- [Atlas Project Epoch](https://github.com/Raynbock/Atlas-Project-Epoch) / [AtlasLoot Project Epoch](https://github.com/Raynbock/AtlaslootProjectEpoch) / [AtlasQuest](https://github.com/Rofos2011/AtlasQuest) – maps and loot tables with Epoch content; AtlasQuest needs Atlas
- [DBM-epoch](https://warperia.com/addon/dbm-epoch/) – boss mods with Epoch encounters
- [Aux Epoch](https://warperia.com/addon/aux-epoch/) – Aux auction house, ported to Epoch
- [ConLogs-Epoch](https://github.com/Defcons/ConLogsApp) – embeds gear, talents and position in your combat log, so one Epog Logs upload has everything
- [ElvUI-Epoch](https://github.com/Bennylavaa/ElvUI-Epoch) – ElvUI tuned for Epoch
- [pfUI Epoch](https://github.com/Fragglechen/pfui-epoch) – full interface replacement, Shagu's pfUI ported for Epoch
- [epoch-addons](https://github.com/wick3dr0se/epoch-addons) – personal collection, currently an ElvUI fork (performance optimized) plus seal-twist and damage meter plugins
- [Defcons/epoch-addons](https://github.com/Defcons/epoch-addons) – community ports and client fixes, archived on 26 September 2026
- [EpochCN](https://github.com/z980944038-dev/EpochCN) – Chinese localization: quests, UI, tooltips, map markers, plus social tools for finding Chinese-speaking players. Its `core` build wants `Data/patch-Z.MPQ` for static text
- Kindrack's Epoch ports: [ModernMapMarkers](https://github.com/Kindrack/ModernMapMarkers-Epoch) (dungeon, raid, world boss, boat, zeppelin, tram and portal markers), [Talented](https://github.com/Kindrack/Talented-Epoch) (build manager for the TBC-style trees), [Leatrix Plus](https://github.com/Kindrack/Leatrix_Plus) (the usual QoL suite)

### Fine on any 3.3.5a

- [WeakAuras WotLK](https://github.com/NoM0Re/WeakAuras-WotLK) – WeakAuras 5.22.1 backported to 3.3.5a and still maintained; grab `WeakAuras2.zip` from its releases and extract all seven folders into `Interface/AddOns`. It picks up the nameplate and unit APIs from Awesome WotLK.
- [DragonUI](https://github.com/NeticSoul/DragonUI) – modular retail-style interface
- [Auctionator 3.3.5 fixed](https://github.com/thierbig/Auctionator-3.3.5-Fixed) – auction house with a working modern sell tab
- **ElvUI plugins:** General 3.3.5a plugins verified working with [ElvUI-Epoch](https://github.com/Bennylavaa/ElvUI-Epoch): [ProjectZidras](https://github.com/Zidras/ElvUI_ProjectZidras), [Enhanced](https://github.com/ElvUI-WotLK/ElvUI_Enhanced), [AddOnSkins](https://github.com/ElvUI-WotLK/ElvUI_AddOnSkins), [SwingBar](https://github.com/ElvUI-WotLK/ElvUI_SwingBar), [ExtraActionBars](https://github.com/ElvUI-WotLK/ElvUI_ExtraActionBars), [VisualProcs](https://github.com/ElvUI-WotLK/ElvUI_VisualProcs), [DmgAtNameplates](https://github.com/Bennylavaa/ElvUI_DmgAtNameplates)

### Install

Extract addon folders into `<client folder>/Interface/AddOns/`, with the folder holding the `.toc` file directly inside `AddOns`.

- GitHub ZIPs may add a suffix (`-main` or `-master`). Rename the folder if needed so the `.toc` file is directly inside AddOns.
- Restart the game rather than `/reload` when an addon is missing.
- Tick Load out of date AddOns on the character screen if it does not show up.
- `/reload` (`/rl` for *speed*) after UI changes and back up `Interface/` and `WTF/` now and then.

## Client enhancements

Optional patches and tools that change the client itself rather than adding to it.

### Asset packs

- [EpochAuthenticHD](https://github.com/thierbig/EpochAuthenticHD) – upscaled textures, HD models, trees, skyboxes, 4K maps, sounds and music, plus a Cataclysm water patch (`PATCH-W`) and an optional fog mod. MPQs go in `Data/`, icons in `Interface/`; skip the icon pack for more FPS and delete `PATCH-E` for the original character models. Its DXVK section is a separate optional step for Vulkan, not part of the pack.
- [Patch-N_Epoch-Reborn](https://github.com/Kindrack/Patch-N_Epoch-Reborn) – map data for dungeon entrances, caverns and mines

### Client features

- [Awesome WotLK](https://github.com/noname08662/awesome_wotlk) – the actively developed successor: MSDF vector fonts, `[@cursor]` and `[@playerlocation]` macros, camera FOV, nameplates out to 200 yards with a `C_NamePlate` API that lets WeakAuras anchor spells and castbars, one-key smart interaction that loots, skins and uses what's in front of you, TTS, `/fcapture`, and `-login` auto-login. Extract the release into your client folder and run `AwesomeWotlkPatch.exe` once to patch `Wow.exe`.
- [AwesomeEpoch](https://github.com/thierbig/AwesomeEpoch) – a fork of the same original codebase that injects at runtime instead of patching the exe, with anti-detection modules, the stance and form dancing that the successor dropped (swap stance and cast in the same click) and a modern interaction button, less actively developed.

### Renderers

Both modify water, fog and lighting through different rendering approaches. They're alternatives, not meant to be used together. Both originated as Ascension-client projects but have been community-verified working on Reborn. They also overlap visually with EpochAuthenticHD's water patch, which replaces MPQ assets rather than injecting a renderer.

- [Modern WoW Renderer](https://github.com/Corfirean/modern-wow-renderer) – a 32-bit `d3d9.dll` proxy: lighting, volumetric fog, weather, water, post-processing.
- [CoAVolFog](https://github.com/jealous-sound/coa-vfog) – a `version.dll` proxy: volumetric fog, god rays, water with wave simulation. It hooks the D3D9 call instead of replacing the DLL, with a documented Linux route.

### Making your own

- [Ladik's MPQ Editor](https://www.wowmodding.net/files/file/149-ladiks-mpq-editor/) opens and repacks client MPQs, [wow.export](https://github.com/Kruithne/wow.export) pulls models and textures out, [WMVx](https://github.com/Frostshake/WMVx) previews them, [WDBXEditor](https://github.com/WowDevTools/WDBXEditor) edits the client's DBC data. Most Epoch mods are MPQ files, so these are the tools for looking inside them.

## Community

- [Fluxer chat](https://chat.project-epoch.org) – official, sign in with your game account
- [Fluxer – troubleshooting channel](https://chat.project-epoch.org/channels/1547040060984000512/1547040060984000543) – launcher, client and addon problems, ask here before giving up
- [WoWRetro Enhancements](https://discord.gg/QXA59eWUMj) – Discord for retro-server addon help, plus a [forum addon index](https://project-epoch.org/forums/?topic=101)
- [r/wowservers](https://www.reddit.com/r/wowservers/) – player discussion and server news
- Creators posting Epoch content at launch: [SLiMOFI](https://www.youtube.com/@SLiMOFI), [Damonism](https://www.youtube.com/@Damonism), [Venario](https://www.youtube.com/@venarioo), [Malonze Gaming](https://www.youtube.com/@MalonzeGaming)
- [Community wiki](https://project-epoch-wow.fandom.com/wiki/Project_Epoch_Wiki) – addon list, install guides, data safety notes

## Tools

- [EpochDB](https://epochdb.net) – Epoch database: NPCs, items, quests, loot tables, vendors, a talent calculator and raid timers, fed by its own data [addon](https://github.com/MrBoxie88/EpochDB)
- [Epog Logs](https://epoglogs.com) – combat logs with rankings, target dummy parses, dungeon speedruns, progression and every guild on the realm, plus armory, gear compare and simulators. Discord sign-up
- [GitAddonsManager](https://woblight.gitlab.io/overview/gitaddonsmanager/) – install and update addons from GitHub or GitLab URLs, stripping `-master`/`-main` suffixes
- [Warperia](https://warperia.com/) – catalogue plus a desktop app that installs into `Interface/AddOns/` and checks for updates
- Realm status from the terminal: `curl https://project-epoch.org/api/realm-status`
- [WoW 3.3.5a addon wiki](https://github.com/NeticSoul/wow-335a-addon-wiki) – API and widget reference for this client build, for fixing an addon rather than replacing it

## Contributing

The project takes volunteers, no experience with the server required to start.

- Report bugs on the [bug tracker](https://project-epoch.org/bugs.html), with reproduction steps
- Apply as a game master, developer, content creator or tester through the forms on the [website](https://project-epoch.org/#forms)
- [Donate](https://project-epoch.org/donate.html) if you just want to cover running costs

Found something missing or wrong here? Open a pull request or an issue.

## Notes

- Disconnects, lag or a connection that never goes through: Cloudflare WARP can sometimes improve routing, depending on your ISP and location. More in the [Connection/DC/Ping Issues?](https://project-epoch.org/forums/?topic=66) thread.
- The project does not distribute the game client and nothing legitimate ever needs your password except the site and client; no GM will ask for it in Fluxer or a DM.
- Back up your client before applying MPQ patches or injecting DLLs. The launcher re-downloads anything it manages, but it will not undo your own additions.
- Epoch ships its own `PATCH-D` and `PATCH-M`. HD asset packs that used those letters have to be renamed, EpochAuthenticHD moved its files up a letter (D→E, E→F, F→G, M→N) for exactly this reason.
- If an addon misbehaves after a server patch, check for an Epoch build before assuming it is broken.
