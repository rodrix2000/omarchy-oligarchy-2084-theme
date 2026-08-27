# Validation report

Validated on 2026-08-26 against Omarchy `4.0.1-1` and the Quattro branch at
commit `0ae1694830b6bd9511042fe1b89a0062d8c083cb`. The billboard-compositing
correction and the seven-wallpaper satirical copy revision were installed and
revalidated live on 2026-08-27.

## Installation and staging

- PASS — Installed from the public GitHub URL with `omarchy theme install`.
- PASS — Repository name resolved to the expected slug `oligarchy-2084`.
- PASS — Theme activated as `Oligarchy 2084`.
- PASS — Seven backgrounds staged and cycled in filename order; the live
  desktop was left on `Preferred Future` for the unobstructed preview layout.
- PASS — Hand-written `colors.toml`, `btop.theme`, `chromium.theme`,
  `icons.theme`, and `keyboard.rgb` survived remote-theme staging.
- PASS — Omarchy regenerated the filtered terminal, editor, Hyprland, and
  shell files from `colors.toml`.
- PASS — `hyprctl configerrors` returned no errors after activation and reload.

## Live surface checks

- PASS — Omarchy shell/bar rendered the active palette.
- PASS — Root menu rendered readable normal, selected, and bordered states.
- PASS — Notification card rendered readable text and gradient border.
- PASS — Background image picker rendered all seven images, opened on the exact
  current background, and displayed a clear selected border.
- PASS — Foot rendered normal/bright ANSI colors, selection, and cursor states.
- PASS — btop rendered CPU, memory, graph, meter, and box colors from the
  included theme.
- PASS — Nautilus rendered the selected Yaru-blue icon treatment and readable
  dark surfaces.
- PASS — Chromium policy output resolved to the included `7,10,18` frame color
  (`#070A12`).
- PASS — Active and inactive Hyprland borders remained distinct over the hero
  wallpaper.
- PASS — The official Plymouth preview workflow generated
  `preview-unlock.png` with the emblem, entry, bullets, and lock icon visible.
- PASS — `preview.png` is a native 1440×900 screenshot of the running system,
  not a conceptual mockup. Its application windows occupy the left half while
  the Preferred Future campaign display remains fully visible on the right.
- PASS — Privately Held and Preferred Future were captured unobstructed at the
  live 1440×900 desktop crop after the correction. Neither contains a duplicate
  panel edge, and no text crosses the physical billboard frame.
- PASS — All seven revised campaign messages were inspected at their native 4K
  resolution, in the contact sheet, and as live 1440×900 desktop crops. The
  longer pre-recorded, premium-feature, and outcome-locked lines remain legible
  and contained by their physical displays.

The actual lock and polkit credential flows were not submitted during automated
validation. Their generated shell sections were inspected for background,
foreground, placeholder, active, and error roles, and the official unlock
preview was rendered. Helix and VS Code were not installed on the target;
Omarchy's generated files for those applications were present and non-empty.

## Contrast and color separation

Measured using WCAG relative luminance:

| Pair | Ratio |
| --- | ---: |
| Foreground / background | 17.47:1 |
| Muted / background | 4.85:1 |
| Selection text / selection | 12.16:1 |
| Accent / background | 11.17:1 |
| Urgent / background | 6.29:1 |

The closest pair among the six normal ANSI hues was green/cyan at ΔE76 25.1,
which remained visually distinct in the live Foot sample.

## Asset and safety checks

- PASS — Seven final backgrounds are 3840×2160 sRGB.
- PASS — Seven textless masters are 3840×2160 sRGB.
- PASS — Four ultrawide variants are 3440×1440 sRGB.
- PASS — Physical-CRT screensaver sources are transparent 1600×900 RGBA assets
  and transcode through Omarchy's default image-to-ASCII command.
- PASS — Social card is 1200×675.
- PASS — All raster files decoded successfully.
- PASS — No symlinks, executable files, code-bearing theme payloads, font
  binaries, generated caches, secrets, or local paths are part of the release.
- PASS — Deprecated visuals and copy are absent from release imagery, filenames,
  README copy, metadata, previews, and social assets. The internal asset audit
  records their exclusion as required by the handoff.

## Contest preflight

The announcement supplied by the project owner was reviewed through the
publisher's embed endpoint on 2026-08-26. It asks for an Oligarchy theme that
is both funny and good-looking enough to ship, sets the deadline to Friday
2026-08-28, and requests submissions by email to `david@omarchy.org`. No email
has been sent.

## Known validation limits

- Dedicated ultrawide files were dimension- and composition-checked but the
  target laptop has no 3440×1440 monitor.
- Recheck that the live announcement has not changed immediately before
  submission; no contest email or post was sent as part of this build.
