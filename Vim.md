### Editting Files
```
:e <file-name>
```
Much better than `:open`!!!


### Comment/Uncommenting
For those tasks I use most of the time block selection.

Put your cursor on the first # character, press CtrlV (or CtrlQ for gVim), and go down until the last commented line and press x, that will delete all the # characters vertically.

For commenting a block of text is almost the same:
	First, go to the first line you want to comment, press CtrlV. This will put the editor in the VISUAL BLOCK mode.
	Then using the arrow key and select until the last line
	Now press ShiftI, which will put the editor in INSERT mode and then press #. This will add a hash to the first line.
	Then press Esc (give it a second), and it will insert a # character on all other selected lines.

For the stripped-down version of vim shipped with debian/ubuntu by default, type : s/^/# in the third step instead (any remaining highlighting of the first character of each line can be removed with :nohl).

### Windows

#### for a terminal window
```:term
```
and then
```. ~/.bash_profile
```


## Find and Replace
:[range]s/{pattern}/{string}/[flags] [count]
```:%s/old/new/g
```
