# SpotifyKeeper

![SpotifyKeeper findet die gelikten Songs einer Playlist und überträgt sie in eine andere](assets/explainer.gif)

Überträgt die gelikten Songs einer Playlist in eine neue oder bestehende Playlist.

Läuft komplett im Browser (Spotify-Login per PKCE, kein Server, kein Client Secret).

Lässt sich als PWA installieren.

## Einrichtung

1. Im [Spotify Developer Dashboard](https://developer.spotify.com/dashboard) eine App mit Web API anlegen.
2. `https://oliver19xx.github.io/SpotifyKeeper/` als Redirect URI eintragen.
3. Seite öffnen, Client ID einfügen, anmelden.

## Einschränkung

Spotify gibt Songs nur aus eigenen und kollaborativen Playlists heraus. Fremde Playlists erst in der Spotify-App in eine eigene kopieren.
