cr2fits
=======

cr2fits.py version **1.0.3m**
Forked from http://github.com/eaydin/cr2fits (1.0.3) to make some changes:

  - Extract all 3 channels from the RAW image and put them on a single 3D fits image (data cube)
  - Delete temporary PPM files
  - Automatically update FITS if there is a previous one.

A script to convert RAW images (canon, nikon etc.) to FITS images. I think this'll be useful for professional or amateur astronomers who happen to work with DSLR cameras and want to process their images with some astronomical tool (IRAF?).
It extracts 3 color channels of the RAW image, put it on a FITS data cube and writes the necessary EXIF information to the FITS header.

Dependencies :

- Python 2.6.x or later. (Including Python 3.2)
- PyFITS : You can get it with your package manager, or here : http://packages.python.org/pyfits/
- dcraw : Try getting the latest version of this. Usually the ones in repositories is not the latest so it's possible that it'll convert your RAW images differently, corrupted. Get the latest version here : http://www.cybercom.net/~dcoffin/dcraw/

Usage : 

`cr2fits.py <cr2-filename>`

- cr2-filename : This will obviously be the name of the file to convert.

Outputs :

The script will output the FITS file (a data cube image). Temporary PPM files are deleted after succesfully loaded as arrays



