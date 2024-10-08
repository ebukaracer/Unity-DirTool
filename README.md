# DirTool
[![](https://img.shields.io/badge/PRs-welcome-blue)](http://makeapullrequest.com) [![License: MIT](https://img.shields.io/badge/License-MIT-blue)](https://github.com/ebukaracer/ebukaracer/blob/ebukaracer-resources/LICENSE.md)

- Handles project folder creation and deletion with ease inside the Unity editor.
	<img src="https://github.com/ebukaracer/ebukaracer/blob/ebukaracer-resources/DirTool-Images/DT2.gif" alt="gif"/>

## Installation
A detailed guide can be found: [here](https://github.com/ebukaracer/EzUnityUtils/blob/main/INSTALLGUIDE.md#install-guide)

*Nevertheless, in unity editor inside package manager:*
- Hit `(+)` and select `Add package from Git URL(Unity 2019.4+)` 
- Paste the `git URL` for this package: https://github.com/ebukaracer/Unity-DirTool.git 
- Hit `Add`

## Usage

### Setup:
*If the installation was successful, a menu option: `Racer > DirTool` will be available.*
- Click on `Racer > DirTool > Menu` to lunch the Editor window.

#### Quick Create:
`Racer > DirTool > Quick Create`
- Handy dropdown option for quickly creating folders that were already supplied in the *Root-Directory* and *Sub-Directories* fields

#### Remove package:
`Racer > DirTool > Remove package`
- Handy dropdown option for quickly uninstalling this package without leaving any trace! 

#### Create [Directories]:
- Creates a root-folder alongside nested sub-folders, using the *Root-Directory* and *Sub-Directories* fields supplied. The *Root-Directory* field can also contain nested directories by separating with slash symbol: `Project/root`
- You must supply the *Sub-Directories* along with their *Root-Directory(optional)*, since this operation mostly focuses on creating the *Sub-Directories*.
- Leaving *Root-Directory* field empty still creates the supplied *Sub-Directories* in relative to Asset's folder: `Assets/[Sub-Directories_supplied]`

#### Delete [Sub Directories]:
- Deletes only the *Sub-Directories* supplied leaving out their Root-Directory.
- If you supplied a *Root-Directory* such as: `Project/` and *Sub-Directories*: `Models, Scripts`, this process will only delete the *Sub-Directories*: `Models, Scripts` , omitting the *Root-Directory*: `Project/` along with other *Sub-Directories* you did not supply in the *Sub-Directories* field.
- You must supply the *Sub-Directories* along with their *Root-Directory(optional)*, since this operation mostly focuses on deleting the *Sub-Directories*.
- Leaving *Root-Directory* field empty still deletes any *Sub-Directories* it finds that is relative to Asset's folder: `Assets/[Sub-Directories_found]`

#### Delete [Root Directory]:
- Deletes the *Root-Directory* alongside *Sub-Directories* supplied.
- If you supplied a nested *Root-Directory* such as: `Project/Models`, the deletion process will terminate at `Project/` whilst deleting `Models/` along with its contents.
- If you supplied: `Projects/`, this process deletes the Root-Directory: `Projects/` along with any *Sub-Directories* it may contain. Hence terminating at `Assets/`
- Therefore, you may leave the *Sub-Directories* field empty, since this operation focuses on deleting only the *Root-Directory*. It is impossible to delete `Assets/` directory ;)

#### Create [ASMDEF]:
- Creates an `asmdef file` in the path supplied at *Root-Directory* field.
- If you intend to use a *custom path*, start with: `Assets/[your_desired_custom-path]`

##  Note for users
> The operations above can also be applied to already existing directories in your project.

> Toggle on or off `Recursive delete`, to control how to delete parent directories containing nested directories or subdirectories.

> Ensure no slash symbol: `/\` terminates the Root-Directory field: `Project/Scripts/` but `Project/Script`

> Few other commands available are backed-up with self-explanatory tool-tips in accordance with what they offer.

> After removing this package, do well to delete `DirTool` folder located at: `Assets/DirTool`, or simply use the [`Remove package`](https://github.com/ebukaracer/Unity-DirTool/tree/main?tab=readme-ov-file#remove-package) menu option.

## Contributing    
Contributions are welcome! Please open an issue or submit a pull request.
