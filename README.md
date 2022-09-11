# vim_tutorial

 The basics

Create a vertical split using :vsp and horizontal with :sp.

By default, they duplicate the current buffer. This command also takes a filename:

:vsp ~/.vimrc

You can specify the new split height by prefixing with a number:

:10sp ~/.zshrc

Close the split like you would close vim:

:q

Easier split navigations

We can use different key mappings for easy navigation between splits to save a keystroke. So instead of ctrl-w then j, it’s just ctrl-j:

nnoremap <C-J> <C-W><C-J>
nnoremap <C-K> <C-W><C-K>
nnoremap <C-L> <C-W><C-L>
nnoremap <C-H> <C-W><C-H>

More natural split opening

Open new split panes to right and bottom, which feels more natural than Vim’s default:

set splitbelow
set splitright

Resizing splits

Vim’s defaults are useful for changing split shapes:

"Max out the height of the current split
ctrl + w _

"Max out the width of the current split
ctrl + w |

"Normalize all split sizes, which is very handy when resizing terminal
ctrl + w =

More split manipulation

"Swap top/bottom or left/right split
Ctrl+W R

"Break out current window into a new tabview
Ctrl+W T

"Close every window in the current tabview but the current one
Ctrl+W o

Please :help me

As with everything in Vim, for more information, check the well-written helpfiles. In Vim, :help splits.
