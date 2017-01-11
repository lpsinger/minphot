# MINPHOT

Minimalist photometric data reduction pipeline. Currently, supports the [Large Monolithic Imager (LMI)](https://jumar.lowell.edu/confluence/display/DCTIC/LMI) on the [4.3-m Discovery Channel Telescope (DCT)](https://lowell.edu/research/research-facilities/4-3-meter-dct/) at [Lowell Observatory](https://lowell.edu).

## Dependencies

On Mac OS:

    $ sudo port install sextractor scamp swarp missfits py27-astropy py27-scipy
    $ pip install --user ccdproc astroquery
