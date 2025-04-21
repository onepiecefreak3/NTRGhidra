# NTRGhidra ![](https://img.shields.io/github/issues/pedro-javierf/NTRGhidra/bug)<br>

A Nintendo DS Loader for Ghidra

![NTRGhidra a Nintendo DS Loader for Ghidra](https://user-images.githubusercontent.com/16199912/56060896-12690380-5d36-11e9-802e-8c7e70cd481e.png)

Latest Ghidra version supported: 11.3.1 (21/04/2025 | dd/mm/yyyy)


# License
NTRGhidra is released under the ![Apache License 2.0](https://github.com/pedro-javierf/NTRGhidra/blob/master/LICENSE).

# Contributing & Support
* Fork, modify and pull request to contribute,
* Open issues suggesting feautures, reporting bugs, asking for documentation or changes, etc.
* Solve known problems reported in the ![issues](https://github.com/pedro-javierf/NTRGhidra/issues) 
* Support by starring the project.

```diff
! This project is looking for maintainers and contributors --> If you'd like to join this effort
! and contribute or administer the project in any way, please open an issue to get in touch. Thank you!
```

# Features
A list of In Progress / To-Do / Completed features is available in [this listing](https://github.com/pedro-javierf/NTRGhidra/projects/1)

# Installation
If you just want to install the loader into a existing Ghidra installation:

1. Download the .zip from the [releases page](https://github.com/pedro-javierf/NTRGhidra/releases) (Or build the project yourself from the code, instructions below).
2. Put the .zip into the GHIDRA_INSTALL_DIR/Extensions/Ghidra folder
3. In the initial Ghidra window (not in the Code Browser), open the "File" menu, and select "Install Extensions". Click the small 'plus' icon in the top right of the window, and select the extension zip file downloaded. This should add an entry into the extensions list. Make sure it is checked and click OK.

![Step 1](install1.png)
![Step 2](install2.PNG)

4. Restart Ghidra.

# How to Build

NOTE: If you notice any exception while debugging with Eclipse, please ![create an issue](https://github.com/pedro-javierf/NTRGhidra/issues)

These are the basic steps to debug and build the loader. You must have a Ghidra installation.

1. Install Ghidra
2. Install the Eclipse IDE
3. In Eclipse, install the Ghidra Development Extension. Click Help > "Install New Software" (https://stackoverflow.com/questions/31553376/eclipse-how-to-install-a-plugin-manually)
4. After the extension is installed, clone/download this repository, which contains an Eclipse project.
5. Open the project with Eclipse (File > Open Projects from File System)
6. You may need to reconnect Ghidra to the project by right clicking the project in Eclipse, and doing GhidraDev -> Link Ghidra...
7. Build: Select "File > Export", and then choose "Ghidra > Ghidra Module Extension". You can then use a local Gradle installation or an online build system.

# Acknowledgements
* Special thanks to [gbatek](https://problemkaputt.de/gbatek.htm) for ds technical info
* Thanks to Gericom for the original C# Header and ARM9 decompression code from EFE(Every File Explorer), as well as for testing.

# Others
For reference and tutorials about Ghidra loaders and how to write them, you may want to read:
* [Tutorial: Writing a Ghidra loader](https://pedro-javierf.github.io/devblog/tutorialwritingaghidraloader/)
* [Advanced Ghidra Loader: labels, overlays and Function ID](https://pedro-javierf.github.io/devblog/advancedghidraloader/)
