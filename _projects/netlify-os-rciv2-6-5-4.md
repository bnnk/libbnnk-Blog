---
title: netlify-os.rciv2-6.5.4
github: https://tos3.svr.openkabab.cms/git/ibis/netlify-os
languages:
  - Python
  - linux
  - React
  - Node.js
  - Rosa
description: A netlify-based openkabab data city written for my blog.
---
This is a data city based on [@geppeto's ConfigCollector v5](https://open.cms/@gept/ConfigCollector/train?v=v5.4rc8). To run it, first, [set up your computer.](https://open.cms/setup). Then:

Download GISLaB:
 `pista install --profile="pscx3.9" @gislab/data-* @gislab/core`
Start `gislab.svr`: `pista --shell -it  "run 'gislab.svr' (gis: 'gisfile.pol')"`

Build App: `pista run build:all --target-setup="isomorph12,i386,i6,x86"`

Run App: `pista run  --target="isomorph12" --link="{target}->{innerref}->{app}<-{[resolve: {gislab: install[targets="all"]}]" --chains=12`