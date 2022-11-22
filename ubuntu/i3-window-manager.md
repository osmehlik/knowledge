
# How to use i3 window manager on Ubuntu

**This article is a work-in-progress.**

## What is i3?

[i3](https://i3wm.org/) is a window manager for Linux.

## Why use i3?

- **i3 can be effectively controlled using keyboard shortcuts** (so you can manipulate windows fast)
- **i3 is lightweight on system resources** (so it works on slow computers)
- **i3 makes windows use all available screen space** (so no waste of screen space)
    - There are exceptions such as dialog windows.

## How to start using it?

You can install i3 using the following command:

```bash
sudo apt install i3
```

**Important**: You should print [i3 - Reference Card](https://i3wm.org/docs/refcard.html)
before you start using it, otherwise you will not know, how to use it.

After you installed i3 and printed the reference card,
you can logout and on login screen you should be able to select i3.

## Customizing i3

Read [i3 User's Guide](https://i3wm.org/docs/userguide.html)
to learn about how to do basic configuration of i3.

### How to set a background image

You can use `feh` application to set a background image.

You can install `feh` using the following command:

```bash
sudo apt install feh
```

After you have `feh` installed,
add the following line to your `~/.config/i3/config`
to set a background:

```
exec_always --no-startup-id feh --bg-scale ~/path_to_some_image.png
```

After you have added the previous line to your configuration file,
restart i3 to see your background.

### Alternative application launchers

By default, i3 uses `dmenu` to show an application launcher.

There are other application launchers available, such as `rofi`,
which can (depending on in which mode you start it)
serve as an application launcher,
or a window switcher.

You can install `rofi` using the following command:

```bash
sudo apt install rofi
```

