# Credits

`index.html` carries no maps, no catalogue and no picture of anything.
Everything on the screen, the disk, the ring, the stars and the haze behind
them, is painted by the page's own shader while you watch. Nothing is loaded
from anywhere.

## How the light bends

Each pixel is a ray of light traced backwards from the eye around a
non-spinning (Schwarzschild) black hole, in units where the Schwarzschild
radius is 1. The ray's path is integrated step by step in flat coordinates
with the acceleration `-3/2 · h² · x / r⁵`, where `h` is the ray's angular
momentum; this reproduces the exact shape of a light ray's orbit around such
a hole. Rays that fall below `r = 1` go black. Rays that pass far from the
hole are bent once by the weak-field angle instead of being marched, which
is what stretches the background stars.

So the things you see are not drawn, they come out of the tracing:

- the disk arching over the top and under the bottom of the hole is the far
  side of the disk, whose light bends around to reach you;
- the thin bright line at the edge of the shadow is light that circled the
  photon sphere at `r = 1.5` before escaping. The images it carries are
  finer than any pixel, so the shader draws them as one line of light at
  impact parameter `3√3/2`, the edge of capture, with a soft warm halo;
- the second, larger ring under the shadow is the underside of the disk,
  its light bent round beneath the hole;
- the centre is black because nothing comes back from there: rays that
  fall in carry only the disk light that lies in front of them;
- one side of the disk is brighter and warmer because the gas there is
  coming towards you (Doppler beaming), softened a little so the far side
  still reads.

The disk is a thin sheet from about the last stable orbit out to twelve
radii, turning with a Keplerian profile, so the inner edge laps the outer.
Its streaks are noise in polar coordinates; because the turning shears
them tighter and tighter, two patterns take turns, each fading out before
it winds too thin. A thin haze either side of the sheet gives it its glow.
Close in, the part of the disk right under you is dimmed on purpose, so
the shadow and the ring stay the subject.

The small hash that seeds the noise and the stars follows Dave Hoskins'
*Hash without Sine* (MIT licence).

## The sound

The sound is made in the page too, from oscillators and generated noise:
a low detuned drone under a soft filter, a slow swell, a breath of filtered
noise for wind, and a faint shimmer that comes forward as you fly in. It is
off until you turn it on. If you play a song of your own, it is read from
your device and played in your browser only; it is never uploaded or stored
anywhere, and the page only listens to its bass to let the disk breathe a
little with the beat.

## The colours are not real

The rose, soft pink and warm gold are an artistic choice for Deep Field.
A real accretion disk is hot enough to glow white-orange, and the hottest
parts whiter still. The faint violet haze behind the stars is painted too.

## Inspiration

The look owes a debt to two real pictures of the same thing: the Event
Horizon Telescope's images of M87* and Sgr A*, and the black hole Gargantua
in *Interstellar*, rendered by Double Negative and described in
O. James, E. von Tunzelmann, P. Franklin and K. S. Thorne, *Gravitational
lensing by spinning black holes in astrophysics, and in the movie
Interstellar* (Classical and Quantum Gravity, 2015). Nothing is copied from
either; they are named with thanks.

w00l23 · Mina Systems
