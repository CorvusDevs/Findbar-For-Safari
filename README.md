# Findbar For Safari

Type a keyword in Safari's address bar, jump anywhere.

Findbar turns Safari's address bar into a power-user launcher:

- **30+ built-in shortcuts:** `g foo` → Google, `gh user/repo` → GitHub, `w foo` → Wikipedia, `so foo` → Stack Overflow, and more
- **Edit every keyword.** Add your own, change the defaults, or remove what you don't use
- **Multi-tab chaining.** `!g foo !w bar` opens Google in the current tab and Wikipedia in a new one
- **Regex keywords.** Pattern-matched shortcuts like `gh/(\S+)/(\S+)` for issue / PR / repo navigation
- **URL rewriting** *(optional, off by default)*. Silently redirect `twitter.com` → `nitter`, `reddit.com` → `old.reddit`, and other privacy-friendly frontends

Findbar is a native Safari Web Extension for macOS, iOS, and iPadOS. No tracking, no telemetry, no account required. Available on the App Store.

## How it works

Safari doesn't expose its address bar to extensions directly — there is no "omnibox" API on Safari the way Chrome has. Findbar catches your search the moment Safari starts navigating to your default engine, parses the query, and rewrites the navigation to your keyword's target. For Findbar's built-in keywords this happens via `declarativeNetRequest` and produces no visible flash; for user-added keywords there is a brief flash of the default engine before redirect. This is a Safari limitation, not something Findbar can work around.

## Privacy

Findbar runs entirely on-device. Your keyword list never leaves your Mac/iPhone/iPad — there is no cloud, no account, no analytics endpoint. The full [privacy policy](https://corvusdevs.com/findbar/privacy) is on the project page.

## Support

Bug reports and feature requests: [open an issue](https://github.com/CorvusDevs/Findbar-For-Safari/issues) on this repo.

## Built by CorvusDevs

Findbar is part of the [CorvusDevs](https://corvusdevs.com) family of Safari power-user extensions, alongside [Corvus RSS Reader](https://github.com/CorvusDevs/Corvus-RSS-Reader-For-Safari), [Purple Crow](https://github.com/CorvusDevs/Purple-Crow-For-Safari), [Alien Crow](https://github.com/CorvusDevs/Alien-Crow-For-Safari), and others.
