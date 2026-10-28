<p align="center">
  <img width="200" alt="eth! logo" src="assets/eth.png">
</p>

<h1 align="center">eth!</h1>

<p align="center">
  A fully offline fork of osu!lazer: your own profiles, your own pp, an ethereal black &amp; white look.<br>
  <b>Beta.</b> Windows only.
</p>

<p align="center">
  <a href="https://github.com/nxtethereal/eth-releases/releases"><b>⬇ Download eth! for Windows</b></a>
</p>

---

eth! is osu!lazer reworked to run entirely on your own PC. You play, earn pp and track your progress locally. There's no account, no osu! servers, and nothing is submitted anywhere.

## Features

### Profiles and pp
- **Local profiles**, each with its own folder, profile picture and play history. Create, switch and delete them from the top right.
- **Three pp totals** in the toolbar: **Normal**, **Relax** and **Autopilot**.
  - Normal uses the official (bancho) formula.
  - Relax uses Akatsuki's relax formula.
  - Autopilot uses the standard formula with autopilot applied, as Akatsuki does.
- Each play's pp is **saved when you set it**, so totals stay consistent.
- An **Akatsuki-style profile page** with best plays, recent plays, grades, stats and a pp history graph.
- pp on the end screen and in local leaderboards, with sorting by pp.

### Gameplay
- **Custom speed rates** (DT/HT/NC/DC at any speed) count as ranked and give pp, as does **Mirror**.
- Star ratings for Relax and Autopilot match normal play.
- **Uncapped frame-rate** sliders for gameplay and menus.

### Beatmaps
- **osu!direct** built in, powered by public beatmap mirrors: search, filter by status, sort, preview and download (osu!standard).
- **Favourites** shared by every profile, with a star in song select.
- Song select starts sorted and grouped by difficulty.

### Look and feel
- A black & white **ethereal theme** with optional neon glow.
- A **black hole** menu background and the eth! **halo logo**.
- A **Customisation** tab for theme colours, the logo, the menu background, and your own **opening song** and volume.

### Updates
- eth! **updates itself** from this page. When a new version is out it asks: **Update now**, **See what's new**, or **Remind me later**, never mid-play.
- An **update indicator** on the toolbar, a **What's new** window after each update, and a toggle for automatic checks.

### Offline and private
- No global leaderboards, chat, multiplayer, news or links to the osu! website.
- The only internet use is osu!direct (beatmap mirrors) and checking this page for updates. See [Internet use](#internet-use) for the full list.

## Internet use

eth! works offline. It only goes online for the things below, and you can see the same list in the game under **Settings → General → Internet use**. Like any website, these services can see your IP address.

| When | What it talks to | What it sends |
|---|---|---|
| **osu!direct**, only while you search, browse or download | Search and beatmap pages: `api.nerinyan.moe` (fallback `catboy.best`)<br>Downloads: `api.nerinyan.moe`, then `catboy.best`, then `osu.direct`<br>Cover pictures: `assets.ppy.sh`<br>Song previews: `b.ppy.sh` | Your search text, filters and beatmap IDs |
| **Setup wizard**, only if you press "download beatmaps" | The same beatmap mirrors as osu!direct | Beatmap IDs |
| **Update checks**: on start and every 30 minutes (if automatic checks are on), or when you click check | GitHub: `api.github.com`, `github.com` and GitHub's download servers | A normal request for eth!'s latest release |
| **Update downloads**, only when you choose **Update now** | GitHub's download servers | Nothing beyond the download request |
| **Links you click** | Open in your browser, not in eth! (eth!'s GitHub release pages, the osu!lazer download page) | n/a |

**eth! never:** signs in or uses an account, submits scores, connects to osu! game servers, chat or multiplayer, sends analytics, telemetry or crash reports, or sets a Discord status. Your profiles, scores and settings never leave your PC.

## Install

1. Open the [latest release](https://github.com/nxtethereal/eth-releases/releases) and download **`eth-win-Setup.exe`**.
2. Run it and pick where to install. The recommended folder is filled in (`%LocalAppData%\eth`), or choose your own, like `C:\eth!`.
3. If Windows SmartScreen warns about an unrecognised app (the installer isn't code-signed yet), choose **More info → Run anyway**.

Your profiles, scores and settings live in `%APPDATA%\osu-offline`, so updating or reinstalling never touches them.

## Thank you, osu!lazer ♥

eth! exists because **peppy and the osu! team** made osu!lazer open source and support people who build on it. If you enjoy eth!, please support the real thing: [get osu!lazer](https://osu.ppy.sh/home/download).

---

<sub>eth! is not affiliated with, endorsed by or supported by ppy or Akatsuki. "osu!" is a trademark of ppy Pty Ltd. Based on osu!lazer (MIT licence); osu! resources are CC-BY-NC 4.0. Relax pp ported from akatsuki-pp-rs (MIT).</sub>
