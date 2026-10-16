# Deep Field

Quiet, interactive simulations of the space around us, in one place.

**Live:** https://w00l23.github.io/deep-field/

| Folder | What it is |
|---|---|
| [`solar-system/`](solar-system/) | The Sun, its planets and their moons, where they really are today. One HTML file, raw WebGL. |
| [`solar-system/original/`](solar-system/original/) | The first sketch of it: eight planets on circles, canvas 2D. |
| [`wormhole/`](wormhole/) | A small ship leaves Earth, tears space open and comes out at Saturn. three.js from a CDN. |
| [`scale-zoom/`](scale-zoom/) | From an atom to the edge of the universe. Coming soon. |

Every page is plain HTML with nothing to build. To run it locally, serve the
folder (for example `python3 -m http.server`) and open `http://localhost:8000`.

The sims were copied in unchanged from their own repos
([solar-system](https://github.com/w00l23/solar-system),
[wormhole](https://github.com/w00l23/wormhole)); the only addition is a small
"‹ Deep Field" link back to this page. Where their maps and star data come
from is in each folder's `CREDITS.md`.

## Licence

Code under the [MIT licence](LICENSE). The maps and star data inside the sims
keep their own terms; see each `CREDITS.md`.

w00l23 · Mina Systems
