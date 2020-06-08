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

Each recording contains an EDF signal file in the [European Data Format](http://www.edfplus.info/). [These EDFs](:files_path:/polysomnography/edfs) were exported from the original data collection system and processed in [Luna](http://zzz.bwh.harvard.edu/luna/).

## NSRR signal harmonization

Using [Luna](http://zzz.bwh.harvard.edu/luna/), a list of all channel names were extracted from the EDFs for the Wisconsin Sleep Cohort. Subsequently, the extracted channel names were assigned to a set of new standardized channel names, outlined on the [montage and sampling rate information page](:pages_path:/montage-and-sampling-rate-information.md). Later, the channel names in EDF files were changed to these standardized channel names for consistency with the montage page. Some recordings made on the Grass Heritage system contained two identically named airflow channels with differing traces. These naming issues were corrected, and the "duplicate" traces are now correctly distinguished as Nasal and Oral Airflow.

## History / changelog

*May 2020*
- WSC team submits raw EDF data to NSRR

## Questions?

Please reach out to us at support@sleepdata.org or in the [Forum](https://sleepdata.org/forum) if you have questions.
