# SemanticMerge (2.0.138.0 Windows) Dark Theme

unofficially dark theme / dark mode for semanticmerge 2.0.138.0

Dark theme is not officially supported yet in this version of semantic merge, but this is my take of fixing up what is already working.
This uses most of the same colors as VSCode Dark.

Only supports C# for now. If you want Java etc., then change the `languages.conf` file.

## Warning 1

Will overrite default configuration files, take a backup before installing.
If you have thirdparty parsers, manually add the line in the `languages.conf` file to the two of the files.

## Warning 2

Hack. I could not get the `CSharp.langdef` colors working, therefor .cs is overriden to use `VBScript.langdef` for syntax coloring (with C# style in the file).
This is done through `languages.conf` file. In semanticmerge for `semanticmergetool`, and plastic4 folder for `mergetool`

## Installation

1. Take a backup of folders `C:\Users\<username>\AppData\Local\plastic4`, and `C:\Users\<username>\AppData\Local\semanticmerge`.
2. Copy files into folder `C:\Users\<username>\AppData\Local`.

## Issues

- Syntax for C# must go through another language definition file (the parser seems to work the same way, but this might change in future versions).
- ~~Right margin in the codeview is white, this is a transparent color to a white background, have not found a way of changing this yet.~~
- Left side helper window still white, can change text color etc. but have not found any way of changing the background.
- ~~White lines in mergetool and resultview in semnaticmergetool.~~
