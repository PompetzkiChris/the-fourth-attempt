# The Fourth Attempt

The Laws of Annihilation, enacted as one cycle. Wordless, one fixed camera, exact
arithmetic. Click to pause; `#t=<seconds>` seeks; `#t=<seconds>&p` opens paused on
that frame.

**Watch it:** https://pompetzkichris.github.io/the-fourth-attempt/

A single self-contained HTML file. No fonts, no CDN, no images, no network of any
kind — one inline script and a canvas.

## What it is

`M = [[1,2,3],[2,4,7],[2,4,7]]` has rank 2 and kernel `span(-2,1,0)`. The fourth
mutually unbiased basis at d = 6 needs three directions in a three-dimensional
candidate space; the unimodular triple `(7,0,-2)`, `(-3,0,1)`, `(-2,1,0)` maps to
`(1,0,0)`, `(0,1,1)`, `(0,0,0)`. The kernel eats one. Two stand where three are
required, so `rank 2 + nullity 1 = 3` and the fourth basis cannot close.

- **Hue** is the kernel fraction `kf(v) = |v·k|/|v|`, fixed for the whole loop:
  700 nm red for a point wholly in the surviving image, 400 nm violet for one
  wholly in the kernel. Wavelength becomes light through the CIE 1931 2-degree
  standard observer and the exact IEC 61966-2-1 matrix to sRGB.
- **Brightness** is the surviving amplitude
  `live(v,t) = sqrt(1 - kf^2 + kf^2 (1-t)^2)` — 1 for every point at t = 0,
  0 exactly at t = 1 for a point wholly in the kernel.
- **White is reserved for the mutually unbiased bases** and nothing else.
- The **scale ladder** runs thirty-three decades on one axis, from the observable
  universe to a foveal cone, and the camera never turns.
- It is **one cycle**: the frame at t = 336 s is the frame at t = 0, pixel for
  pixel, verified across all 504,000 pixels at zero channel difference.

`verify.rkt` in the working tree certifies the elimination exactly in Racket.
