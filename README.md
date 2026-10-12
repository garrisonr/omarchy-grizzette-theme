# Grizzette — the Garrison Gazette theme for Omarchy

Your whole desktop, set like the morning edition: peachy-cream newsprint
(`#FFDDB5`), chocolate ink (`#6B3816`), orange-red accents (`#FB4E00`), and
icy-blue cool highlights (`#CAE7FC`). 70s coffee-brand retrofuturism, now
with window borders. Made to sit naturally next to the Garrison Gazette,
Save-A-Tron, the Shopping List app, and the Film Database.

## What's inside

- `colors.toml` — the full palette. Omarchy renders every app config
  (terminal, bar, launcher, notifications, lock screen, editor) from this.
- `backgrounds/` — four wallpapers, cycle with `omarchy theme bg next`
  (`Super + Ctrl + Space`):
  - `grizzette.jpg` — 70s drive-in theater at dusk (default)
  - `grizzette-testpattern.jpg` — retro TV test pattern
  - `grizzette-gadget.jpg` — As-Seen-On-TV gadget ad, Ron Popeil energy
  - `grizzette-coffee.jpg` — the original coffee-ad design (alternate)
- `screensaver-logo.png` — a bold Grizzette "G" badge. Omarchy's
  screensaver shows an ASCII-art logo, and this file is drawn to convert
  cleanly. It is NOT installed by the theme — set it yourself in the
  Omarchy menu under *Style > Screensaver* (it converts PNG to ASCII for
  you).
- `preview.png` — theme-switcher preview.
- `light.mode` — marks this as a light theme.
- `FONTS.md` — the font pairing guide (fonts live outside the theme;
  see that file for the exact commands).

## Install

The easy way, straight from GitHub (replace with your username):

```bash
omarchy theme install https://github.com/<your-github-username>/omarchy-grizzette-theme.git
omarchy theme set grizzette
```

Or copy it over by hand:

```bash
# copy the theme into place
mkdir -p ~/.config/omarchy/themes
cp -r /path/to/grizzette ~/.config/omarchy/themes/

# apply it
omarchy theme set grizzette
```

Verify the ramp looks right:

```bash
omarchy dev theme-preview grizzette
```

Switch back any time with `omarchy theme set <other-theme>`.

## Font pairing

Themes can't set fonts in Omarchy — that's a separate system setting.
See `FONTS.md` in this folder for the exact commands and the recommended
retro pairing (spoiler: Victor Mono's cursive italics).

## Tweak it

It's your theme — edit `~/.config/omarchy/themes/grizzette/colors.toml`
and re-run `omarchy theme set grizzette` to regenerate everything.
Drop extra wallpapers into `~/.config/omarchy/backgrounds/grizzette/`
(they sort first and become the default on theme switch).
