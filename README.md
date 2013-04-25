Programmer Dvorak with Rdesktop
===============================

[Rdesktop][1] uses its own set of keyboard layout files.

  [1]: http://www.rdesktop.org/

    $ ls /usr/share/rdesktop/keymaps
    ar      de     en-us  fo     fr-ch  is  lt         nl     pt     sv
    common  de-ch  es     fr     he     it  lv         nl-be  pt-br  th
    cs      en-dv  et     fr-be  hr     ja  mk         no     ru     tr
    da      en-gb  fi     fr-ca  hu     ko  modifiers  pl     sl

If you want to use any layout other than `en-us`, use the `-k` option.

    $ rdesktop -k fr-ca server

I use [Programmer Dvorak][2], so I was thrilled when I [found someone][3] who
had created a keymap for it.

  [2]: http://www.kaufmann.no/roland/dvorak/
  [3]: http://permalink.gmane.org/gmane.network.rdesktop.devel/3695

Copy [en-dvp][4] to `/usr/share/rdesktop/keymaps` and you're on your way.

  [4]: en-dvp

    $ rdesktop -k en-dvp server
