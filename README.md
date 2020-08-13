# Material for the session "Introduction to Deep Learning in R for the analysis of UAV-based remote sensing data"

*OpenGeoHub summer school 2020*


# Installation

Install a current version of R and the following packages:

`install.packages(c("keras","tfdatasets","mapview","stars","rsample","gdalUtils","purrr", "magick", "jpeg"))`

Install miniconda, keras and tensorflow python dependencies:

- `reticulate::install_miniconda()`
- `keras::install_keras()`

For installing dependencies of rgdal, stars and magick on linux:

- gdal:`sudo apt-get install gdal-bin libgdal-dev`

- stars: `sudo apt-get install libudunits2-dev`

- magick: `sudo apt-get install libmagick++-dev`

Download and unzip the turoial data from:
https://docs.docker.com/docker-for-windows/install/


# Docker

If you are in for using Docker, I´ve prepared a Docker image that includes all software and data for the tutorial. To use it, download and install Docker:

- Linux: https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository
- Windows: https://docs.docker.com/docker-for-windows/install/
- Mac: https://docs.docker.com/docker-for-mac/install/

Then:

- in your terminal (or power shell) type: docker run -d -p 8788:8787 dachro/oghss:latest
    - `8788` on the left side of the `:` is the port on your host system. You can use any other available port that your prefer
- after the container has been built and started, open you browers and go to `localhost:8788/` (or whatever port you have chosen)
- you should see the rstudio server login page. Log in via username: rstudio and password: rstudio
