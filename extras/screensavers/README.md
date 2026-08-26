# Optional screensaver sources

These 1600×900 high-contrast images are source material for Omarchy's
image-to-ASCII screensaver workflow. Each message is contained inside a
physical retro-CRT terminal so the optional imagery follows the wallpapers'
diegetic-text rule. Their transparent backgrounds are intentional: Omarchy's
stock converter uses the alpha channel as its artwork mask. They are not
activated by installing this theme.

- `public-access-read-only.png`
- `voice-received-policy-unchanged.png`

Use them manually only if you want to change your screensaver content.

```bash
omarchy transcode ascii public-access-read-only.png ~/.config/omarchy/branding/screensaver.txt
omarchy launch screensaver
```
