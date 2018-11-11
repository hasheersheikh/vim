Basic VIm 
===

Modality
===

	Insert  - Brush is on the canvas
	Normal  - Brush is off the canvas
	Command - Mixing your pallette

Starting Vim
===
	:w filename
	
Pen to the page
===

	i - Enter insert mode at cursor
	I - Enter insert mode at first non-blank character
	s - Delete character under cursor and enter insert mode
	S - Delete line and begin insert at beginning of same line
	a - Enter insert mode _after_ cursor
	A - Enter insert mode at the end of the line
	o - Enter insert mode on the next line
	O - enter insert mode on the above line
	C - Delete from cursor to end of line and begin insert
	^ - move cursor first non blank character in line
	0 - move cursor first character in line including blank
	$ - move cursor to last character in line
	This is a test sentence
	
(Next class will cover 'c')

Replacing the character 
===
	r- replace the character 
	R- replaces multiple character until you stop
	c - change whatever we specify
	
Picking up the brush
===

	ESC
	Ctrl+[

Scanning the canvas
===

	    k
	    ^
	h <   > l
	    v
	    j


	G - move to the first caracter of last line
	gg - move to the start of the file

"They invented the mouse, why not use that?"
===
	because it is fast

Getting from a to b: Motions
===
Basics: wWbBeE
a word is lower case word is seprated with space 
a WORD is a word which is seprated with non space character
	w - Forward to the beginning of next word
	W - Forward to the beginning of the next WORD
	b - Backward to the next beginning of a word
	B - Backward to the next beginning of a WORD
	e - Forward to the next end of word
	E - Forward to the next end of WORD

Slightly less basic: fFtT
All follow [(n)um]<verb><n(o)un> syntax

	[n]f<o> - Forward until (nth) (o)  (Inclusive)
	[n]F<o> - Backward until (nth) (o) (Inclusive)
	[n]t<o> - Forward until (nth) (o)  (Exclusive)
	[n]T<o> - Backward until (nth) (o) (Exclusive)

	
	for example to find e in example we use fe for inclusive forworod finding
	simalarly for backword we use Fe
	for exclusive finding of e is for te(forword)
	for exclusive finding of e is Te (backword)

	abcdefg, abcdefg, abcdefg

Searching
===
   bounded and unbounded is a word totally included and word totlly not included in ie' subword
	/  - Forward
	?  - Backward
	*  - Word under cursor - forward  (bounded)
	g* - Word under cursor - forward  (unbounded)
	#  - Word under cursor - backward (bounded)
	g# - Word under cursor - backward (unbounded)
	n  - Next result, forward
	N  - Next result, backward
(Note here to explain what bounded/unbounded mean)

Delete
===
	x - delete one character on cursor
	X - delete one character previous to cursor
	d - delete what ever we specify
	D - delete to the end of the line
	
Copy/Paste
===

	y - Yank. Example: yw (yank word)
	p - paste after cursor
	P - paste before cursor

Autocomplete commands
===
	for autocomplete mode you have to be in insert mode
	<initial words for letter> Ctrl-p - for auto complete the word(list will apper to Autocomplete this)
	<word> Ctrl-x + Ctrl-l - for auto complete the LINE (list will apper for completing the line)


Searching file path within file
===
	[/]+Ctrl-x + Ctrl-f - access path inside the file (give you the list of all path inside the directory)

# vim: set syn=mkd :
