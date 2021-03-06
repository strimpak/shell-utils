Some years ago I read a book about shell scripting; AFAIR it was called something like "Teach yourself shell scripting in 
24 hours" by Sams publishing. The author of the book had the (nice) idea of creating a library with shell functions that 
can be used over and over by system administrators, shell programmers, and generally users who enjoy typing on a terminal.

I decided to take the library and extend it. Thus, whenever I find a useful function I add it, and whenever I encounter a bug 
I am trying to fix it. I named the library shell-utils because this is what it really is. To use shell-utils simply add it to 
your shell's environment. For example, this is how my `.bashrc` entry looks like:
```
if [ -f ~/bin/shell-utils.sh ]; then
   . ~/bin/shell-utils.sh
fi
```
Even though the library contains around fifteen functions, I found out that the most useful (at least if you are working with 
many different file types) are `file_to_lower`, `file_to_upper` and `rename_all_suffix`, `rename_all_prefix`. See the 
following figure to get an idea of how they can be invoked.

![example](http://i67.tinypic.com/f1yw5u.png)
