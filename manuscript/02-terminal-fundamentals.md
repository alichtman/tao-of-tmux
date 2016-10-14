# Terminal fundamentals

Before I get into tmux, there are a few fundamentals of the command line I want
to run over.

Seasoned developers are familiar with what zsh, bash, iterm2, konsole, /dev/tty,
and so on, but a fair deal never had a run through of how they interact with
each other.

## POSIX roots

Operating systems like MacOS (formerly OS X), Linux and the BSD's all of
something similar[^similar-POSIX] to the POSIX specification in terms of how
they square away various responsibilities and interfaces of the operating
system.

[^similar-POSIX]: Not all operating systems follow the POSIX standard
absolutely. What you'll end up finding is that they're categorized as "Mostly POSIX-compliant"[^posix-compliant-wikipedia].

In daily life, we often use systems that break compatibility with POSIX
standards for sheer reasons of practicality. Operating systems like MacOS will
drop you right into Bash. ``make(1)``, which is also a POSIX standard, is in
actuality GNUMake on MacOS by default.  Did you know that as of September 2016
POSIX Make has no conditionals?

I'm not saying this to take a run at purists, as I'm someone who tries to remain
as compatible as possible in my scripting, it gets very hard to do simple
things after a while. On FreeBSD, the default Make uses dots between
conditionals:

    .IF

    .ENDIF

But on most Linux systems and MacOS, Bash is often the default shell
interpreter, so they get to do:

    IF

    ENDIF

## Terminal interface

The terminal interface can be best introduced by stating their is an official
specification laying out its technical properties, interfaces and
responsibilities [^opengroup-terminalinterface].


[^opengroup-terminalinterface]: http://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap11.html
[^posix-compliant-wikipedia]: https://en.wikipedia.org/wiki/POSIX#Mostly_POSIX-compliant

## Terminal emulation

GUI Terminals: Terminal.app, iterm, iterm2, konsole, lxterm, xfce4-terminal,
rxvt-unicode, xterm, roxterm, gnome terminal, cmd.exe + bash.exe

## Shell interpreters (Shells)

Examples: POSIX sh, BASH, ZSH, tcsh, ksh, fish

When we speak about "shells", such as the examples below, we're often referring
to the interpretter.

Plain old shell is based of a standard.

As of October 2016, the [latest specification](http://pubs.opengroup.org/onlinepubs/9699919799/utilities/V3_chap02.html#tag_18_01)
covers in technical detail the responsibilities of the shell.


## Shell language

http://pubs.opengroup.org/onlinepubs/9699919799/utilities/sh.html