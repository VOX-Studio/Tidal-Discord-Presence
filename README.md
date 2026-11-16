TIDAL Discord Presence
======================

Display what you are listening to on TIDAL on your Discord profile
("Listening to TIDAL," track title, artist, album art, progress bar).

Prerequisites
- Windows 10 or 11
- The TIDAL desktop app (not the website)
- The Discord desktop app (must be open)
- Discord > Settings > Activity Privacy > "Share my activity" enabled

Installation
1. Move `TidalDiscordPresence.exe` to a permanent folder
   (e.g., Documents). Do not leave it in your Downloads folder if you
   choose to enable automatic startup.
2. Double-click the file.
   Windows may display a "Windows protected your PC" message because
   the program is not digitally signed. Click "More info," then select
   "Run anyway."
3. A window will appear, offering the option to launch the program
   automatically when Windows starts.
4. Play a track on TIDAL: your status will appear on Discord within
   a few seconds. It will disappear when you pause playback.

The program runs in the background (no visible window).
- To stop it: Task Manager > TidalDiscordPresence > End task
- To remove it from startup: Task Manager > Startup apps
- Settings and logs: `%APPDATA%\TidalDiscordPresence`
  (see `config.json` and `tidal_presence.log`)

To display album art, the track title and artist are sent to
Deezer's public API. To disable this feature, set `"fetch_cover": false`
in `config.json` and restart the program.