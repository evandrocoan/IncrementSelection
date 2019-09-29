Increment Selection
==================

Add a number to each selection in Sublime Text, incremented once per selection.
You may also insert the number of line containing the selection by using the '#' symbol.

This plugin is based on [Riccardo Marotti's answer](http://stackoverflow.com/a/14578077) on StackOverflow.  The default hotkey is <kbd>ctrl</kbd> <kbd>alt</kbd> <kbd>i</kbd> or <kbd>cmd</kbd> <kbd>ctrl</kbd> <kbd>i</kbd>.

Usage
-------

Place the cursors where you need:

![step 1](http://i.stack.imgur.com/rBPkj.png)

Insert the number the counter should start from (in this case 1):

![step 2](http://i.stack.imgur.com/hODtW.png)

Select the number you typed (<kbd>shift</kbd> <kbd><&mdash;</kbd>):

![step 3](http://i.stack.imgur.com/EJLco.png)

Type the shortcut:

![step 4](http://i.stack.imgur.com/w7wpJ.png)


Examples
----------

Tips:  `[]` stands for a selection, `|` stands for a caret.

	[1] text [1] text [1] -> 1| text 2| text 3|

	[a] text [a] text [a] -> a| text b| text c|

	[A] text [A] text [A] -> A| text B| text C|

	[01] text [01] text [01] -> 01| text 02| text 03|

	[05,2] text [05,2] text [05,2] -> 05| text 07| text 09|

	[5,-1] text [5,-1] text [5,-1] -> 5| text 4| text 3|

	[a,3] text [a,3] text [a,3] -> a| text d| text g|

Increment follows the difference between the first and second element:

	[10] text [9] text [1] -> 10| text 9| text 8|

	[a] text [c] text [a] -> a| text c| text e|

Generate line numbers:

	[#] line -> 1| line
	[#] line -> 2| line
	[#] line -> 3| line
	[#] line -> 4| line
	[#] line -> 5| line


## Installation

### By Package Control

1. Download & Install `Sublime Text 3` (https://www.sublimetext.com/3)
1. Go to the menu `Tools -> Install Package Control`, then,
   wait few seconds until the `Package Control` installation finishes
1. Go to the menu `Preferences -> Package Control`
1. Type `Package Control Add Channel` on the opened quick panel and press <kbd>Enter</kbd>
1. Then, input the following address and press <kbd>Enter</kbd>
   ```
   https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json
   ```
1. Now, go again to the menu `Preferences -> Package Control`
1. This time type `Package Control Install Package` on the opened quick panel and press <kbd>Enter</kbd>
1. Then, search for `IncrementSelection` and press <kbd>Enter</kbd>

See also:
1. [ITE - Integrated Toolset Environment](https://github.com/evandrocoan/ITE)
1. [Package control docs](https://packagecontrol.io/docs/usage) for details.

