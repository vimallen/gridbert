---
title: Vim tips and snippets
author: Dave Allen
layout: post
permalink: /vim-tips-and-snippets/
categories: software
---
A few things that I find useful in vim.

#### How to create a new file in the file explorer
Vim's built-in file explorer, properly called netrw, is excellent. Once you get used to a few aspects you won't need any of the 'sidebar' plug-ins available. It is not immediately obvious how to create a new file when in the file explorer view for example. So here's how.

1.	In the command line, cd to the directory of your project.
1.	Run vim . (vim dot) to open the file explorer.
1.	Your cursor will already be on the correct position for creating a new file. 
![cursor position][1]
1.	Type % and you'll be see a prompt in the vim's command line to enter a filename.

Nothing will appear in your working tree of your computer's OS until you edit and save the file. If after that you still don't see the file, then its probably because you have moved to another directory during your session. 

#### To change to the directory of the currently open file type
	
	:lcd %:p:h

This is a bit of a mouthful so adding the following to your .vimrc is very useful:

	" CDC = Change to Directory of Current file
	command CDC cd %:p:h

Now typing CDC will put you in the right place. Typing uppercase proves not to be awkward.

More vim things to follow.

[1]: ../images/cursorHere.jpg