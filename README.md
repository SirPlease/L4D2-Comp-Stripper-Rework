# L4D2 Competitive Stripper Rework
#### Version: v0-dev
#### Released: N/A

## Important Links
### [Map Changes Documentation](https://github.com/Derpduck/L4D2-Comp-Stripper-Rework/wiki/Map-Changes)
#### [Wiki](https://github.com/Derpduck/L4D2-Comp-Stripper-Rework/wiki) - Documentation / Guides
#### [Releases](https://github.com/Derpduck/L4D2-Comp-Stripper-Rework/releases)
#### [Patch Notes](https://github.com/Derpduck/L4D2-Comp-Stripper-Rework/blob/master/CHANGELOG.md) - Patch notes for each release version
#### [Development Branch](https://github.com/Derpduck/L4D2-Comp-Stripper-Rework/tree/dev) - See changes currently under development
#### [Issues](https://github.com/Derpduck/L4D2-Comp-Stripper-Rework/issues) - Bug Reports / Feature Requests / Suggestions
#### [Projects](https://github.com/Derpduck/L4D2-Comp-Stripper-Rework/projects) - See what's being worked on!
#### [Templates](https://github.com/Derpduck/L4D2-Comp-Stripper-Rework/tree/master/_Templates)

## About The Project
This repository is for reworking the Stripper:Source map changes for competitive L4D2 from scratch, ensuring full compatibility with the map changes added to the game by the Last Stand update.

The aim is to re-implement improved versions of historical changes, unify map modifications across servers and configs, and providing a basic template that already includes all necessary fixes and improvements, which can easily be added to or modified by any server owners and config developers.

While many of the changes will appear similar to those included in from competitive Stripper:Source modifications, as they are designed to address the same issues and meet the expectations of the competitive community, the goal is to re-create everything from the ground up to ensure the best possible implementation of these changes.


## Usage
Any server owner or config developer can freely use this as a base for their own Stripper modifications if _**credit is given**_ to this repository.

All changes are tested and implemented with the latest version of Stripper:Source only.
* **Version:** 1.2.2 (hg82) `(updated 2011-04-15)`
* **AlliedModders:** https://forums.alliedmods.net/showthread.php?t=39439
* **Source:** https://github.com/alliedmodders/stripper-source
* **Documentation:** https://www.bailopan.net/stripper/


## Compatibility
The Stripper Rework is designed for full compatibility with the Last Stand map changes, as a result there is no need to modifiy `mapspawn.nut` or related files. The removal of any entities added through this method will be handled by Stripper:Source.

Servers should ensure the following scripts (located in `left4dead2/scripts/vscripts`) are unmodified:
* mapspawn.nut
* anv_mapfixes.nut
* anv_versus.nut

In order to ensure full compatibility with the changes provided by this rework, it is highly recommended that servers **DO NOT** load `clip_removal.smx` with configs that use this rework.

This plugin is flawed and does apply changes to both versus rounds. All functionality of this plugin can also be achieved with Stripper, making it entirely redundant.

#### Redundant Plugins
The following plugins can be removed from configs using the rework:
* **clip_removal** - Redundant, poor functionality, compatibility issues with reworked clips
* **l4d2_saferoom_gun_control** - Legacy ProMod plugin
    * **saferoom_gun_control.txt** - Dependent file that defines rules for saferoom weapons
* **l4d2_fireworks_noise_block** - Silenced the firework sounds on the Dark Carnival finale


## Documentation
A complete changelog for each map is available on the **[wiki](https://github.com/Derpduck/L4D2-Comp-Stripper-Rework/wiki)**.

Documentation for contributors and anyone looking to understand the implementation of Stripper:Source changes can also be found on the wiki.

Use the templates found in the [Templates](https://github.com/Derpduck/L4D2-Comp-Stripper-Rework/tree/master/_Templates) folder to ensure consistency with all Stripper:Source implementations found in this rework, and to make it as easy as possible for future contributors to modify.

To see what is being worked on currently, planned changes, and potential ideas for changes check out **[Projects](https://github.com/Derpduck/L4D2-Comp-Stripper-Rework/projects)**. 


## Official Map Updates
**Documentation and source code for the Last Stand update map updates can be found here:**\
**[Tsuey/L4D2-Community-Update](https://github.com/Tsuey/L4D2-Community-Update)**

**[How to view changes in-game](https://github.com/Derpduck/L4D2-Comp-Stripper-Rework/wiki/Viewing-Changes-In-Game)**


## Official Map Sources
### Decompiled VMFs (Valve Map Format)
**Decompiled versions of the offical L4D2 maps can be found here:**\
**[spumer/left_4_dead_2__decompiled_maps](https://github.com/spumer/left_4_dead_2__decompiled_maps)**

These files can be viewed and modified in the Hammer Editor by installing L4D2 Authoring Tools on Steam.\
It is highly recommended that any work done for this project is done through Hammer then implemented into Stripper to ensure values are accurate as possible.
**Disclaimer:** These files may not be 100% accurate as the decompiling process is not perfect, and the source files are not provided by Valve in any official capacity.

### Decompiled VScripts
**Decompiled versions of L4D2's VScripts can be found here:**\
**[jacob404/Official-Vscripts-Decompiled](https://github.com/jacob404/Official-Vscripts-Decompiled)**

These scripts can be used as reference or as a base for modifying director scripts for maps.\
Compiled versions of new or updated vscripts can be found at `Steam\steamapps\common\Left 4 Dead 2\update`.

### Stripper Dumps
To dump all entities on a map to text type `stripper_dump` in console while Stripper:Source is loaded.\
Files are dumped to the `stripper\dumps` directory in `.txt` format.


## Setting Up A Competitive L4D2 Server
**Resources and information for setting up a competitive L4D2 server can be found here:**\
**[SirPlease/L4D2-Competitive-Rework](https://github.com/SirPlease/L4D2-Competitive-Rework)**

This project is not part of the L4D2 Competitive Rework, however the competitive rework is a useful resource for anything related to running a competitive L4D2 server and competitive configs.\
Stripper changes found in this project are inspired by previous competitive configs.


## Contributing
Anyone is able to fork this repository and create pull requests to contribute to the project and will be credited below.\
Raise any issues or questions on the **[issue](https://github.com/Derpduck/L4D2-Comp-Stripper-Rework/issues)** tab.


## Credits
If you believe that you or any other historical contributors haven't been credited properly please raise an **[issue](https://github.com/Derpduck/L4D2-Comp-Stripper-Rework/issues)** so that they can be credited for their Stripper:Source and other related work.

### Rework Contributors
* Derpduck
* SirPlease

### Historical Contributors
* ProdigySim
* Jacob
* Blade
* Tabun
* Stabby
* CircleSquared
* Estoopi
* NF
* Visor
* RedJaneDoe
* Electrik
* SirPlease
* Spoon
* Wicket
* Devilesk
* Tsuey
