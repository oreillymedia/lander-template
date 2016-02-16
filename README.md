# lander-template

## Using this template in Atlas

When creating a [new project](https://atlas.oreilly.com/new):

* Click `Advanced`
* Select `Custom`
* Fill in the git url as: https://github.com/oreillymedia/lander-template.git

## Theme

This template uses the `oreillymedia/lander-theme` at https://atlas.oreilly.com/oreillymedia/lander-theme

## Ipython

* Upload / commit a `index.ipynb` file
* optionally update the `Dockerfile` that with the notebook's dependencies

## Atlas Config

In `atlas.json`:

* Change `server_url` to point to a tempnb server
* Change `video_url` to point to a youtube video
* Change `poster_url` to point to a local image file (`assets/poster.png`) or to an absolute url
* Change `cues_url` to point to a local image file (`assets/cues.json`) or to an absolute url

## Lander

This template links directly to remote versions of the js libraries it requires.

You can change these by adjusting changing the following in `atlas.json`:

```json
"javascripts" : [
  "https://cdn.oreillystatic.com/oreilly/scripts/lander/video.js",
  "https://cdn.oreillystatic.com/oreilly/scripts/lander/thebe.js",
  "https://cdn.oreillystatic.com/oreilly/scripts/lander/lander.js"
],
"stylesheets" : [
  "https://cdn.oreillystatic.com/oreilly/scripts/lander/video-js.css",
  "https://cdn.oreillystatic.com/oreilly/scripts/lander/lander.css"
]
```

You can add local versions of Lander and videojs, from the assets folder:

```json
"javascripts" : ["assets/video/video.js","assets/lander/lander.js"],
"stylesheets" : ["assets/video/video-js.css","assets/lander/lander.css"]
```

This will be uploaded to our cdn when they are imported into the [curator](https://curator.oreilly.com/).

## Dockerfile

Basic docker file that pulls from https://hub.docker.com/r/jupyter/notebook/~/dockerfile/