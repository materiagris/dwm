# dwm
Suckless dwm configuration and customization

dwm version: 6.2

## Installation
```
# cd /usr/src
# git clone git://git.suckless.org/dwm
```

## Most prominent changes in config.def.h

- Terminus font
```
static const char *fonts[]          = { "xos4 Terminus:size=15" };
static const char dmenufont[]       = "xos4 Terminus:size=15";
```

- Gray color
```
static const char col_cyan[]        = "#696969";
```

- Floating Layout icon: from '><>' to '(~)'
```
     { "(~)",      NULL },    /* no layout function means floating behavior */
```

- MODKEY definition
```
#define MODKEY Mod4Mask
```
- Keys customization
```
    { MODKEY,           XK_Return,    spawn,          {.v = termcmd } },    
    ...
    { MODKEY,           XK_BackSpace, zoom,           {0} },
```

## Patches

- Vanitygaps (adds gaps between windows): dwm-vanitygaps-20190508-6.2.diff
