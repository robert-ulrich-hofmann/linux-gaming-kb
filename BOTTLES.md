Soldier of Fortune

    archive.org installer
    environment variable MESA_EXTENSION_MAX_YEAR=2000
    Windows XP
    turn off all features
    soda 9.0.1
    todo: turn cue+bin into iso
    iso as folder in bottle
    setup
    best settings?

Sims All Expansions

    archive.org installer

Battle.NET

Switching from / to any Proton runner to any "normal" Wine runner changes your user and and home directory in the Windows context. (Windows user "steamuser" vs "your-linux-username"). After doing that some games can not access their user settings / files anymore (so far I have seen it with StarCraft II and HOTS), which leads to the "Core: access permission error" error.
You need to delete the games and all their config files and reinstall them.

For the `Variables.txt` file to be present you have to start the game once.

Battle.NET / Hots

- Add to `C:\users\YOURUSER\Documents\Heroes of the Stom\Variables.txt`
  ```
  frameratecap=40
  frameratecapGlue=30
  ```
  where `frameratecap` is the fps limit during gaming (focus on application) and `frameratecapGlue` is the fps limit while minimized / out of focus / in certain menus. In HOTS this is, sadly, also concerning the animations in champ select.

Battle.NET / StarCraft II

- Play the game in DX9 (instead of default DX11) for way better performance at same visual quality by adding `--renderer=dx9` as additional command line option in Battle.NET client 
- Add to `C:\users\YOURUSER\Documents\StarCraft II\Variables.txt`
  ```
  frameratecap=40
  frameratecapGlue=12
  ```
  where `frameratecap` is the fps limit during gaming (focus on application) and `frameratecapGlue` is the fps limit while minimized / out of focus / in certain menus.
