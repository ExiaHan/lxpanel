# lxpanel
Pulled from lxde site.

***

LXPanel is a lightweight X11 desktop panel.

To build this program you need some development packages:
  libtool 2.2 or newer, intltool, libgtk 2.18 or newer,
  libfm-gtk 1.2 or newer, libwnck, libkeybinder.
Optional development packages may be required to build some modules:
  libmenu-cache,
  libalsasound ('volumealsa' plugin isn't built if missing),
  libindicator 0.3.0 ('indicator' plugin isn't built if missing),
  wireless-tools (required to build 'netstat' plugin),
  libxml-2.0 (required to build 'weather' plugin).

To install this program, three other packages are needed:
  menu-cache, libfm-gtk, lxmenu-data.
Please install them before installing lxpanel.

There are 2 programs contained in the package.

1. lxpanel: the panel

2. lxpanelctl: the controller of lxpanel, can be used to control lxpanel in 
               other programs.  The best place to use lxpanelctl is by far 
               the numerous key bindings provided by window managers.
               When the key combination is pressed, call lxpanelctl to popup
               system menu, or to open run dialog in lxpanel.
               Run lxpanelctl without any argument to see what command it 
               currently recognizes.


About Netstat and Netstatus plugins:

1. netstatus was ported from netstatus panel applet of GNOME Project.  This
   plugin has good support on Linux/BSD/other UNIX, and it is released under
   GNU GPL. (the same as LxDE)

2. netstat is a new plugin written by LxDE developers as the lightweight
   replacement of netstatus plugin.  It aims to be more usable and resource
   efficient.  At the current stage, netstat runs only on Linux.


About theming & lxpanel:

1. LXPanel tries to use as much themed icons as possible.  Fallback icons
   may be also provided if they are placed into $(datadir)/lxpanel/images
   directory.  Few plugins already provide their fallback icons.

2. Current icon names that can be themed specifically for lxpanel include:
	*"lxpanel-background"
	*"clock"
	*"capslock-on"
	*"capslock-off"
	*"numlock-on"
	*"numlock-off"
	*"scrllock-on"
	*"scrllock-off"
	*"window-manager"
	*"ns-lock"
	*"cpufreq-icon"
	*possibly more, as yet unfound.

There are also a substantial amount of others, but they use the icon naming specification.

3. You can also set theme for any plugin specifically using it's widget name
    which is equal to plugin type.

4. There is a specific RC file which can be loaded by LXPanel, it can be placed
    as ~/.config/lxpanel/$PROFILE/gtkrc, where $PROFILE is the profile used on
    the LXPanel start.


About keyboard options translations in xkb plugin:

The 'xkb' plugin can use translations from language packs that are present
    in many distributions. To use it you should have language pack which
    includes "xkeyboard-config" translations.
