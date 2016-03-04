# Remapping Apple Keyboard for use with Linux

## Rationale

I am using a Qwerty wired aluminum Apple Keyboard with Numeric Keypad
on a Linux machine.

### Leftmost button on second row.

The leftmost button on row 2 is engraved with a '§' and a '±' as
shifted value.

But the keyboard generates '<' and '>'.

My personal favorite mapping is '§' and '€' for that key.

### Function keys

The function keys are only available when pressed together with the
'fn' key. Without this modifier, they are assigned to the engraved
functionality such as 'XF86AudioLowerVolume' and
'XF86AudioRaiseVolume'.

I like to switch this. I want the function keys to be available
without the fn modifier and I also want to use F13 till F19.

## Usage

The .xmodmaprc file in this repo performs this remapping for me.

This file must be read by xmodmap at the startup of the session:

`xmodmap path_to_this/.xmodmaprc`


## Reference

Some links that I found helpful when preparing this .xmodmaprc:

- [List of Keysyms Recognised by
  Xmodmap](http://wiki.linuxquestions.org/wiki/List_of_Keysyms_Recognised_by_Xmodmap)

- [FAQ: How to disable/remap a keyboard key in
  Linux?](http://www.linuxscrew.com/2008/09/15/faq-how-to-disableremap-a-keyboard-key-in-linux/)

- [xev
  manpage](http://manpages.ubuntu.com/manpages/trusty/man1/xev.1.html)
