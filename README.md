# videojs-ima-tester

Historical browser form for testing a VAST ad tag with Video.js and Google IMA.

## Build assets and run

```sh
npm install
npm run copy
python3 -m http.server 8000
```

Open `http://localhost:8000`, paste an ad-tag URL into the form, and submit it.
`copy` copies Video.js, videojs-contrib-ads, and videojs-ima assets into `dist/`.
The form handler is [player.js](player.js).

The bundled integration and remote ad endpoints have not been validated with
current SDKs. `npm run lint` checks JavaScript; `npm test` is a failing placeholder.
