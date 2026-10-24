# Awesome Project Epoch Reborn

A curated list of Project Epoch Reborn resources: official links, client setup, addons, client enhancements, community and tools.

Project Epoch Reborn is the community-run continuation of Project Epoch, a custom Classic+ server with original questlines, reworked classes, custom dungeons, world PvP and optional challenges, on the 3.3.5a client (build 12340). It went live on 23 October 2026.

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
- [Forums](https://project-epoch.org/forums/?view=latest) – [Announcements](https://project-epoch.org/forums/?board=announcements), [Patch notes](https://project-epoch.org/forums/?board=patch-notes), [Help & Support](https://project-epoch.org/forums/?board=support), [Guild Recruitment](https://project-epoch.org/forums/?board=guild-recruitment), plus a board per class
- [Bug tracker](https://project-epoch.org/bugs.html)
- [Talent calculator](https://project-epoch.org/talents/)
- [Class overview](https://project-epoch.org/classes/overview/) – every class gets its own page and calculator
- [Features](https://project-epoch.org/features/) – [challenges](https://project-epoch.org/features/challenges/), [PvP](https://project-epoch.org/features/pvp/), [dungeons](https://project-epoch.org/features/instances/dungeons/) and [raids](https://project-epoch.org/features/instances/raids/), [racial knowledge](https://project-epoch.org/features/racial/), [professions](https://project-epoch.org/features/professions/overview/), [race and class combos](https://project-epoch.org/features/combos/)
- [Server rules](https://project-epoch.org/rules.html)
- [Donate](https://project-epoch.org/donate.html)

Realm status sits in the site header, or grab it raw from `https://project-epoch.org/api/realm-status`.

Official chat runs on [Fluxer](https://chat.project-epoch.org), not Discord. The team migrated off Discord in September 2026, so community Discords are fan-run.

## Client

Use a clean enUS 3.3.5a client (build 12340). Epoch does not distribute it, but the client the original team published is on their CDN: [3.3.5-enUS-minified.zip](https://epoch-cdn.com/client/3.3.5-enUS-minified.zip), a trimmed client at ~12 GB. If that link ever dies, [ChromieCraft's downloads](https://chromiecraft.com/en/downloads/) serve the same build, though the original is the one to prefer. Budget around 20 GB once Epoch's patches land on top.

Extract it into a folder you own, then point the [official launcher](https://project-epoch.org/how-to-connect.html) (if you have connection issues see: [notes](#notes)) at the folder holding `Wow.exe`, press Update, wait for the patches to verify, then press Play. Connection setup is built into the launcher: no access key, no editing `realmlist.wtf`.

- Windows 10/11: extract the ZIP and run `ProjectEpochLauncher.exe`. SmartScreen may warn you the first time because the exe is unsigned, click More info then Run anyway.
- **Linux:** two ways in. Run the launcher natively, extract the Linux archive and start `epoch-launcher`, or add the Windows `ProjectEpochLauncher.exe` to Steam as a Non-Steam Game and force Proton Experimental on it in its compatibility settings, then launch it from Steam. Either way, point the launcher at your extracted client folder and pick the Wine or Proton build you want in the launcher's Proton/Wine setup (the sliders icon, top right). The site labels the native launcher a preview build, so if it gives you trouble, fall back to the Steam route.

## Addons

Most WotLK 3.3.5a addons work as-is. Epoch ships custom quests, items, spells and loot, so addons built on static game data (quest helpers, loot tables, boss mods) show wrong or missing data unless they have an Epoch version. Check the AddOns board and the community wiki before assuming something is broken.

### Where to get them

- [Epoch Forums – AddOns](https://project-epoch.org/forums/?board=addons) – the pinned Addons Mega Thread lives here
- [Warperia – Project Epoch](https://warperia.com/server-addons/project-epoch/) – an Epoch-tagged addon category, with a desktop installer and update checker
- [Community wiki – AddOns](https://project-epoch-wow.fandom.com/wiki/AddOns) – community addon list, install notes and troubleshooting
- [GitHub search](https://github.com/search?q=project+epoch+addon&type=repositories&s=updated&o=desc) – most Epoch addons live in personal repos, sort by recently updated
- [NoM0Re/WoW-3.3.5a-Addons](https://github.com/NoM0Re/WoW-3.3.5a-Addons) – big pack of general 3.3.5a addons
- [Felbite](https://felbite.com/) – long-running WotLK addon archive
- [LegacyWoW](https://legacy-wow.com/wotlk-addons/) / [wowgaming addon archive](https://wowgaming.github.io/addon-archive/) – older 3.3.5 collections

### Epoch-specific

- [pfQuest Epoch](https://github.com/Bennylavaa/pfQuest-epoch) – quest and item data for Epoch, an extension that sits on top of pfQuest-wotlk. enUS clients only, and its author has stepped back, so forks carry it now
- [Questie for Epoch](https://github.com/NeticSoul/questie-335-epoch) – if you would rather keep Questie, this fork merges its quest database with pfQuest Epoch's
- [Zygor Guides Viewer](https://github.com/SimonGaufreteau/ZygorGuidesViewer) – 1-60 leveling guide ported to Epoch
- [What's Training? Epoch](https://github.com/ZythDr/Whats-Training-Epoch) – every spell your class learns, in a spellbook tab
- [Atlas Project Epoch](https://github.com/Raynbock/Atlas-Project-Epoch) / [AtlasLoot Project Epoch](https://github.com/Raynbock/AtlaslootProjectEpoch) / [AtlasQuest](https://github.com/Rofos2011/AtlasQuest) – maps and loot tables with Epoch content, AtlasQuest needs Atlas
- [DBM-epoch](https://warperia.com/addon/dbm-epoch/) – Deadly Boss Mods with Epoch encounters
- [Aux Epoch](https://warperia.com/addon/aux-epoch/) – Aux auction house addon, ported to run on Epoch
- [ConLogs-Epoch](https://github.com/Defcons/ConLogsApp) – embeds your gear, talents and position into the combat log, so one upload to Epog Logs carries everything
- [ElvUI-Epoch](https://github.com/Bennylavaa/ElvUI-Epoch) – ElvUI tuned for Epoch
- [pfUI Epoch](https://github.com/Fragglechen/pfui-epoch) – full interface replacement, Shagu's pfUI ported and adapted for Epoch
- [epoch-addons](https://github.com/wick3dr0se/epoch-addons) – ElvUI fork with paladin seal-twist and damage meter plugins
- [Defcons/epoch-addons](https://github.com/Defcons/epoch-addons) – community ports plus client bug fixes (EpochFixes, Aux, ArkInventory). Frozen since September 2026
- [EpochCN](https://github.com/z980944038-dev/EpochCN) – Chinese localization bundle: quests, UI, tooltips and map markers, with social tools for finding other Chinese-speaking players. Its `core` build wants `Data/patch-Z.MPQ` for the client's static text
- Kindrack's Epoch ports: [ModernMapMarkers](https://github.com/Kindrack/ModernMapMarkers-Epoch) (markers for dungeons, raids, world bosses, boats, zeppelins, trams and portals on the world map), [Talented](https://github.com/Kindrack/Talented-Epoch) (talent build manager for Epoch's TBC-style trees) and [Leatrix Plus](https://github.com/Kindrack/Leatrix_Plus) (the usual QoL suite, backported)

### Fine on any 3.3.5a

- [DragonUI](https://github.com/NeticSoul/DragonUI) – modular retail-style interface
- [Auctionator 3.3.5 fixed](https://github.com/thierbig/Auctionator-3.3.5-Fixed) – auction house with a working modern sell tab
- [ElvUI](https://github.com/ElvUI-WotLK/ElvUI) – the 3.3.5a build (Epoch's fork is listed above), with its plugins: [ProjectZidras](https://github.com/Zidras/ElvUI_ProjectZidras), [Enhanced](https://github.com/ElvUI-WotLK/ElvUI_Enhanced), [AddOnSkins](https://github.com/ElvUI-WotLK/ElvUI_AddOnSkins), [SwingBar](https://github.com/ElvUI-WotLK/ElvUI_SwingBar), [ExtraActionBars](https://github.com/ElvUI-WotLK/ElvUI_ExtraActionBars), [VisualProcs](https://github.com/ElvUI-WotLK/ElvUI_VisualProcs), [DmgAtNameplates](https://github.com/Bennylavaa/ElvUI_DmgAtNameplates)

### Install

Extract addon folders into `<client folder>/Interface/AddOns/`. The folder holding the `.toc` file has to sit directly inside `AddOns`.

- GitHub ZIPs add a suffix to the folder name (`pfQuest-epoch-main`). Rename it to match the addon (`pfQuest-epoch`), or the game will not load it.
- Restart the game rather than `/reload` when an addon is missing.
- Tick Load out of date AddOns on the character screen if an addon does not appear.
- `/reload` after UI changes and back up `Interface/` and `WTF/` now and then.

## Client enhancements

Optional patches and tools that change the client itself rather than adding to it.

### Asset packs

- [EpochAuthenticHD](https://github.com/thierbig/EpochAuthenticHD) – upscaled textures, HD character models, better trees, 4K zone maps, refreshed sounds and zone music, plus DXVK for Vulkan. Its README states it is kept up to date against the current Reborn client. MPQ files go in `Data/`, icons go in `Interface/`. Skip the HD spell and item icons if you want more FPS and delete `PATCH-E` if you prefer the original character models.
- [Patch-N_Epoch-Reborn](https://github.com/Kindrack/Patch-N_Epoch-Reborn) – a client patch for Reborn that ships map data for dungeon entrances, caverns and mines

### Injector

- [AwesomeEpoch](https://github.com/thierbig/AwesomeEpoch) – launches the client through an injector to add modern client features: stance and form dancing, the modern interaction button, `[@cursor]` macros, a see-through-walls camera, extra unit queries and a nameplate API that lets WeakAuras anchor reactive spells and castbars. Update through the launcher first, then run the game through this

### Renderers

Both replace water, fog and lighting, so pick one, never both. Neither targets Epoch.

- [Modern WoW Renderer](https://github.com/Corfirean/modern-wow-renderer) – a 32-bit `d3d9.dll` proxy adding dynamic lighting, volumetric fog, weather, reflective water and post-processing. It is developed and tested against the Ascension client, which its README says puts a stock 3.3.5 client outside the tested target. No Linux notes.
- [CoAVolFog](https://github.com/jealous-sound/coa-vfog) – a `version.dll` proxy adding volumetric fog, god rays and water with real wave simulation, for the Ascension/CoA client. It hooks the D3D9 call rather than replacing the DLL, so it is the one with a documented Linux route: set the game's Steam launch options to `WINEDLLOVERRIDES=version=n,b %command%`, tested on Steam Deck with Proton and DXVK.

### Making your own

- [Ladik's MPQ Editor](https://www.wowmodding.net/files/file/149-ladiks-mpq-editor/) opens and repacks client MPQs, [wow.export](https://github.com/Kruithne/wow.export) pulls models and textures out of them, [WMVx](https://github.com/Frostshake/WMVx) previews those models, and [WDBXEditor](https://github.com/WowDevTools/WDBXEditor) edits the client's DBC data. Epoch's own patches and most community mods are MPQ files, so these are the tools for looking inside them.

## Community

- [Fluxer chat](https://chat.project-epoch.org) – official, sign in with your game account
- [Fluxer – troubleshooting channel](https://chat.project-epoch.org/channels/1547040060984000512/1547040060984000543) – launcher, client and addon problems, ask here before you give up on it
- [WoWRetro Enhancements](https://discord.gg/QXA59eWUMj) – Discord for retro-server addon help, plus a [forum addon index](https://project-epoch.org/forums/?topic=101) maintained in their thread
- [r/wowservers](https://www.reddit.com/r/wowservers/) – player discussion and server news
- Creators who were posting Epoch content at launch: [SLiMOFI](https://www.youtube.com/@SLiMOFI), [Damonism](https://www.youtube.com/@Damonism), [Venario](https://www.youtube.com/@venarioo), [Malonze Gaming](https://www.youtube.com/@MalonzeGaming)
- [Community wiki](https://project-epoch-wow.fandom.com/wiki/Project_Epoch_Wiki) – addon list, install guides, data safety notes

## Tools

- [EpochDB](https://epochdb.net) – community-run Epoch database: NPCs and mobs, items, quests, loot tables, vendors, a talent calculator and raid timers, fed by its own data-collection [addon](https://github.com/MrBoxie88/EpochDB)
- [Epog Logs](https://epoglogs.com) – combat log uploads with DPS/HPS/tank rankings, target dummy parses, dungeon speedruns, progression tracking and every guild on the realm, plus an armory, gear compare, talents and simulators. Sign up with Discord
- [GitAddonsManager](https://woblight.gitlab.io/overview/gitaddonsmanager/) – install and update addons from GitHub or GitLab URLs, strips `-master`/`-main` suffixes for you
- [Warperia](https://warperia.com/) – web catalogue plus a desktop app that installs straight into `Interface/AddOns/` and checks for updates
- Realm status from the terminal: `curl https://project-epoch.org/api/realm-status`
- [WoW 3.3.5a addon wiki](https://github.com/NeticSoul/wow-335a-addon-wiki) – API, widget and pattern reference for this exact client build, for when an addon needs fixing rather than replacing

## Contributing

The project takes volunteers, no experience with the server required to start.

- Report bugs on the [bug tracker](https://project-epoch.org/bugs.html), with reproduction steps
- Apply as a game master, developer, content creator or tester through the forms on the [website](https://project-epoch.org/#forms)
- [Donate](https://project-epoch.org/donate.html) if you just want to cover running costs

Found something missing or wrong here? Open a pull request or an issue.

## Notes

- Disconnects, lag or a connection that never goes through: try Cloudflare WARP or another free VPN, which can fix or improve the routing. More in the [Connection/DC/Ping Issues?](https://project-epoch.org/forums/?topic=66) thread.
- The project does not distribute the game client and nothing legitimate ever needs your password except the site and client; no GM will ask for it in Fluxer or a DM.
- Back up your client before applying MPQ patches or injecting DLLs. The launcher re-downloads anything it manages, but it will not undo your own additions.
- Epoch ships its own `PATCH-D` and `PATCH-M`. HD asset packs that used those letters have to be renamed, EpochAuthenticHD moved its files up a letter (D→E, E→F, F→G, M→N) for exactly this reason.
- If an addon misbehaves after a server patch, check for an Epoch build before assuming it is broken.
