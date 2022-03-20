# mL-nodeapp
My own version of the node application door for Mystic, inspired by Carlos Roldan aka Necromaster's original version.

## Installation:
To install this door, you will need to;
- Copy `scripts/mL-nodeapp.mpy` into your Mystic scripts directory for the theme you are using
- Copy `text/mL-nodeapp` directory and all subdirs/files into your Mystic text directory for the theme you are using

## Mystic menu item;
Create a menu item like this;

```
║ Display Text  │  ]n[   tqwnEt aPPLy   ]n[                                   ║
║ LightBar OFF  │                                                             ║
║ LightBar ON   │                                                             ║
║ LightBar X Y  │ 0   0                                                       ║
║ Hot Key       │ N                                 ┌ GRID MENU JUMPS ─────── ║
║ Access String │ s20                               │ Up     00    Escape  00 ║
║ Display When  │ User has access                   │ Down   00    Tab     00 ║
║ Redraw After  │ Yes                               │ Left   00    PageUp  00 ║
║ Execute Timer │ 0                                 │ Right  00    PageDn  00 ║
║ Timer Type    │ Every <timer> interval            │ Home   00    End     00 ║
║                                                                             ║
║ Action List ────────────── Access ───── Data ─────────────────────────────  ║
║ (GY) Execute Python 2 Scri              mL-nodeapp netname                  █
```

There is one argument being passed, and that is the network name you wish to get node applications for. You can have multiple networks, you can just add a menu entry for each network and configure each network like this;

## Network configuration file
In your theme's text directory, where you copied the `mL-nodeapp` directory into, you will see some example configs;

mL-nodeapp
└── nets
    ├── retronet
    │   ├── header.ans
    │   └── net.ini
    └── tqwnet
        ├── header.ans
        └── net.ini

You will see there is a config file called `net.ini`, in here are various options for things like colour schemes and infopack location etc. Here's the tqwnet net.ini config;

[network]
netName = tqwnet
netSysop = MeaTLoTioN
netAddress = 1337:1/101
header = header.ans
infoPack = /mystic/files/tqw/tqw_info/tqwinfo.zip
brightColour = 11
normColour = 03
fieldBG = 17
fieldFG = 15
normBG = 16
menuOption = 14


