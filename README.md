# MINPHOT

Minimalist photometric data reduction pipeline. Currently, supports the [Large Monolithic Imager (LMI)](https://jumar.lowell.edu/confluence/display/DCTIC/LMI) on the [4.3-m Discovery Channel Telescope (DCT)](https://lowell.edu/research/research-facilities/4-3-meter-dct/) at [Lowell Observatory](https://lowell.edu).

## Dependencies

The pipeline depends on the [Astr*O*matic](https://www.astromatic.net) tools, [Astropy](http://www.astropy.org), and a few [Astropy affiliated packages](http://www.astropy.org/affiliated): [CCDProc](http://ccdproc.readthedocs.io) and [Astroquery](http://astroquery.readthedocs.io).

To install these dependencies on Mac OS:

    $ sudo port install sextractor scamp swarp missfits py27-astropy py27-scipy
    $ pip install --user ccdproc astroquery

## Instructions

1.  Check out anywhere you like:

        $ git clone https://github.com/lpsinger/minphot.git /path/to/src

2.  Change to the directory that contains your raw images:

        $ cd /path/to/raw

3.  Run `minphot`, passing the filenames of your raw images to it. It will examine the image headers, generate a Makefile, and then run make:

        $ /path/to/src/minphot lmi.????.fits

    *Note*: after this stage, you can run `make clean` to nuke the analysis data products (leaving the raw images intact), or run `make` to redo any part of the analysis.

4.  Last, you can extract photometry of individual targets:

        $ /path/to/src/minphot-summarize targets.lis *.solved.cat
