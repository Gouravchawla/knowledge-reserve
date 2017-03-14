############################
Date: 2017-03-14
URL : NA
############################

### Movement: 
- h (left); j(down); k(up); l(right)
- 0 : put cursor at the start of line
- gg : move cursor to start of file
- G : move cursor to start of last line of file

### Deletion:
- x : delete one letter under the cursor
- dw : delete word from cursor position
- de : delete word from cursor position
- dd : delete the whole line

### Multiple Deletions:
- `d<n>w` : delete n number of  words and the space after that
- `d<n>e` : delete n number of words
- `<n>dd` : delete n number of lines

- u : undo
- U : undo all the changes on that line
- CTRL+R = redo

### Copy/Paste:
- CTRL+Shift+V: paste from clipboard

### Chapter 28: FOLDING
- zfap: fold a paragrap
- zo: open fold
- zc: close fold
- zm: fold more
- zM: fold more(all)
- zr: fold reduce
- zR: fold Reduce(all)
- zi: toggle between folds
