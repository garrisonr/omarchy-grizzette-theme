# Fonts for the Grizzette look

Short version: **a theme can't set your fonts.** Omarchy themes only carry
colors and backgrounds — fonts are a separate system-wide setting. But
here's the pairing that sells the newsprint vibe:

## The one command that matters

Omarchy uses one monospace font for the terminal, the top bar, the menus,
and the launcher, all at once:

```bash
omarchy font list      # see what's installed
omarchy font current   # see what's active
omarchy font set "VictorMono Nerd Font"   # the retro pick (match the exact name from the list)
```

## Recommendations

- **Default (safe):** JetBrainsMono Nerd Font — what Omarchy ships. Clean,
  great glyph coverage, zero risk.
- **The Grizzette pick:** Victor Mono (Nerd Font version) — its cursive
  italics are pure 70s, which is exactly the energy of this theme. Install
  it from the Omarchy menu under *Install > Style > Font* if it's not in
  your list, then set it with the command above.
- **Also worth a look:** Fira Code, Iosevka, Cascadia Mono — all installable
  from that same menu.

## If you want a serif for documents and GTK apps

That's outside Omarchy's font command — it's a GNOME/GTK setting:

```bash
gsettings set org.gnome.desktop.interface document-font-name 'Serif 12'
```

Swap in any serif you have installed (check with `fc-list : family | grep -i serif`).
This only affects document-viewing apps, not the bar or terminal.
