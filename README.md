# DirTool

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-blue.svg)](http://makeapullrequest.com) [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/ebukaracer/ebukaracer/blob/ebukaracer-resources/LICENSE.md)

- Streamlines creation and deletion of *Project's Directories* via an easy-to-navigate user interface inside Unity editor.

## Installation
A detailed guide can be found [here](https://github.com/ebukaracer/EzUnityUtils/blob/main/INSTALLGUIDE.md#install-guide)

*Alternatively, you can quickly install this package by choosing: `Add package from Git URL(Unity 2019.4+)` thereafter you paste the `git URL` for this package: https://github.com/ebukaracer/Unity-DirTool and click  `Add`*

## Usage Guide
*If the installation was successful, a menu option: `DirTool` will be available via `Racer` menu drop-down inside unity editor.*

📌*The DirTool-Menu for this package comes with pre-populated fields for directories you may find handy in your project. Feel free to adjust to your taste.*

## Operations

#### Quick Create:
- Handy shortcut for quickly creating folders that were already supplied in the *Root-Directory* and *Sub-Directories* fields.

#### Create [Directories]:
- Creates a root-folder alongside nested sub-folders, using the *Root-Directory* and *Sub-Directories* fields supplied. The *Root-Directory* field can also contain nested directories by separating with slash symbol: `Project/root`
- Here, you must supply the *Sub-Directories* along with their *Root-Directory(optional)*, since this operation mostly focuses on creating the *Sub-Directories*.
- Leaving *Root-Directory* field empty still creates the *Sub-Directories* supplied relative to Asset's folder: `Assets/[your Sub-Directories]`

#### Delete [Sub Directories]:
- Deletes only the *Sub-Directories* supplied leaving out their Root-Directory.
- If you supplied a Root-Directory: `Project/` and Sub-Directories: `Models, Scripts`, this process will only delete the Sub-Directories: `Models, Scripts` , omitting the Root-Directory: `Project/` along with other Sub-Directories you didn't supply in the Sub-Directories field.
- Here, you must supply the *Sub-Directories* along with their *Root-Directory(optional)*, since this operation mostly focuses on deleting the *Sub-Directories*.
- Leaving *Root-Directory* field empty still deletes any *Sub-Directories* it finds that is relative to Asset's folder: `Assets/[found Sub-Directories]`

#### Delete [Root Directory]:
- Deletes the Root-Directory alongside Sub-Directories supplied.
- If you supplied a nested Root-Directory such as: `Project/Models`, the deletion process will terminate at `Project/` whilst deleting `Models/` along with its contents.
- If you supplied: `Projects/`, this process deletes the Root-Directory: `Projects/` along with any Sub-Directories it may contain. Hence terminating at `Assets/`
- Here, you may leave the *Sub-Directories* field empty, since this operation focuses on deleting only the *Root-Directory*. It is impossible to delete `Assets/` directory!

> [!NOTE]
> 📌*The operations above can also be applied to already existing directories in your project.*
> 
> 📌*The deletion process is a destructive one, as such, check sure you're not deleting folders containing important contents.*
> 
> 📌*Ensure no slash symbol: `/\` terminates the Root-Directory field: `Project/Scripts/` but `Project/Script`.*
> 
> 📌*Few other commands available are backed-up with self-explanatory tool-tips in accordance with what they offer.*  
> 
> 📌*After removing this package, do well to delete `DirTool` folder located at: `Assets/DirTool`*

## Contribution
Feel free to open an `issue` If you discovered any bug or feel like something is missing. 

*PS: Kindly, drop a ⭐ if found useful.*
