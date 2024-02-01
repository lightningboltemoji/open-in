<div align="center">
  <h1>open-in</h1>
  <div>Add a macOS context menu shortcut for your favorite editor!</div>
  <div><img width="260" height="364" src="https://user-images.githubusercontent.com/51724788/227115981-886d8f74-ac42-474c-8570-a82204ea45a4.gif"/></div>
</div>

<h1></h1>

Releases are published for **Visual Studio Code** and **Zed**, but following the steps below should work for most editors. Tested with **macOS Sonoma 14.3**.

### Option 1: Prebuilt

1. Download the [latest release](https://github.com/lightningboltemoji/open-in/releases), extract, open to install

### Option 2: DIY (recommended)

1. Open Automator
2. File > New > Quick Action
3. Search the actions sidebar for "Open Finder Items"
3. Drag it to the main area that says "Drag actions ..."
4. Open with -> Other... -> Visual Studio Code (or any editor)
5. File -> Save
6. Enter "Open in Visual Studio Code" (or what you want the context action to say)
7. Open Terminal
8. Execute `plutil -remove NSServices.0.NSIconName "$HOME/Library/Services/Open in Visual Studio Code.workflow/Contents/Info.plist"`

## Credits

Nothing about this is original. This is just meant to combine the best pieces of the existing methods that are floating around.

* [Sankra/OpenFolderInVSCode](https://github.com/Sankra/OpenFolderInVSCode)
* [idleberg's gist](https://gist.github.com/idleberg/bc65021a736e9139e3e31f7f2c761d5d)
* [Erik Johnson's Stack Exchange answer](https://apple.stackexchange.com/a/453044)
