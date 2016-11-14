Sextractor for HPC
(source extraction for HPC)

Put all the images in the same directory and try first running e.g. 

sex Blind_03_N4_01.fits.fz_proj.fits -CATALOG_NAME test.cat  -WEIGHT_IMAGE Blind_03_N4_01_wtmap.fits.fz_proj.fits

to read the image Blind_03_N4_01.fits.fz_proj.fits with the noise map Blind_03_N4_01_wtmap.fits.fz_proj.fits and 
create a catalogue of stars in the file test.cat 

Then try diff test.cat Blind_03_N4_01_wtmap.fits.fz_proj.fit-catalogue.dat

to test for catalogue differences with the file Blind_03_N4_01_wtmap.fits.fz_proj.fit-catalogue.dat, which was obtained running

sex Blind_03_N4_01.fits.fz_proj.fits  -CATALOG_NAME Blind_03_N4_01_wtmap.fits.fz_proj.fit-catalogue.dat  -WEIGHT_IMAGE Blind_03_N4_01_wtmap.fits.fz_proj.fits
