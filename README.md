# Hack the Planet

A late-90s cyberpunk theme for Omalauncher / Omarchy: terminal black, acid
green, electric cyan and hot magenta, with a bitmap Gibson-mainframe wallpaper.

## In this repo

- `colors.toml` — the theme palette.
- `backgrounds/1-gibson.png` — 1440×3120 bitmap wallpaper: 4 px blocks, 44-colour
  quantise, scanlines. A wireframe mainframe tower over a perspective grid and
  a neon skyline.
- `widget/agenda.owl` — optional 3×6 phone-agenda widget.
- `widget/preview.png` — sanitized tile preview (sample events only).

## Install

Clone this repo as a theme directory:

```sh
gh repo clone Bekkenes/hack-the-planet ~/.config/omarchy/themes/hack-the-planet
```

Then set it in `~/.config/omalauncher/style/style.toml`:

```toml
theme = "hack-the-planet"
```

or pick it in Settings › Style. Changes show within a second.

The wallpaper is the theme's first background. `backgrounds/1-gibson.png` is
the master; the launcher centre-crops it.

Optional widget:

```sh
cp widget/agenda.owl ~/.config/omalauncher/widgets/
owl-check ~/.config/omalauncher/widgets/agenda.owl
```

It reads the phone's calendars through `android.calendar` and asks for
permission on first tap. Nothing is read before that.

## Screen fit

The wallpaper is composed for a 9:19.5 master with the mainframe centred. It
was checked against:

- phone 9:20 and 9:16
- fold inner 5:6 and fold cover
- landscape 20:9 and 6:5
- tablet 16:10
- square

The tower stays centred and readable across those crops.

## License

MIT. Original fan art inspired by *Hackers* (1995); not affiliated with the
film. The widget is MIT as well.
