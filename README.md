# Off-Road Velociraptor Safari (WebGL)

Unity WebGL build mirrored from [blurst.com/raptor-safari](https://blurst.com/raptor-safari). The game must be served over **HTTP**; opening `index.html` via `file://` will not load WebAssembly reliably.

## Run locally

From this directory:

```bash
python3 -m http.server 8765 --bind 127.0.0.1
```

Then open **http://127.0.0.1:8765/** in your browser.

Other static servers work the same way, for example:

```bash
npx serve -l 8765
```

Stop the server with **Ctrl+C** when you are done.

## Production (Vercel)

Hosted on the **Trevor’s Pro** team (`trevsm-s-team`), not the Hobby team.

**URL:** **https://raptor-safari.vercel.app/** (GitHub integration is on this Pro project.)

Manual deploy from this directory:

```bash
vercel --prod --scope trevsm-s-team
```

If the site asks for a Vercel login in the browser, open the project in the [Vercel dashboard](https://vercel.com) → **Settings** → **Deployment Protection** and allow public access for the environments you want (for a small static game, turning protection off on Production is typical).
