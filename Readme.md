# vim-todo

Easy-peasy todo list manager for VIM!

##Usage

Basically vim-todo works with .todo files and gives them syntax highlighting
and some special commands. There are two modes: normal and edit.

Normal mode is default. **j** and **k** let you navigate among tasks. **v** marks a
task as finished and **x** un-finishes it.

When you press **e**, you enter edit mode, and you can navigate the file with vim
modes normally, so you can add new tasks and change things.

You can find an example.todo file to see how a vim-todo file looks like :)

##Known issues
* Filetype detect does not work. Workaround: create a todo.vim file in
  your ~/.vim/ftdetect folder with the following line:

    au BufRead,BufNewFile *.todo,TODO setfiletype todo
