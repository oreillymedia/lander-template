# lander-template

## Ipython

* Add a `index.ipynb` file
* optionally add a `Dockerfile` that with the notebook's dependencies

## Atlas Config

In `atlas.json`:

* Change `server_url` to point to a tempnb server
* Change `video_url` to point to a youtube video
* Change `poster_url` to point to a local image file (`assets/poster.png`) or to an absolute url

## Dockerfile

Basic docker file that pulls from https://hub.docker.com/r/jupyter/notebook/~/dockerfile/ 