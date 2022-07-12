# Cvar list

<br>

> #### The following conventions are used to describe argument types:
> `string` - normal text characters  
> `integer` - whole numbers variable, e.g. 1, 2, 3, 4  
> `float` - floating point value variable, e.g. 1.0, 0.9, 0.8, 0.7  
> `bitflag` - binary digit whole value variable, e.g. 1, 2, 4, 8, 16, etc (or add 1+2 = 3, 1+2+4 = 7, etc)  

> #### Cvar color table  
`white` `red` `green` `blue` `yellow` `magenta` `cyan` `orange` `mdred` `mdgreen` `dkgreen` `mdcyan` `mdyellow` `mdorange` `mdblue` `ltgrey` `mdgrey` `dkgrey` `black`  

# Commands
| Command | Example | Description |
|---------|---------|-------------|
| minimize | `/minimize` | Minimize the game |
| +stats | `/bind X +stats` | Show stats window |
| -stats | `/bind X -stats` | Hide stats window |
| +vstr | `/bind X +vstr "commandA commandB"` | Bind commandA to key press and commandB to key release |
| cycle | `/bind X "cycle cg_drawcrosshair 0 10 1"` | Cycle through cvar values. |

# Cvars
# Client  
#### Engine/renderer (cl/r)
| Cvar | Argument type | Value range | Default | Description |
|---------|---------------|-------------|---------|-------------|
| cl_master | `string` | `N/A` | `wolfmaster.idsoftware.com` | Master server list |
| cl_httpDomain | `string` | `N/A` | `www.rtcw.life` | Domain to redirect to for map downloads |
| cl_httpPath | `string` | `N/A` | `/files/mapdb` | Path to the file database of the domain to redirect to |
| in_mouse | `integer` | `0-2`| `1` | Switch mouse input type between default and raw `(2)` |
| con_height | `float` | `0.1-1.0` | `0.5` | Change console height |
| con_type | `integer` | `0-1` | `0` | Enable/disable con_color |
| con_colorRed | `float` | `0.0-1.0` | `0.5` | Change console color in the red range |
| con_colorGreen | `float` | `0.0-1.0` | `0.5` | Change console color in the green range |
| con_colorBlue | `float` | `0.0-1.0` | `0.5` | Change console color in the blue range |
| con_colorAlpha | `float` | `0.0-1.0` | `1` | Change console color opacity |
| r_debugImages | `integer` | `0-1` | `0` | Texture debug information |

#### Mod (cg)
| Cvar | Argument type | Value range | Default | Description |
|---------|---------------|-------------|---------|-------------|
| cg_drawSpectatorState | `integer` | `0-1` | `1` | Draw "SPECTATOR" state |
| cg_drawClock | `integer` | `0-1` | `1` | Draw local time |
| cg_autoAction | `bitflag` | `0-3` | `0` | Auto actions. `1` - take screenshot, `2` - record demo, `3` - both |
| cg_useScreenshotJPEG | `integer` | `0-1` | `1` | Use JPEG for auto action screenshots |
| cg_altScoreboard | `integer` | `0-2` | `0` | Draw alternative scoreboard. `1` - default font, `2` - new font |
| cg_altScoreboardColor | `string` | `N/A` | `default` | Alternative scoreboard color |
| cg_altScoreboardAlpha | `float` | `0.0-1.0` | `0.6` | Alternative scoreboard opacity (alt color should not be default) |
| cg_drawFlags | `integer` | `0-1` | `0` | Draw country flags on all scoreboards |
| cg_drawMotd | `integer` | `0-1` | `0` | Draw server message of the day on top of all scoreboards |
| cg_chatY | `integer` | `N/A` | `385` | Chat position in the vertical axis |
| cg_notifyTextY | `integer` | `N/A` | `42` | Kill feed position in the vertical axis |
| cg_chatAlpha | `float` | `0.0-1.0` | `0.33` | Chat opacity |
| cg_chatBackgroundColor | `string` | `N/A` | `""` | Chat background color |
| cg_chatBeep | `bitflag` | `0-3` | `0` | Chat notification sounds. `1` - global chat only, `2` - team chat only, `3` - both |
| cg_statsWindowX | `integer` | `N/A` | `5` | /+stats window position in the horizontal axis |
| cg_statsWindowY | `integer` | `N/A` | `200` | /+stats window position in the vertical axis |
| cg_hitsounds | `bitflag` | `0-7` | `0` | Enable hitsounds. `1` - head only, `2` - body only, `4` - team only |
| cg_hitsoundBodyStyle | `integer` | `0-5` | `1` | Change body hitsound |
| cg_hitsoundHeadStyle | `integer` | `0-9` | `1` | Change head hitsound |
| cg_spectatorSpeed | `integer` | `0-8000` | `0` | Spectator free cam speed |
