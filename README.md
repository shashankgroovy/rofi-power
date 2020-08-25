Rofi-power
==========

A simple rofi script for power management.

And just has one system dependency `systemd`

Usage
------
### Bind in i3:

```
# start rofi
bindsym $mod+Escape exec --no-startup-id ~/.config/rofi-power/rofi-power
```

### Use with polybar:

```
[module/power]
type = custom/script
exec = /path/to/rofi-power/rofi-power --show

format = <label>
format-background = ${color.shade1}
format-foreground = ${color.modulefg}
format-padding = 3

click-left = /path/to/rofi-power/rofi-power &
```

![scrot](scrot.png)

> Note: It might look different on your system. I am using onedark theme in
> rofi with compton for transparency
