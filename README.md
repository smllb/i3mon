# i3mon

Arrange, rotate and save monitor layouts for i3 — a small X11/xrandr display manager.

## Usage

    i3mon                  # GUI, auto-loads last profile
    i3mon <profile>        # GUI with a specific profile pre-loaded
    i3mon --apply <profile># apply a layout to the live display, then exit
    i3mon --list           # list saved profiles

## Install

    cp i3mon ~/bin/i3mon

Profiles are stored as JSON in `~/.config/i3mon/<name>.json`.

### i3 autostart

    exec --no-startup-id i3mon --apply base