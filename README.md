This is a Chrome extension (written in C#) that shows a Xamarin.Forms page inside a popup. Xamarin.Forms and C# are compiled to WebAssembly via Uno.platform and Mono Wasm.

## How to build
1. Open the solution with Visual Studio 2019 or VS for Mac 8.6.7 (or newer)
1. Publish the .wasm project to a local folder
1. Copy manifest.json, stylesheet.css and icon.png from uno_extension/ folder into it.
1. Delete subfolders which start with underscore.
1. Edit index.html to include <link rel="stylesheet" type="text/css" href="./stylesheet.css" /> like the index.html that is inside uno_extension/

## How to install:
1. In Chrome go to `chrome://extensions/`
1. Enable [Developer mode] (if not enabled)
1. Click [Load unpacked]
1. Go inside the publilshed folder above
1. Click [Select Folder]/[Open] button
