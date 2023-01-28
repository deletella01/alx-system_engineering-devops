##  Loops, conditions and parsing

/  #!/usr/bin/env As a Shebang
The #! is called a shebang. It consists of a number sign and an exclamation point character (#!), followed by the full path to the interpreter such as /bin/bash. All scripts under Linux, *BSD, macOS, and Unix-like system execute using the interpreter specified on a first line. However, there is a small problem. BASH or Perl is not always in the same location (PATH) such as /bin/bash or /usr/bin/perl. If you want to make sure that script is portable across different UNIX like operating systems you need to use /usr/bin/env command as shebang.

## The for loop
-- How does it work?
The for loop is the first of the three shell looping constructs. This loop allows for specification of a list of values. A list of commands is executed for each value in the list.

The syntax for this loop is:

for NAME [in LIST ]; do COMMANDS; done

If [in LIST] is not present, it is replaced with in $@ and for executes the COMMANDS once for each positional parameter that is set.

The return status is the exit status of the last command that executes. If no commands are executed because LIST does not expand to any items, the return status is zero.

NAME can be any variable name, although i is used very often. LIST can be any list of words, strings or numbers, which can be literal or generated by any command. The COMMANDS to execute can also be any operating system commands, script, program or shell statement. The first time through the loop, NAME is set to the first item in LIST. The second time, its value is set to the second item in the list, and so on. The loop terminates when NAME has taken on each of the values from LIST and no items are left in LIST.