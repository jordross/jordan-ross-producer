# Screenshots

Drop 2–4 images per project (jpg/png/webp). Suggested names:

- `swagflip/01.jpg` … `02.jpg`
- `truedirt/01.jpg` … `03.jpg`
- `freeride/01.jpg` … `02.jpg` plus `logo.png`
- `freeride/gameplay-60.mp4` + `gameplay-poster.jpg` (in-engine 720p60 clip)

Then in `index.html`, replace each placeholder like:

```html
<div class="shot">Add screenshot<br /><code>images/swagflip/01.jpg</code></div>
```

with:

```html
<div class="shot has-image"><img src="images/swagflip/01.jpg" alt="SWAGFLIP gameplay" /></div>
```

Tips: gameplay/in-engine stills beat splash art alone. Keep stills under ~500KB each when you can. The Freeride clip is a compressed web MP4.
