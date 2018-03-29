# Remapping Apple Keyboard for use with Linux

## Rationale

I am using a Qwerty wired aluminum Apple Keyboard with Numeric Keypad
on a Linux machine.

### Leftmost button on second row.

The leftmost button on row 2 is engraved with '§' and '±' as shifted
value.

But the keyboard generates '<' and '>'.

My personal favorite mapping is '§' and '€' for that key.

### Function keys

The function keys are only available when pressed together with the
'fn' key. Without this modifier, they are assigned to the engraved
functionality such as 'XF86AudioLowerVolume' and
'XF86AudioRaiseVolume'.

I like to switch this. I want the function keys to be available
without the fn modifier and I also want to use F13 till F19.

### Caps Lock

I do not want 'Caps Lock' so I change it into an extra 'Escape' key.

### Numeric keypad

I don't want the 'Num_Lock' key, so I turn it into an 'F20' key.
Tne 0-9 keys should always be numbers, none of the KP_ stuff.

## Usage

The .xmodmaprc file in this repo performs this remapping for me.

This file must be read by xmodmap at the startup of the session:

`xmodmap path_to_this/.xmodmaprc`

## Caveat

My settings are listed and described for informational purposes. You
may want different settings. Feel free to adapt the .xmodmaprc file to
suit your wishes.

## Reference

Some links that I found helpful when preparing this .xmodmaprc:

- [List of Keysyms Recognised by
  Xmodmap](http://wiki.linuxquestions.org/wiki/List_of_Keysyms_Recognised_by_Xmodmap)

- [FAQ: How to disable/remap a keyboard key in
  Linux?](http://www.linuxscrew.com/2008/09/15/faq-how-to-disableremap-a-keyboard-key-in-linux/)

- [xev
  manpage](http://manpages.ubuntu.com/manpages/trusty/man1/xev.1.html)

- [xmodmap manpage] (http://www.xfree86.org/4.2.0/xmodmap.1.html)


