# Agentic Design Systems hero video

A muted, autoplay video that plays once and then stops fills the hero slot on `agentic-ds.html`
(1025 x 713, about 1.44:1; it is scaled to fill and cropped to that frame).

| File | What it is |
|---|---|
| `hero.mp4` | The video (H.264). Keep it **under ~10 MB** so the page stays fast. |
| `hero-poster.jpg` | A still frame: shown while the video loads and for reduced-motion visitors. |

Until `hero.mp4` exists the slot shows a labelled placeholder.

Browsers only autoplay **muted** video, so it starts silent. A slim control bar
(over the bottom of the video) lets visitors play/pause, drag the timeline, replay
after it ends, and unmute. Pausing sticks; reduced-motion visitors see the poster
until they press play. The icons are drawn in the css.gg style; to use the exact
css.gg SVGs, swap the inline `<svg>`s inside `.vc` in `agentic-ds.html`.

## Compressing a big export

GitHub's web uploader accepts files up to 25 MB (a normal `git push` up to 100 MB),
and a hero should be far smaller than that. This keeps 1280 px wide, strips audio:

```bash
ffmpeg -i input.mov -vf "scale=1280:-2" -c:v libx264 -crf 28 -preset slow -an -movflags +faststart hero.mp4
```

Make the poster from the first frame:

```bash
ffmpeg -i hero.mp4 -frames:v 1 -q:v 3 hero-poster.jpg
```
