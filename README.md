# Cerberus Launcher

<img src="docs/icon-512.png" width="160" alt="Cerberus Launcher icon">

**Version 0.3.2 (beta).** A lean Android phone home screen from Onknight Studios. Portrait, bottom dock, swipe-up app drawer with search, and widgets you can drag around. Written natively in Java with no third-party libraries. It is the phone companion to Onknight Launcher for Android TV, and a separate app.

## Features (0.3.2)
- **News feed.** From the first home page, swipe right to pull in your news screen from the left. A large lead story with its photo, then headlines with thumbnails, source, time and a short summary from RSS feeds you choose; tap a story to read it in your browser. Tap **Feeds** to add, rename or remove feeds (paste a website or feed address; the app finds the feed and checks it before saving), or **Refresh** to reload. Back, Home or a swipe left returns to the launcher. Everything is local: no accounts, no subscriptions. Starting feeds: CBC Toronto, CBC Technology, CBC Sports, Sportsnet, CBS Sports NFL, MobileSyrup, TWiT News.
- **Scrolling dock.** Up to 20 apps; scroll the dock sideways when they don't all fit. The all-apps button stays pinned at the end.

## Also in 0.2
- **Home pages.** Swipe sideways between pages. Tap the **+** above the dock to add a page. Hold a block against the left or right screen edge while dragging to carry it to the next page; it makes a new page if you're on the last one. Hold empty space > Remove this page. Up to 9 pages.
- **Hosts real Android widgets.** Hold empty space > Add widget. Symfonium's music widget is listed first. Android asks once to allow the launcher to show widgets.
- **Drag and drop.** Hold any block to move it. In edit mode, drag the bottom-right handle to resize, tap the top-right X to remove, tap outside to finish.
- **Built-in blocks.** Clock and weather (icons drawn in code, Celsius or Fahrenheit by country, automatic location or "Set my city"). Text and the forecast scale with the block size.
- **Dock.** Up to 6 apps plus an all-apps button. Defaults to phone, messages, browser, camera and Symfonium if found. Hold an app to add or remove it.
- **App drawer.** Swipe up (or tap the dots). Search as you type, Enter launches the first match. Hold an app for Add to dock, App info or Uninstall.
- **Wallpaper.** Cerberus artwork by default, or choose any photo. Shows the whole picture with a soft blurred fill around it; switch to "Fill the screen" in the Wallpaper menu to crop instead.
- **Home app.** Menu > Set as home app (uses Android's own prompt).

## Install
Download the APK from the [Releases](../../releases) page (or the latest build under Actions > Artifacts) and sideload it, or build it yourself with Android Studio (Build > Build APK). It uses the QUERY_ALL_PACKAGES permission to list your apps, so it is meant for sideloading rather than the Play Store.

## Version history
- **0.3.2 beta** - Add feed now accepts a normal website address and finds its RSS feed for you (the page's advertised feed link first, then common spots like /feed and /rss).
- **0.3.1 beta** - Prettier news feed: a large lead-story card with its picture, thumbnails on every story that has one, date header, softer cards and type.
- **0.3 beta** - Swipe-right-from-page-1 RSS news feed with editable feeds. Dock holds up to 20 apps and scrolls.
- **0.2 beta** - Multiple home pages (swipe, + button, page dots, drag a block to the edge to move it to another page). Wallpaper no longer zoomed in: whole picture with blurred fill, plus a Fill option.
- **0.1 beta** - First phone release.

## Known limits in 0.3.2
- Portrait only.
- Some widgets cannot be resized smaller than their minimum and may clip.
- Swiping up over a scrolling widget can open the drawer; use the dots button if that gets in the way.
- Dock reordering by drag is not in yet.
- Google Discover is not supported (Google only allows it through companion apps that can break with Google app updates); the RSS feed is the news screen.
- Some sites change or remove their RSS addresses. If a feed stops loading, the news screen says which one.
- No app icons on home pages yet (widgets, clock and weather only).

## Building
- Android Studio: open the project folder and press Run. (Android Studio creates the Gradle wrapper for you on first sync.)
- GitHub: every push builds a debug APK (Actions tab). Push a tag such as `v0.3.2` and the APK is attached to a new release automatically.
- Stack: native Java, no third-party libraries. AGP 8.7.3, Gradle 8.9, compileSdk 35, targetSdk 33, minSdk 26.

## Notes
- Cerberus artwork (wallpaper and icon) is by Tom and is included for this project.
- Onknight Studios. Phone companion to Onknight Launcher (TV).
