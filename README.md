Rofi-power
==========

A simple rofi script for power management.

And just has one system dependency `systemd`


Usage
------
Bind in i3:

```
# start rofi
bindsym $mod+Escape exec --no-startup-id ~/.config/rofi-power/rofi-power
```

Use with polybar:

```
[module/power]
type = custom/script
exec = ~/.config/rofi-power/rofi-power --show

format = <label>
format-background = ${color.shade1}
format-foreground = ${color.modulefg}
format-padding = 3

click-left = ~/.config/rofi-power/rofi-power &
```
