# Workspaces

[Omarchy](https://omarchy.org)'s workspace indicators with two additions. It is a copy of Omarchy's built-in `omarchy.workspaces` widget and replaces it on the bar.

- **Hidden windows.** When a workspace holds a full-size window (maximized or fullscreen), its button takes the theme's active window border color and the count of windows behind it is cut out of the glyph, so the digits read on any theme. The tooltip says how many windows the full-size one hides.
- **Secondary laptop panel.** A laptop panel (`eDP-*`) beside an active external monitor lists only its first workspace, for setups where the external monitor holds the workspaces and the laptop panel is a side display.

Everything else is Omarchy's widget as it was when copied.

## Install

```bash
scripts/install workspaces
omarchy plugin enable io.github.ltecosta.workspaces
```

Put it where `omarchy.workspaces` was and take that one off the bar. The manifest declares itself a clone of `omarchy.workspaces`, which gives it the same access to Omarchy's services.

## Keeping up with Omarchy

Being a copy, it does not follow changes Omarchy makes to its own widget. After an Omarchy update, compare it with `$OMARCHY_PATH/shell/plugins/bar/widgets/Workspaces.qml` and carry the changes over.

## License

MIT. Based on Omarchy's workspaces widget, © David Heinemeier Hansson, MIT; both notices are in [LICENSE](LICENSE).
