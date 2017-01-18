# Srch

A code searching tool for windows.

## Features

- Boyer-Moore
- Parallel search threads
- Utilizing char distribution (currently optimized for C)
- RegEx
- Case-Sensitivity
- Whole word Only
- Extension filter
- Drag & Drop
- GUI

## How to Use 

Run srch.exe and drag & drop a folder as your search path.

CTRL + F			-> Search text
CTRL + Shift + F	-> Search files
CTRL + Q			-> Cancel search
CTRL + S			-> Advanced settings
CTRL + ENTER		-> Search selected text (global hotkey)
F1 to F12			-> Load options from files

Edit the .txt files in the root folder to specify default search paths etc.

## Open Performance optimizations

1. Reduce the amount of exception handlers (try/catch)
2. Using the functionality encapsulated in the options class is convenient (e.g. options.GetValue(Options.AvailableOptions.SearchInComments)), but slows down the search queries (in the example case by ~30-40ms).

## Known Bugs

- When specifying the Editors, arguments must not be in quotes.
- Hotkeys only work in the first instance, other registrations fail.
- Window does not redraw occasionally.
- The source has to be cleaned up and reformatted.

## Usability improvements

- Implement more intuitive color picker / wheel
- Highlight the searched string in the results (a switch to richtext is needed)

## Contact

If you find any bugs, please contact me at srch(dot)bughunting(at)googlemail(dot)com

## Compiling

The application is compiled with

* Microsoft Visual Studio Express 2012 Version 11.0.61219.00 Update 5
* Microsoft .NET Framework  Version 4.6.01055

## Licensing

[MIT](https://github.com/atom/atom/blob/master/LICENSE.md)
