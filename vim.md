# Operators

|||
|-------|---------|
|c|change|
|d|delete|
|y|yank into register|
|~|swap case|
|gu|make lowercase|
|gU|make uppercase|
|!|filter to external program|
|<|shift left|
|>|shift right|
|=|indent|

# Text Objects

|||
|-------|---------|
|aw|a word (with followed space), by start of words (punctuation considered words)|
|iw|inner word|
|aW|a WORD, by start of words (spaces separate words)|
|iW|inner WORD|
|ap|a paragraph|
|ip|inner paragraph|
|ab|a bracket|
|ib|inner bracket|
|at|a tag block|
|it|inner tag block|

# Motions

|||
|-|-|
|%|go to first matching paren / bracket|
|[count]+|down to first non blank char of line|
|[count]$|to end of line|
|[count]f/F(char)|to next occurence of (char)|
|[count]t/T(char)|to before next occurence of (char)|
|[count]h/k/j/l|left, down, up, right|
|[count]]m|go to beginning of next method|
|[count]w/W|go a word / WORD to the right|
|[count]b/B|go a word / WORD to the left|
|[count]e/E|go to end of word / WORD right|

# Useful VIM Shortcuts

Some of these shortcuts work with some plugins that I have, you can see the list of plugins [here](https://github.com/naeemba/dotfiles/blob/master/nvim/init.vim).

|Command|Description|Source|Details|
|-------|-----------|------|-------|
|`=i{`|Correct indentions|[source](https://www.freecodecamp.org/news/learn-linux-vim-basic-features-19134461ab85/)|Place the cursor anywhere within a block you want to indent, press Esc to enter normal mode and then: =i{|
|`m{lowercaseletter}`|Create local bookmark|[source](https://www.freecodecamp.org/news/learn-linux-vim-basic-features-19134461ab85/)||
|`:marks`|List all local bookmarks|[source](https://www.freecodecamp.org/news/learn-linux-vim-basic-features-19134461ab85/)||
|`` `{lowercaseletter} ``| Go to bookmark|[source](https://www.freecodecamp.org/news/learn-linux-vim-basic-features-19134461ab85/)||
|`ytx`|Yank till character|[source](https://vim.fandom.com/wiki/Copy,_cut_and_paste)|yank from the current cursor position up to and before the character (til x)|
|`yfx`|Yank till character|[source](https://vim.fandom.com/wiki/Copy,_cut_and_paste)|yank from the current cursor position up to and including the character (find x)|
|`:e %:h/filename`<br />`:w`|Create a new file|[source](https://stackoverflow.com/a/13239757/2443849)|will create a new file named filename in the same directory as the currently open file, and write it|
|`2dt{character}`|Delete until second occurance of `{character}`|[source](https://askubuntu.com/a/64840)|This will delete upto but not including `{character}`|
|`2ft{character}`|Delete until second occurance of `{character}`|[source](https://askubuntu.com/a/64840)|This will delete upto and including `{character}`|
|`daw`|Delete the word under the cursor|[source](https://stackoverflow.com/a/835016/2443849)|Delete a word|
|`caw`|Delete the word under the cursor and put you in insert mode|[source](https://stackoverflow.com/a/835016/2443849)|Change a word|
|`:E`|Open current directories files to select from|[source](https://stackoverflow.com/questions/573039/shortcut-to-open-file-in-vim#comment3399452_574537)|Browsable current directory|
|`:ex`|File explorer|[source](https://stackoverflow.com/a/1205382/2443849)|Open file explorer, hitting `r` on a file will rename it and hitting `d` will delete that file|
|`Gmove {newName}`|Rename file|[source](https://stackoverflow.com/a/13501814/2443849)|Rename current file in buffer, git and disk with undo history|
|`Gwrite`|Add to git|[source](https://stackoverflow.com/a/13501814/2443849)|Add current file to git|
|`:E`|File Explorer|[source](https://unix.stackexchange.com/a/495104)||
|`:E => select file => shift-d`|Delete File|[source](https://unix.stackexchange.com/a/495104)||
|`I`|Move cursor to the first non blank char of the current line and go to insert mode|[source](http://worldtimzone.com/res/vi.html)||
|`I`|Move cursor to end of the current line and go to insert mode|[source](http://worldtimzone.com/res/vi.html)||
|`^`|Move to first non blank char in current line|[source](https://stackoverflow.com/a/50483994/2443849)||
|`*`|Search for the word under the cursor|[source](https://chrome.google.com/webstore/detail/lbhnkgjaoonakhladmcjkemebepeohkn)||
|`:e`|Refresh current file|[source](https://unix.stackexchange.com/a/149210)||
|Ctrl+w followed by `w`, `h`, `j`, `k`, `l`|Switch between windows|[source](https://linuxhint.com/how-to-use-vim-split-screen/)[source](https://superuser.com/a/280501/894627)||
|`vi'`|Select inside `'`|[source](https://stackoverflow.com/a/1062001)||
|`vib`|Select inside block (parenthesis)|[source](https://stackoverflow.com/a/1062001)||
|`viB`|Select inside curly braces|[source](https://stackoverflow.com/a/1062001)||
|`va'` `vab` `vaB`|Like 3 aboves, also will select the `'` itself too|[source](https://stackoverflow.com/a/1062001)||
|6+|6x go down to line start|[source](https://www.youtube.com/watch?v=E-ZbrtoSuzw)|
|gUaW|capitalize a WORD|[source](https://www.youtube.com/watch?v=E-ZbrtoSuzw)|
|3ce|3x change to word end|[source](https://www.youtube.com/watch?v=E-ZbrtoSuzw)|
|4$|4x go to end of line|[source](https://www.youtube.com/watch?v=E-ZbrtoSuzw)|
|d]m|delete to start of next method|[source](https://www.youtube.com/watch?v=E-ZbrtoSuzw)|
|%|jump to match of next paren or bracket|[source](https://www.youtube.com/watch?v=E-ZbrtoSuzw)|
