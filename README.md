# open-in-vscode

Add "Open in Visual Studio Code" to the macOS context menu. Tested with macOS Ventura 13.2.1.

<img width="260" height="364" src="https://user-images.githubusercontent.com/51724788/227115981-886d8f74-ac42-474c-8570-a82204ea45a4.gif"/>

### Option 1: Prebuilt

1. Download the [latest release](https://github.com/lightningboltemoji/open-in-vscode/releases), extract, open to install

### Option 2: DIY (recommended)

1. Open Automator
2. File > New > Quick Action
3. Drag "Open Finder Items" to the main area
4. Open with -> Other... -> Visual Studio Code
5. File -> Save
6. Enter "Open in Visual Studio Code" (or anything you want the context action to say)
7. Open Terminal
8. Execute `plutil -remove NSServices.0.NSIconName "$HOME/Library/Services/Open in Visual Studio Code.workflow/Contents/Info.plist"`

## Credits

Nothing about this is original.

* [Sankra/OpenFolderInVSCode](https://github.com/Sankra/OpenFolderInVSCode)
* [idleberg's gist](https://gist.github.com/idleberg/bc65021a736e9139e3e31f7f2c761d5d)
* [Erik Johnson's Stack Exchange answer](https://apple.stackexchange.com/a/453044)
