# Steam Games

## HITMAN World of Assassination
``%command% -USEALLAVAILABLECORES -force-vulkan --use-d3d11``
- Proton Hotfix!
- exclusive fullscreen for better fps

## Mass Effect Legendary Edition
``gamemoderun %command%``
- 7.0.6 to install ea
- experimental
- ge9-23
- runs exceptionally well stable no jitters no artifacts, 120 fps WOW

## Hellcard
``PROTON_USE_WINED3D=1 PROTON_NO_FSYNC=1 PROTON_NO_ESYNC=1 MESA_GL_VERSION_OVERRIDE=4.4 %command% -USEALLAVAILABLECORES``
- browse game files before first run and...
  - make sure that `registry_ccg.xml` contains the correct screen resolution
  - set `enable_game_analytics` in `ccg_custom_settings.txt` to 0

## Helldivers 2
``%command% -USEALLAVAILABLECORES -force-vulkan --use-d3d11``
- gamemoderun leads to game guard errors, won't even start with it
- ge 10-29
- ingame options:
  - disable cross play (prevent crashing loading into missions screens)
  - disable async compute in graphics settings
  - cap 30, uncapped will result in laggy mouse and your character walking slow motion

## Mechabellum
``gamemoderun %command%``
- Proton Experimental works perfectly
- GE does not work at all, game never finishes "Establishing connection to server..." at startup 
- lock fps @30, it will break down to single digit fps in later rounds anyway

## Sniper Elite: Resistance
``PULSE_LATENCY_MSEC=90 gamemoderun %command% -USEALLAVAILABLECORES``
- Proton 10.0.1
- disable efficiency cores or the performance will drop to from 40 to 15 fps within minutes of loading a game
- crackling audio only in cutscenes and kill cams, not in normal game
- fix with pulse buffer, the less the better (less lag) (I needed 90)
- `-USEALLAVAILABLECORES` gives 5 FPS boost (on 6 real cores without HT)

## Half Sword Demo / Playtest
``gamemoderun %command%``
- ge10-29

## Half Sword Early Access
``gamemoderun %command%``
- ge10-29
- Settings:
  - Everything on medium seems to run better than everything on Low
  - "DLSS: Ultra Performance" has no visual degradation and improves FPS by 10. Whatever it does on my Intel iGPU xD

## LEGO Star Wars
``PROTON_USE_WINED3D=1 PROTON_NO_ESYNC=1 PROTON_NO_FSYNC=1 gamemoderun %command%``
- Proton 7.0.6

## RoboCop: Rogue City
``PULSE_LATENCY_MSEC=30 gamemoderun %command% -USEALLAVAILABLECORES``
- ge10-8
- badly optimized, needs to run with xess on performance (allthough it's still really enjoyable!)

## GTA V Enhanced
``-nobattleeye`` 
- ge10-10
- singleplayer only, hassle-free out of the box. `gamemoderun` does not work.

## GTA V Legacy
``gamemoderun %command% -nobattleeye`` 
- ge10-11
- singleplayer only, hassle-free out of the box. Way better performance (and no drops / stuttering than Enhanced version)
 
## Escape from Duckov
``gamemoderun %command%``
- Proton Experimental

## next
``gamemoderun %command%``
- version
- review
