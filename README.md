# texture-cam

A little camera that collects textures from wherever you are. One static page, no build step.

## Three versions, one app

| Path | What it is |
|---|---|
| `/` | Camera with a curved film-roll strip underneath, plus the texture gallery |
| `/camera` | Full-screen camera, edge to edge; a VIEW window opens the gallery |
| `/3d` | The camera as a solid 3D object on grey that turns with the phone's tilt |

`/camera` and `/3d` forward to `/?camera` and `/?cam3d`; all three run the same `index.html`.

## Run locally

Open `index.html` in a browser, or serve the folder (`npx serve .`). The live camera needs HTTPS (or localhost).
Add `?camera` or `?cam3d` to the URL to see the other versions.

## Deploy

`vercel.json` serves the repo root as a static site. Import the repo at vercel.com/new (preset: Other), or run `npx vercel --prod`.
