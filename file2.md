SOURCE :  https://www.linux.com/training-tutorials/vim-tips-using-tabs/#:~:text=With%20Vim%207.0%2C%20users%20now,have%20access%20to%20this%20feature.

SOURCE : https://stackoverflow.com/questions/53664/how-to-effectively-work-with-multiple-files-in-vim

SOURCE : https://stackoverflow.com/questions/53664/how-to-effectively-work-with-multiple-files-in-vim#:~:text=You%20can%20switch%20between%20tabs,can%20easily%20switch%20between%20files.&text=Show%20activity%20on%20this%20post.,-Listing



You can switch between tabs with :tabn and :tabp, With :tabe <filepath> you can add a new tab; and with a regular :q or :wq you close a tab. If you map :tabn and :tabp to your F7/F8 keys you can easily switch between files.




Listing
To see a list of current buffers, I use:

:ls
Opening
To open a new file, I use

:e ../myFile.pl
with enhanced tab completion (put set wildmenu in your .vimrc).

Note: you can also use :find which will search a set of paths for you, but you need to customize those paths first.

Switching
To switch between all open files, I use

:b myfile
with enhanced tab completion (still set wildmenu).

Note: :b# chooses the last visited file, so you can use it to switch quickly between two files.

Using windows
Ctrl-W s and Ctrl-W v to split the current window horizontally and vertically. You can also use :split and :vertical split (:sp and :vs)

Ctrl-W w to switch between open windows, and Ctrl-W h (or j or k or l) to navigate through open windows.

Ctrl-W c to close the current window, and Ctrl-W o to close all windows except the current one.

Starting vim with a -o or -O flag opens each file in its own split.
