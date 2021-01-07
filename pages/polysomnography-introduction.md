# Polysomnography introduction

The Sleep Research Laboratory is part of the Clinical and Translational Research Core of the University of Wisconsin.  The Research Laboratory is in a dedicated wing of the CTRC unit in University of Wisconsin Hospital and Clinics. The Sleep Research Lab consists of two sleep rooms and a control room. The sleep rooms are used almost exclusively by the Wisconsin Sleep Cohort Study, but are also available for other researchers.

Notes:
- [WSCS Manual of Operations (PDF)](:files_path:/documentation/WSCS_Manual_of_Operations.pdf)
- [Montage and Sampling Rate Information](:pages_path:/montage-and-sampling-rate-information.md)

## Signal files

The WSC cohort contains [raw polysomnography signal data](:files_path:/polysomnography) for 2,570 overnight recordings. The study visit breakdown is as follows:

- 1,123 recordings at Visit 1
- 758 recordings at Visit 2
- 566 recordings at Visit 3
- 121 recordings at Visit 4
- 2 recordings at Visit 5

Each recording contains an EDF signal file in the [European Data Format](http://www.edfplus.info/). [These EDFs](:files_path:/polysomnography) were exported from the original data collection system and processed in [Luna](http://zzz.bwh.harvard.edu/luna/).

## Annotation files

The WSC team provided sleep staging and respiratory event scoring annotations. These annotations are [available alongside the .EDF signal files](:files_path:/polysomnography) in the following formats:

- **.eannot** - One row per epoch with an indication of scored sleep stage (e.g. *wake*, *N1*, *N2*, *N3*, *REM*). These annotation files were created by the NSRR team using Luna. [Read more about Luna's .eannot annotation format.](http://zzz.bwh.harvard.edu/luna/ref/annotations/#eannot-files)
- **.sco.txt** - WSC original respiratory event scoring for Gamma studies.
- **.stg.txt** - WSC original staging format for Gamma studies.
- **.log.txt** - WSC original biocalibrations and light indicators for Gamma studies.
- **.allscore.txt** - WSC original staging and respiratory event scoring for Twin studies.

The staging and scoring rules are described in the [WSC Manual of Operations](:files_path:/documentation/WSCS_Manual_of_Operations.pdf).

## NSRR signal harmonization

Using [Luna](http://zzz.bwh.harvard.edu/luna/), a list of all channel names were extracted from the EDFs for the Wisconsin Sleep Cohort. Subsequently, the extracted channel names were assigned to a set of new standardized channel names, outlined on the [montage and sampling rate information page](:pages_path:/montage-and-sampling-rate-information.md). Later, the channel names in EDF files were changed to these standardized channel names for consistency with the montage page. Some recordings made on the Grass Heritage system contained two identically named airflow channels with differing traces. These naming issues were corrected, and the "duplicate" traces are now correctly distinguished as Nasal and Oral Airflow.

## History / changelog

*November 2020*
- Add .eannot staging files and original scoring annotation files

*August 2020*
- Deposit 2,570 EDFs on NSRR

*May 2020*
- WSC team submits raw EDF data to NSRR

## Questions?

Please reach out to us at support@sleepdata.org or in the [Forum](https://sleepdata.org/forum) if you have questions.
