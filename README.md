# Deep Field

*Small windows into a very big sky.*

Deep Field is one calm place for a set of quiet, interactive simulations of
the space around us, made by a self-taught builder at night, in plain HTML,
with Claude as pair programmer.

**Live:** https://w00l23.github.io/deep-field/

## Projects

| Project | What it is | Folder |
|---|---|---|
| [Solar System](https://w00l23.github.io/deep-field/solar-system/) | The Sun, its planets and their moons, where they really are today. One HTML file, raw WebGL. | [`solar-system/`](solar-system/) |
| [The original sketch](https://w00l23.github.io/deep-field/solar-system/original/) | The first version of it: eight planets on circles, canvas 2D. | [`solar-system/original/`](solar-system/original/) |
| [Wormhole](https://w00l23.github.io/deep-field/wormhole/) | A small ship leaves Earth, tears space open and comes out at Saturn. three.js from a CDN. | [`wormhole/`](wormhole/) |
| Scale Zoom | From the width of an atom to the edge of the observable universe. Coming soon. | [`scale-zoom/`](scale-zoom/) |

## Run it locally

Every page is plain HTML with nothing to build. Serve the folder and open it:

```sh
python3 -m http.server 8000
# then open http://localhost:8000/
```

The wormhole loads three.js from jsDelivr, so it needs a network connection;
everything else runs offline. The 404 page links home through the site's
path on GitHub Pages (`/deep-field/`), and falls back to `/` on localhost.

## How it is put together

- `index.html` is the hub: a canvas starfield and a card for each project.
- Each sim is copied in unchanged from its own repo
  ([solar-system](https://github.com/w00l23/solar-system),
  [wormhole](https://github.com/w00l23/wormhole)). The only additions are a
  page title, a description and share tags in its `<head>`, and a small
  "‹ Deep Field" link in the top-left corner back to the hub.
- `assets/` holds the card previews, the share images and the icons;
  `404.html` is what GitHub Pages shows for any missing path.

## Credits and data sources

The maps, orbits and star positions inside the sims are other people's
measurements and pictures:

- **NASA**: Earth Observatory (Blue Marble, Black Marble) and the Goddard
  Scientific Visualization Studio (CGI Moon Kit, Deep Star Maps 2020).
- **NASA / JPL**: Solar System Dynamics for the planets' orbits and the
  Horizons system for the moons, dwarf planets, comets and spacecraft; the
  Cassini mosaic of Jupiter with the Space Science Institute.
- **USGS Astrogeology**: the Mars, Io, Europa, Ganymede and Callisto mosaics
  (NASA / JPL / USGS).
- **NASA / JHUAPL**: Mercury from MESSENGER (with the Carnegie Institution)
  and Pluto from New Horizons (with SwRI).
- **ESA / Gaia / DPAC**: the star counts under the Milky Way and most of the
  stellar parallaxes; **SIMBAD** at CDS, Strasbourg, for the distances; the
  **Yale Bright Star Catalogue** (5th ed., Hoffleit & Warren) via CDS.
- The **IAU** Working Group on Cartographic Coordinates and Rotational
  Elements, and J. Meeus, *Astronomical Algorithms*, for how each body is
  turned and how bright it looks.
- **three.js** (MIT licence) renders the wormhole.

Each sim's folder has the full table in its `CREDITS.md`
([solar system](solar-system/CREDITS.md), [wormhole](wormhole/CREDITS.md)),
including how each map was reduced or changed. The pictures are public
domain (NASA, USGS); Gaia and SIMBAD ask to be named.

Built with [Claude](https://claude.ai) as pair programmer.

## Licence

Code under the [MIT licence](LICENSE). The maps and star data inside the sims
keep their own terms; see each `CREDITS.md`.

w00l23 · Mina Systems
