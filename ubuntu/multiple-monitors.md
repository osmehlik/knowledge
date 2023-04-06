
# How To Configure Multiple Monitors

Multiple monitors can be configured using `xrandr` command.

Run this after you have connected or disconnected monitors:

```bash
xrandr --auto
```

It should disable newly disconnected monitors and enable newly connected monitors.

To find out, which monitors `xrandr` knows about, run:

```bash
xrandr --query
```

To set up screen mirroring (some monitor with same content as other monitor), run:

```bash
xrandr --output some_monitor_name --same-as another_monitor_name
```

To set up extended screen, run:

```bash
xrandr --output some_monitor_name --right-of another_monitor_name
```
