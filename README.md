# Swytcher

> A small program that listens to X events and changes your keyboard layout.

Use setxkbmap to configure your different keyboard layouts.

E.g.,

```bash
setxkbmap -option ''  # clear previous options
setxkbmap \
	-option grp:shifts_toggle \  # toggle layout by lshift+rshift
	-option grp_led:caps \  # caps led indicates secondary layout
	-option caps:escape \  # map caps to escape
	\  # set US layout as first, Swedish as second, US intl as third:
	"us,se,us(altgr-intl)"
```

## TODO

* Add tests  ☑

* Create setup.py ☑

* Private repo on bitbucket? ☑

* Add config file ☑
    * Use config-file ☑

* Check that package can be installed
    * Figure out how to include config files in the package

* Finish README.md

* Publish on Github

* Publish to PyPi

* When finished, add my program to
  http://unix.stackexchange.com/questions/12072/how-do-i-get-current-keyboard-layout#

* Debian package?

More functionality:

* Executable to toggle layout
* Remember layout for windows
    * Should be easy to implement using the default fallback
    * but I need to get unique window id to check against
