# SpotifyKeeper

![SpotifyKeeper findet die gelikten Songs einer Playlist und überträgt sie in eine andere](assets/explainer.gif)

Überträgt die gelikten Songs einer oder mehrerer Playlists in eine neue oder bestehende Playlist.

Läuft komplett im Browser (Spotify-Login per PKCE, kein Server, kein Client Secret).

Lässt sich als PWA installieren.

Jede Übertragung landet in einer Sync-Liste. „Alle synchronisieren“ holt neue Likes in die gewählten Ziele und entfernt zurückgenommene. Entfernt werden nur Songs, die die App selbst ins Ziel gelegt hat. Die Liste liegt im Browser, also pro Gerät.

## Einrichtung

1. Im [Spotify Developer Dashboard](https://developer.spotify.com/dashboard) eine App mit Web API anlegen.
2. `https://oliver19xx.github.io/SpotifyKeeper/` als Redirect URI eintragen.
3. Seite öffnen, Client ID einfügen, anmelden.

## Einschränkung

Spotify gibt Songs nur aus eigenen und kollaborativen Playlists heraus. Fremde Playlists erst in der Spotify-App in eine eigene kopieren.

## Release

In `index.html` `APP_VERSION` erhöhen und `CHANGELOG` ergänzen, in `sw.js` `CACHE` anpassen. Nutzer sehen den Changelog beim nächsten Start automatisch.
