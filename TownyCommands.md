---
title: Towny Commands
feature_text: |
  ## Towny Commands
feature_image: "/assets/banner.png"
excerpt: "Use this page to look up a commnad for use with the TownyAdvanced plugin."
---

### /towny
  - /towny - Shows basic Towny commands
  - /towny ? - Additional Towny help
  - /towny map - Shows text-based map
  - /towny prices - Shows taxes/costs associated with running a town.
  - /towny time - Shows time until next new-day (tax/upkeep collection.)
  - /towny top {residents/land} - Shows top {residents/land owners}

### /plot (or /p)
  - /plot Shows the /plot commands.
  - **Claims**
    - /plot claim *\<mod\>* - Resident command to personally claims a plot that are for sale.
    - /plot claim auto - Resident command to personally claim an area of plots that are for sale, around the player typing the command.
    - /plot unclaim *\<mod\>* - Resident command to unclaim personally owned plots.
    - /plot {forsale/fs} *\<mod\>* *\<$$\>* - Set a plot for sale.
    - /plot {notforsale/nfs} *\<mod\>* - Set a plot to not be for sale.
      - *\<mod\>* use modifier **circle/rect** and quantifier **(1-4)** to set a shape and radius to apply the action to.
      - *\<$$\>* - Cost of plot.
    - /plot set *\<type\>* - set a plot to a certain type of plot
      - *\<type\>* -> shop/embassy/arena/wilds
  - /plot set reset - Sets a plot back to a normal plot.
  - /plot set name - allows a mayor or plot-owner to rename plots they own, overwriting the ~Unowned message. Personal-plots display both the plot's given name and the name of the plot-owner.
  - **Permissions**
    - /plot perm - Shows the permissions line of the plot in which the player stands.
    - **Set**
      - /plot set perm {on/off} - Edits the perm line of the single plot in which the player is standing. See here for details.
      - /plot set perm {resident/ally/outsider} {on/off}
      - /plot set perm {build/destroy/switch/itemuse} {on/off}
      - /plot set perm {resident/ally/outsider} {build/destroy/switch/itemuse} {on/off}
      - /plot set perm reset - Resets the plot in which you stand to the default perm line of the /town or /resident screen (depending on if the plot is owned personally or by the town.)
    - **Toggle**
      - /plot toggle fire - Turn on/off firespread in the plot in which you stand.
      - /plot toggle pvp - Turn on/off pvp in the plot in which you stand.
      - /plot toggle explosion - Turn on/off explosions in the plot in which you stand.
      - /plot toggle mob - Turn on/off hostile mobspawning in the plot in which you stand.
  - /plot clear - Command to remove list of block id's from a plot, used by a mayor on town-owned land, or by a plot-owner on their personal plots.

### /resident (or /res)
  - /resident - Shows a player their resident screen.
  - /resident ? - Shows /res commands available.
  - /resident {resident} - Shows a player another player's resident screen.
  - **Friends**
    - /resident friend add {resident} - Resident adds online player to their friends list.
    - /resident friend add+ {resident} - Resident adds offline player to their friends list.
    - /resident friend remove {resident} - Resident removes online player from their friends list.
    - /resident friend remove+ {resident} - Resident removes offline player from their friends list.
    - /resident friend clearlist - Removes all friends from a resident's friend list.
  - /resident list - Lists residents in towny's data folder.
  - /resident spawn - If player has a current bed spawn, command will teleport player to their bed.
  - **Chat Modes**
    - /resident toggle map - Turns on map which refreshes when moving across plot borders.
    - /resident toggle townclaim - Turns on mode where /town claim is automatically used when moving across plot borders.
    - /resident toggle plotborder - Turns on smokey plot-border view. Border shows when players cross to different townblocks.
    - /resident reset - This turns off all modes that are active.
  - **Permissions**
    - /resident set perm {on/off} - Edits the perm line on the resident screen. See here for details.
    - /resident set perm {friend/ally/outsider} {on/off}
    - /resident set perm {build/destroy/switch/itemuse} {on/off}
    - /resident set perm {friend/ally/outsider} {build/destroy/switch/itemuse} {on/off}
    - /resident set reset - This takes the perm line seen in the /resident screen and applies it to all plots personally owned by the player typing it.
  - /resident tax - Shows taxes a player pays.

### /town (or /t)
  - /town - Shows a player their town's town screen.
  - /town ? - Shows /town commands available.
  - /town {town} - Shows a player another town's town screen.
  - /town here - Shows you the town screen of the town in which you stand.
  - /town leave - Leaves a town.
  - /town list - Lists towns.
  - /town online - Shows players in your town which are online.
  - /town new {townname} - Creates new town.
  - /town add {resident} - Mayor command to add residents to your town.
  - /town kick {resident} - Mayor command to remove residents from your town.
  - /town spawn - Teleports you to your town's spawn.
  - /town spawn {town} - Teleports you to another town's spawn.
  - **Claims**
    - /town claim *\<mod\>* - Mayor command to claim the townblock in which you stand for your town.
    - /town claim auto - Claims as many townblocks around you as is possible given money in townbank and available townblocks.
    - /town unclaim *\<mod\>* - Mayor command to unclaim the townblock in which you stand.
    - /town unlaim all - Mayor command to unclaim all townblocks.
    - *\<mod\>* use modifier **circle/rect** and quantifier **(1-4)** to set a shape and radius to apply the action to.
    - /town claim outpost - Claims an outpost for your town.
  - /town withdraw {$} - Removes money from town bank.
  - /town deposit {$} - Adds money from player to the town bank.
  - /town outpost {# (where # equals the corresponding outpost's number)} - Teleports to an outpost.
  - /town ranklist - Displays residents and their ranks.
  - /town rank {add|remove} {playername} {rankname} - Grants or removes a rank to a resident of the town.
  - /town reslist - Displays a full list of residents in the town.
  - **Settings**
    - **Set**
      - /town set board {message} - Sets message seen by residents upon logging in.
      - /town set mayor {resident} - Mayor command to give mayor status to another resident.
      - /town set homeblock - Sets the homeblock and spawn of your town.
      - /town set spawn - Sets the town spawn, must be done inside the homeblock.
      - /town set name {name} - Change your town's name.
      - /town set outpost - Sets a townblock as an outpost.
      - **Permissions**
        - /town set perm {on/off}
        - /town set perm {resident/ally/outsider} {on/off}
        - /town set perm {build/destroy/switch/itemuse} {on/off}
        - /town set perm {resident/ally/outsider} {build/destroy/switch/itemuse} {on/off}
        - /town set perm reset - This takes the perm line seen in the /town screen and applies it to all plots owned by the town.
        - /town toggle fire - Turn on/off firespread in your town.
        - /town toggle pvp - Turn on/off pvp in your town.
        - /town toggle explosion - Turn on/off explosions in your town.
        - /town toggle mob - Turn on/off hostile mobspawning in your town.
      - /town set tag {upto4character} - Sets the town's tag, which is sometimes used on that chat line.
      - /town set tag clear - Clears the tag set for the town.
      - /town set taxes {$} - Sets taxes collected from each resident daily. Also sets percentage if taxpercent is toggled on.
      - /town set plottax {$} - Set taxes collected from each resident daily, per plot that they own.
      - /town set plotprice {$} - Sets default cost of plot for the town.
      - /town set shopprice {$} - Sets default cost of a shopplot for the town.
      - /town set shoptax {$} - Set taxes collected from each resident daily, per shopplot that they own.
      - /town set embassyprice {$} - Sets default cost of a embassy plot for the town.
      - /town set embassytax {$} - Set taxes collected from each resident daily, per embassy plot that they own.
    - **Toggle**
      - /town toggle explosion - Turn on/off explosions in town.
      - /town toggle fire - Turn on/off firespread in town.
      - /town toggle mobs - Turn on/off hostile mobspawning in town.
      - /town toggle public - Turn on/off public /town spawning and the co-ordinates of the town's homeblock in the /town screen.
      - /town toggle pvp - Turn on/off pvp in town.
      - /town toggle taxpercent - Turn on/off taxing by percent/flatrate.
      - /town toggle open - Turn on/off public joining to your town.
  - /town join {townname} - Command to join a town that doesn't require invites.

### /nation (or /n)
  - /nation - Shows a player their nation's nation screen.
  - /nation ? - Shows /nation commands.
  - /nation list - Lists nations.
  - /nation online - Shows players in your nation which are online.
  - /nation {nation} - Shows a player the /nation screen of another nation.
  - /nation leave - Mayor command to leave the nation they are a part of.
  - /nation withdraw {$} - King command to remove money from the nation bank.
  - /nation deposit {$} - King command to add money to the nation bank.
  - /nation new {nationname} - Mayor command to create a nation.
  - /nation rank - Command to set assistant/custom ranks in the nation.
  - /nation add {town} .. {town} - Invites/Adds a town to your nation.
  - /nation kick {town} .. {town} - Removes a town from your nation.
  - /nation delete {nation} - Deletes your nation.
  - /nation ally add {nation} - Add a nation to your nation's ally list.
  - /nation ally remove {nation} - Removes a nation from your nation's ally list.
  - /nation enemy add {nation} - Add a nation to your nation's enemy list.
  - /nation enemy remove {nation} - Removes a nation from your nation's enemy list.
  - /nation rank {add|remove} {playername} {rankname} - Grants or removes a rank to a resident of the nation.
  - **Set**
    - /nation set king {resident} - King command to change the king of the nation.
    - /nation set captial {town} - Sets the capitol and king of the nation.
    - /nation settaxes {$} - Sets nationtax applied to the towns within the nation.
    - /nation setname {name} - Sets the nation's name.
    - /nation settitle {name} {titlegoeshere} - King command to add a Title to a member of the nation.
    - /nation set surname {name} {surnamegoeshere} - King command to add a Suffix to a member of the nation.
    - /nation set tag {upto4character} - Sets the nation's tag, which is sometimes used on that chat line.
    - /nation set clear - Clears the tag set for the nation.
  - /nation toggle neutral - Sets whether your nation will pay daily to be neutral during towny war.
  
  ### Chat commands
  - /townchat, /tc - Put in from of text to speak with members of your town only, or without text afterwards to enter the channel.
  - /nationchat, /nc - Put in from of text to speak with members of your nation only, or without text afterwards to enter the channel.
  - /global, /g - Put in from of text to speak in globalchat, or without text afterwards to enter the channel.
  - /res set mode reset - Reset chat mode to default chat.

  - /channel leave|join {channel} - Channel leaving and joining.
  - /leave {channel} - Leaves a channel.
  - /join {channel} - Joins a channel.
  - /chmute {channel} {player} - Mutes a player in a channel.
  - /mutelist {channel} - Displays mute list for a channel.
  - /chunmute {channel} {player} - Unmutes a player in a channel.
