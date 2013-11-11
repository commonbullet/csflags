#CS Flags



##Summary
CS Flags is a flag domintion plugin for Counter Strike 1.6 or Condition Zero; it's similar to dod, or UT domination mod - flags are fixed points to be checked by teams, the team that captures and keeps flags most wins. 
It’s supposed to be played with deathmatch (CSDM plugin) or other plugin that eventually respawns players in a round.


##Requirements
* Amxx 1.75 or above
* Flag models
* cfg files for maps you wish to play with cs flag
* sound files


##Installation:
* Plugin – place csflags.amxx on [amxx_installation_dir]/plugins folder; open [amxx_installation_dir]/config/plugins.ini file and write this line at the end of it: `csflags.amxx` 
* Editor - only required if you want to edit flag points; same as "Plugin" above with the csflags_editor.amxx.
* Models – place csflags.mdl in cstrike/models folder
* Config files – place them into [amxx_installation_dir]/configs/csflags; i.e. cstrike/addons/amxx/configs/csflags
* Sound files - place sound files into cstrike/sound/csflags directory

##CVARS:
* `amx_csflags_enabled` - 0: plugin disabled, 1: plugin enabled
* `amx_csflags_max_wins` – (default 3) max round wins limit ; if it’s 0 there’s no win limit
* `amx_csflags_max_points` – (default 100) determines how many points must be scored so a team wins a round
* `amx_csflags_tiematch` – (default 0)  if tie match is disabled (0), it will extend map time limit until a team wins the match *
* `amx_csflags_allflags_win` – (default 1) when it's enabled (1) a team may win a rounf if it captures all flags
* `amx_csflags_mapendtime` – (default 0.5) if a team wins a csflags match it will provide some extra time to vote, or to whatever is needed
* `amx_csflags_remove_map_obj` - (default 1) remove maps default objectives on load (defuse, rescue, etc.)
* `amx_csflags_capturefrags` - (default 0) number of frags to be added to a player who captures a flag
* `amx_csflags_winfrags` - (default 0) number of frags added to each player of the team that wins a round
* `amx_csflags_respawn` - (default 0) if it's set to 1, players are moved to each their team spawn points when a round is over
* `amx_csflags_capturedelay` - (default 3) time (seconds) required to capture a flag
* `amx_csflags_freeze` - (default 0) when a round is over, if it's set to 1,  players will freeze until next round starts
* `amx_csflags_vote_startcmd` - (default "") if you use a third part voting map system and it provides a command to start voting, it may be useful.
* `amx_csflags_useradio` - (default 1) if it's set to 1, the player who captures a flag sends a emulated radio message sound "Control point is secure".

\* map extending won’t work if mp_timelimit is set to 0 by default. Check if there aren’t other plugins messing with time; if you experience bugs, maybe you’d better set maxwins to 0 and and tiematch to 1.

##Commands
* `amx_csflags_stop` – stops current csflag match
* `amx_csflags_restart` – reset score and restart csflags match

##Editing flags:
* Install csflags_editor (requires csflag.mdl).
* Type in console csflags_edit to start it.

##CSFlags points included in package:

Cfg files included in this release:
cs_assault, cs_havana, cs_havana_cz, cs_italy, cs_italy_cz, cs_militia_cz, cs_office_cz, de_airstrip, de_airtrip_cz, de_aztec, de_aztec_cz, de_dust, 
de_dust_cz, de_dust2, de_dust2_cz, de_inferno, de_inferno_cz, de_train.

##Credits
Thanks to people that have helped me with amxx scripting (random order): bAnTAi, GHW\_Chronic, teame06, XxAvalanchexX, VEN, schnitzelmaker.

Thanks to all translators!
arkshine, Dav3, Deviance, fezh, Howdy, lucius, MmikiM, SAMURAI16, SeToY

Thanks to all people who have been helping me to improve the plugin by reporting issues or requesting features.

Special thanks to arkshine - much of the plugin features were based on his ideas, requests and suggestions.
