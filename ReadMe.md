# Steve's Unreal Scripts

## Summary

These scripts are to help with various tasks in [Unreal Engine](https://www.unrealengine.com). 
They're written on the basis of using Git / Git LFS rather than Perforce (many of Unreal's own
automation tools assume P4, which can be inconvenient).

These scripts support **UE4 and UE5** and will detect which one your project is using

* [Setting up a project for Git / Git-LFS](./doc/GitSetup.md): including LFS locking
  * + in fork: locking, ignoring file types and folders from [XistGG/UE5-Git-Init](https://github.com/XistGG/UE5-Git-Init/) and Epic Games' default `.urcignore` file
* [Managing Git LFS Locking Tasks](https://github.com/sinbad/GitScripts): push and unlock, release locks you don't need any more
* [Packaging a Game](./doc/Package.md): building, cooking, archiving
* [Releasing a Game](./doc/Release.md): e.g. uploading to Itch, Steam
* [Rebuilding Lightmaps](./doc/RebuildLightmaps.md): build lighting on the command line easily (supporting git-lfs locking, no P4 dependency like RunUAT)
* [Getting Latest for Artists](./doc/GetLatest.md): pulls from git and builds so C++ changes are automatically updated
* [Synchronising BuiltData Files outside of Git](./doc/DataSync.md)
* [Cleaning Up](./doc/Cleanup.md): Deleting unneeded Hot Reload DLLs etc


## Prerequisites

* Powershell Core 7+
  * Almost everything is compatible with Win10 built-in PS 5.1 but 7 is better, and platform independent
* PsIni module installed (library for reading INI files easily)
   * Run `Install-Module PsIni` in a Powershell console
* Itch's [`butler` tool](https://itch.io/docs/butler/) if you wish to release to Itch.io
* The [Steamworks SDK](https://partner.steamgames.com/doc/sdk) if you wish to release on Steam

