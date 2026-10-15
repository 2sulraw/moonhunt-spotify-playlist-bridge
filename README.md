# moonhunt-Spotify-playlist-bridge

A community addon for the MoonHunt download manager — paste a Spotify track,
playlist, or album link, match the songs on YouTube, and download them
individually or all at once into a group named after the playlist.

For legal safety reasons, this is built and distributed as an addon instead
of a built-in feature.

## Install

1. In MoonHunt, open the Addon page → **Add**.
2. Either **Install from URL** (paste the release `.zip` link below) or
   download the `.zip` and use **Choose .zip file**.
3. The playlist-bridge tab appears in the Addon sidebar.

## Use

Paste a Spotify link → **Resolve** → **Match** → download per song or
**Download all** (creates a Downloads group named after the playlist, with a
progress ring and Cancel while queueing). Failed matches show the reason on
the row — retry them individually.

Search modes (Match step): **Legacy** (sequential, recommended for restricted
networks), **2x**, **3x**, or **All** (everything at once — experimental, may
hit YouTube rate limits).

The Tracks header also has **Clear**: stops matching/queueing, cancels this
list's still-running downloads, and empties the list for a new search.

## Notes

- No Spotify account or API keys needed.
- If Spotify changes its page layout, playlist resolving may break until updated.
- Requires yt-dlp set up in MoonHunt (Media page) and a working YouTube
  connection. Restricted networks need the app's proxy configured.

## Files

- `manifest.json` — addon id, name, version, entry point, link patterns.
- `addon.js` — the whole addon: single ESM module, no build step.

## License

MIT — personal use at your own responsibility.
