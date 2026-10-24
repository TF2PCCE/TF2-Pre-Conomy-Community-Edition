# Team Fortress 2: Pre-Conomy
Source repository for TF2 Pre-Conomy: Community Edition, an attempt to revive TF2: Preconomy, A TF2 sourcemod aiming to create an authentic old-school experience.

Note: This is in very early stages!!! Expect crashes or missing weapon reverts.

## Build instructions

Clone the repository using the following command:

`git clone https://github.com/TF2PCCE/TF2-Pre-Conomy-Community-Edition/TF2-Pre-Conomy`

### Windows

Requirements:
 - Source SDK 2013 Multiplayer installed via Steam
 - Visual Studio 2022 with the following workload and components:
   - Desktop development with C++:
     - MSVC v143 - VS 2022 C++ x64/x86 build tools (Latest)
     - Windows 11 SDK (10.0.22621.0) or Windows 10 SDK (10.0.19041.1)
 - Python 3.13 or later

Inside the cloned directory, navigate to `src`, run:
```bat
createtf2pcceprojects.bat
```
This will generate the Visual Studio project `tf2pcce.sln` which will be used to build your mod.

Then, on the menu bar, go to `Build > Build Solution`, and wait for everything to build.

You can then select the `Client (Mod Name)` project you wish to run, right click and select `Set as Startup Project` and hit the big green `> Local Windows Debugger` button on the tool bar in order to launch your mod.

The default launch options should be already filled in for the `Release` configuration.

### Linux

Requirements:
 - Source SDK 2013 Multiplayer installed via Steam
 - podman

Inside the cloned directory, navigate to `src`, run:
```bash
./buildtf2pcceprojects
```

This will build all the projects related to the SDK and your mods automatically against the Steam Runtime.

You can then, in the root of the cloned directory, you can navigate to `game` and run your mod by launching the build launcher for your mod project, eg:
```bash
./tf2pc
```
