# Graph-Tool Custom Image

This is the same image as `tiagopeixoto/graph-tool`, with pip installed so that a `requirements.txt` file can be used to install additional python packages.

There is also a `docker-compose.yml` file, so you can get a notebook up and running with `docker-compose up`.

## Modifying Requirements

If you want to customize this for yourself, the fastest way would be `git clone https://github.com/pmbaumgartner/graph-tool-pip`. Edit your `requirements.txt` file from there, and then `docker-compose up` should rebuild the image with the additional packages you've installed, and `docker-compose build` will force a rebuild.

## Docker Image

Use `docker pull pbaumgartner/graph-tool-pip` if you wish to use this specific image. It has `kmapper==1.2.0` in the `requirements.txt` file.