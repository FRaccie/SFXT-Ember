# SFxT Ember Netplay

Rollback netplay and online rooms for **Street Fighter X Tekken** (Steam, PC). 1v1.

This repository only hosts the downloads. **Test builds:** they can crash or desync. Crash reports are sent
automatically (see [Reports](#reports)).

## Download

Get the latest build from [Releases](../../releases):

- **Nightly** (pre-release): the newest test build, rebuilt with each change. A nightly plays online for 7 days after
  it was built; after that, download the latest one.
- `sfxt-ember-<version>-setup.exe`: the installer (recommended).
- `sfxt-ember-<version>.zip`: the same files, to extract yourself.
- `sfxt-ember-<version>-SHA256SUMS.txt`: checksums of both.

## Install

**Installer:** run the setup. It installs into its own folder (no administrator needed) and adds
"SFxT Ember Netplay" to the Start menu. Nothing is put in the game's folder.

**Zip:** extract every file into a folder of your own (not the game's folder) and start `sfxt-ember-launcher.exe`.

The launcher finds the game through Steam. If it does not, start it with the game's folder:

```
sfxt-ember-launcher.exe --game "D:\SteamLibrary\steamapps\common\Street Fighter X Tekken"
```

Both players need the same game files: the Steam version as Steam installs it, or both the same patched copy. The room
tells you when the other player's files differ.

Antivirus programs can flag unsigned mods. If the game will not start, add an exception for Ember's folder.

## Play

Start **SFxT Ember Netplay** (the launcher) with Steam running; it starts the game. Starting the game from Steam
starts it without Ember. **F10** opens and closes the room screen.

| | |
|---|---|
| Host a room | Your room's code goes on screen; "Copy code" puts it on your clipboard. Send it to the player you want to play. A host can list the room publicly. |
| Browse rooms | The public rooms; pick one to join. |
| Paste code and join | Copy a host's code, then press this. |
| Ready | Pick your team (point and partner, costume, colour), then Ready. When both players are ready, the match starts by itself. |

## Your files

Your logs are in `%APPDATA%\sfxt` (type that in Explorer's address bar). Include `sfxt.log` when you report a problem.

## Reports

When the game crashes, a crash report (a minidump of the game's memory and `sfxt.log`) is sent to the developers'
error tracker. Problems such as a desync are reported too. To turn reports off, create an empty file named
`sfxt-ember-no-reports.txt` in `%APPDATA%\sfxt`.

## Uninstall

**Installer:** uninstall "SFxT Ember Netplay" from Windows' Apps & features.
**Zip:** delete its folder. `%APPDATA%\sfxt` holds your logs; delete it too if you want them gone.

---

Street Fighter X Tekken is © CAPCOM. TEKKEN is © Bandai Namco Entertainment. This project is not affiliated with or
endorsed by either.
