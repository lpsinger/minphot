# MINPHOT

Minimalist photometric data reduction pipeline. Currently, supports the [Large Monolithic Imager (LMI)](https://jumar.lowell.edu/confluence/display/DCTIC/LMI) on the [4.3-m Discovery Channel Telescope (DCT)](https://lowell.edu/research/research-facilities/4-3-meter-dct/) at [Lowell Observatory](https://lowell.edu).

## Dependencies

The pipeline depends on the [Astr*O*matic](https://www.astromatic.net) tools, [Astropy](http://www.astropy.org), and a few [Astropy affiliated packages](http://www.astropy.org/affiliated): [CCDProc](http://ccdproc.readthedocs.io) and [Astroquery](http://astroquery.readthedocs.io).

To install these dependencies on Mac OS:

    $ sudo port install sextractor scamp swarp missfits py27-astropy py27-scipy
    $ pip install --user ccdproc astroquery

## Instructions



