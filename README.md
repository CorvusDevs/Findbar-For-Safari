<div align="center">
  <img src="https://corvusdevs.github.io/Findbar-For-Safari/icon.png" width="128" height="128" alt="Findbar icon">
  <h1>Findbar for Safari</h1>
  <p><strong>Type a keyword in Safari's address bar, jump anywhere</strong></p>
  <p>
    <a href="https://apps.apple.com/app/findbar-for-safari/">
      <img src="https://img.shields.io/badge/Coming_soon_to_the-App_Store-2563EB?style=for-the-badge&logo=app-store&logoColor=white" alt="Coming soon to the App Store">
    </a>
  </p>
  <p>
    <img src="https://img.shields.io/badge/macOS-14.0+-000000?style=flat-square&logo=apple&logoColor=white" alt="macOS 14.0+">
    <img src="https://img.shields.io/badge/iOS-17.0+-000000?style=flat-square&logo=apple&logoColor=white" alt="iOS 17.0+">
    <img src="https://img.shields.io/badge/iPadOS-17.0+-000000?style=flat-square&logo=apple&logoColor=white" alt="iPadOS 17.0+">
    <img src="https://img.shields.io/badge/Languages-33-4CAF50?style=flat-square" alt="33 Languages">
  </p>
  <p>
    <a href="https://corvusdevs.github.io/Findbar-For-Safari/">Website</a>
  </p>
</div>

---

Findbar turns Safari's address bar into a power-user launcher. Type `g foo` for Google, `gh user/repo` for GitHub, `w foo` for Wikipedia — and 27 more shortcuts you can edit, plus bang chaining, regex keywords, and optional URL rewriting. Findbar is not a Chrome extension ported to Safari. It's built specifically for Safari with native performance, no background processes, and zero data collection.

## Features

- **30 built-in keywords** — `g`, `d`, `b` for search engines; `w`, `mdn`, `ad` for references; `gh`, `so` for code; `y`, `spo`, `n` for media; `r`, `hn`, `tw`, `bs` for social; `m`, `maps` for maps; `npm`, `cargo`, `pip`, `brew` for package managers, and more.
- **Edit every keyword** — Change the trigger, URL template, default URL, or aliases. Add your own. Soft-delete with a 20-entry trash bin for recovery.
- **Bang chaining** — `!g foo !w bar` opens Google in the current tab and Wikipedia in a new one. Configurable separator.
- **Regex keywords** — Pattern-matched shortcuts like `gh/(\S+)/(\S+)` → `https://github.com/$1/$2` for issue / PR / repo navigation.
- **URL rewriting** *(optional, off by default)* — Curated rules to silently redirect Twitter → Nitter, Reddit → old.reddit, YouTube → Piped, and more privacy-friendly frontends. All toggleable, all editable.
- **Live validation** — As you type a keyword or rewrite rule, friendly errors appear inline: missing URL protocol, invalid regex, capture-group mismatches, conflicting triggers.
- **In-app language picker** — 33 languages with flag icons + native names. Defaults to your system locale; switch anytime from the picker in the top-right.
- **What's New on update** — First launch after an update shows a sheet listing what changed; "NEW" pills mark recently-added settings rows.
- **DNR fast path** — Built-in keywords compile to Safari's `declarativeNetRequest` rules for zero visible-flash interception. User-added and regex keywords use a JavaScript fallback (brief default-engine flash before redirect — a Safari platform limitation, not a Findbar bug).
- **Multi-platform** — Native Safari Web Extension for macOS, iOS, and iPadOS. Same settings sync via iCloud if you sign in to Safari.

## Privacy

No account required. No sign-ups, no cloud sync, no tracking, no analytics. Your keyword list, rewrite rules, and preferences live entirely on your device. Findbar collects zero data. See the [full privacy policy](https://corvusdevs.github.io/Findbar-For-Safari/privacy.html).

## How it works

Safari does not expose its address bar to extensions directly — there is no `omnibox` API on Safari the way Chrome and Firefox have. Findbar catches your navigation the moment Safari starts loading the default search-engine URL, extracts the typed query, and rewrites the navigation to your keyword's target. For built-in keywords this happens via `declarativeNetRequest` (no visible flash); for user-added and regex keywords there is a brief flash of the default engine before redirect. The "Search [engine]" hint that appears in the URL bar while typing is Safari's default behavior for any unrecognized text — every keyword-search extension on Safari behaves the same way.

## More from CorvusDevs

| | App | Description |
|---|-----|-------------|
| <img src="https://corvusdevs.github.io/icons/red-crow.png" width="32"> | [Red Crow for Safari](https://corvusdevs.github.io/Red-Crow-For-Safari/) | YouTube enhancement with 40+ features |
| <img src="https://corvusdevs.github.io/icons/purple-crow.png" width="32"> | [Purple Crow for Safari](https://corvusdevs.github.io/Purple-Crow-For-Safari/) | BTTV, FFZ & 7TV emotes plus 50+ Twitch features |
| <img src="https://corvusdevs.github.io/icons/corvus-rss.png" width="32"> | [Corvus RSS Reader for Safari](https://corvusdevs.github.io/Corvus-RSS-Reader-For-Safari/) | Privacy-first RSS and Atom feed reader for Safari |
| <img src="https://corvusdevs.github.io/icons/auto-mute-tab.png" width="32"> | [Auto Mute Tab for Safari](https://corvusdevs.github.io/Auto-Mute-Tab-For-Safari/) | Automatically mute background tabs in Safari |
| <img src="https://corvusdevs.github.io/icons/ekual.png" width="32"> | [Ekual](https://corvusdevs.github.io/Ekual/) | Automatic loudness equalization for macOS |
| <img src="https://corvusdevs.github.io/icons/tekla.png" width="32"> | [Tekla](https://corvusdevs.github.io/Tekla/) | Swipe-to-type virtual keyboard for macOS |

---

<div align="center">
  <sub>Made with care by <a href="https://corvusdevs.github.io">CorvusDevs</a></sub>
</div>
