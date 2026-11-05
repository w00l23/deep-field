# Credits

`index.html` loads nothing. The stars, their paths, the sky behind them and
the light curve are all drawn by the page itself on a 2D canvas.

## How they move

Each pair follows its real orbit. Every frame the page solves Kepler's
equation for where the pair is along its ellipse, then splits that between
the two stars by their masses, so both turn about their shared centre of
mass (the small cross). Each orbit is sped up to last 14 to 26 seconds.

## The light curve

The strip under the stars is the light a distant eye would get, looking
from wherever you have turned the view, over one whole orbit. Where the
near star's disc covers part of the far one, the far star's light is lost in
proportion to the covered area (uniform discs, no limb darkening). Turn a
pair edge-on and the dips appear; turn it face-on and the line goes flat.

## Sizes

Algol is drawn true to size against its orbit. Alpha Centauri and Sirius are
not: their stars are hundreds or thousands of times smaller than their
orbits, so they are enlarged to be seen, and any eclipse they show when you
turn them edge-on comes from those enlarged discs.

## Numbers

Approximate published values, rounded:

| Pair | Period | Eccentricity | Inclination | Masses (suns) | Luminosities (suns) |
|---|---|---|---|---|---|
| Alpha Centauri A, B | 79.9 years | 0.52 | 79.2° | 1.08, 0.91 | 1.5, 0.5 |
| Sirius A, B | 50.1 years | 0.59 | 136.3° | 2.06, 1.02 | 25.4, 0.056 |
| Algol Aa1, Aa2 | 2.867 days | ≈ 0 | 98.6° | 3.17, 0.70 | 182, 6.9 |

Sources: Pourbaix & Boffin 2016 and Kervella et al. 2016 (Alpha Centauri);
Bond et al. 2017 (Sirius); Baron et al. 2012 (Algol). Algol's third star,
far out on a 680-day orbit, is left out. Star colours are chosen to match
each star's type, not measured.
