Work with multiple files in Vim 
===============================

ref: <http://stackoverflow.com/questions/53664/how-to-effectively-work-with-multiple-files-in-vim>

`:ls`
----

for list of open buffers

*	`:bp` previous buffer
*	`:bn` next buffer
*	`:bn` (`n` a number) move to n'th buffer
*	`:b <filename-part>` with tab-key providing auto-completion (awesome !!)

In some versions of vim, `bn` and `bp` are actually `bnext` and `bprevious` respectively. Tab auto-complete is helpful in this case.

Or when you are in normal mode, use `^` to switch to the last file you were working on.

Plus, you can save sessions of vim

	:mksession! ~/today.ses

The above command saves the current open file buffers and settings to `~/today.ses`. You can load that session by using

	vim -S ~/today.ses

No hassle remembering where you left off yesterday. ;)
