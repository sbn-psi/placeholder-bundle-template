Readme for PDS SBN LONEOS data holdings
Updated May 4, 2021

Overview
========

The Lowell Observatory Near-Earth Object Search (LONEOS) was a NASA-funded
NEO survey project which operated from January 2010 to March 2008.  During
its operation, LONEOS discovered 22,077 asteroids.  

In 2014, the PDS Small Bodies Node (SBN) began efforts to obtain and safe
the LONEOS data in hopes of eventually archiving it in the PDS.  A subset of
the data were still on RAID hard drives at Lowell Observatory,
and these eventually were sent to SBN and transferred to a storage server
and backed up.  The remainder of the data were on magnetic tapes.  In 2017,
these tapes were shipped to SBN in Tucson and eventually were sent to a data
recovery service for transfer to hard drive.  These data were added to the
SBN LONEOS data holdings.

The full SBN LONEOS data holdings are now being made available to the public 
domain as of Sept. 15, 2020 in their unrestored and unarchived form.  There
are no restrictions on the use of these data.  The data have no original
documentation, non-standard FITS filenames, at least seven different
versions of FITS headers among the image files, and numerous duplications. 
These and other deficiencies would have to be ameliorated before the data
set could be archivable in PDS.

Contents of data directories
============================

Data recovered by Lowell Observatory from their RAID system:
These have the original directory names as provided by Lowell Observatory,
except when two directories had the same name, an "a" was appended to one
of them.  These directories have subdirectories by month and year.

/2000
/2003
/2004
/2004_RAID
/2004a
/2005-backup
/2006-backup
/2007-backup
/2008-backup
/2010
/2010a
/2011


Data from the magnetic tapes:

/tape - These images were recovered in the initial data recovery run. This
test run consisted of a small sample of the tapes. The subdirectories in
this directory are based on tape number. Beyond that, the names are what
were provided by the data recovery firm.

/recovered - These images were recovered in the main data recovery run.
These were all of the remaining LONEOS backup tapes. The subdirectories in
this directory are based on tape number. Beyond that, the names are what
were provided by the data recovery firm.


Notes on the LONEOS data
========================

 * Information from the FITS headers of the LONEOS image files are often not
correct, especially the observing location, and the right ascension and
declination. The chip used for some images was rectangular, and two
consecutive frames moved one chip short length made up one survey field.
They were often named filea and fileb. The right ascensions and declination
recorded in the headers of filea and fileb correspond to the center of the
survey field and not the individual chips. If accurate coordinates are
needed, it is recommended to derive a plate solution or use astrometry.net. 

 * Keywords in the FITS headers are not consistent throughout the dataset
(e.g. UT or UTSTART are used for start of the observing time).

 * Duplicate images with different filenames might be present.


