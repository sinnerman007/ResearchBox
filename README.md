# ResearchBox

**GitHub description:** A lightweight research launcher that turns one query into organized, category-specific searches across the web.

ResearchBox is a browser-based research workspace. Enter a query, choose a research lens, and get a curated set of source cards with tailored searches. Open sources in separate tabs, keep notes, and save sessions in your browser.

## Features

- Search modes for **Person**, **Place**, **Thing**, and **Not sure**. Not sure uses a lightweight local classifier and keeps ambiguous queries broad.
- A configurable source registry with category-specific query generation.
- Search cards for web, images, Wikipedia, YouTube, Reddit, news, maps, social and professional sites, shopping, travel, and academic sources.
- Select or deselect sources, open selected searches, copy generated queries, and add per-source notes.
- Related search suggestions and session notes.
- Local search history and saved research sessions.
- Dark and light themes, responsive layouts, and settings for default category, safe search, and source count.
- No account, server, API key, database, or build step required.

## Run it

Open `index.html` in a modern browser. The app is self-contained and runs locally.

To publish it with GitHub Pages, place `index.html` at the repository root, then enable Pages for the branch and folder containing the file.

## Privacy and search behavior

ResearchBox stores history, settings, saved sessions, and notes in the browser's `localStorage` on the current device. It does not send this data to a ResearchBox server.

Searches open on the selected external websites. ResearchBox does not embed third-party pages, scrape websites, or display live results inside the app. Your query is sent to an external provider only when you open that provider's search.

Some browsers may block multiple tabs opened at once. If **Open selected** is blocked, allow pop-ups for the page and try again.

## Customization

The source registry and category-specific query and URL builders live in the script near the top of `index.html`. Add or update a source there to make it available to the relevant categories. No API integration is required for external search links.

## Limitations

- Search results and provider availability are controlled by external websites.
- The local classifier is heuristic and may not infer the intended category. Choose a category directly when the distinction matters.
- Local data is tied to the browser and device; clearing site data removes it.
- Safe search is applied to supported Google web and image searches. Other providers use their own settings.

## License

No license is specified. Add a `LICENSE` file before redistributing this project under a particular license.
