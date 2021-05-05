NSRR Harmonized version of WSC dataset provides users with a unique set of files with basic validations, summaries of annotations & channels, and Canonical files.  This NSRR Harmonized version has gone through the below processing steps:
1. Checks to identify inconsistent files
    1. Evaluate consistent Data Delimiter and number of columns across all scoring files with particular category 
    2. Evaluate EDF Sample rate to identify any floating/weird values
    3. Evaluate EDF duration to identify any floating/weird values
    4. Evaluate alignment of Epochs and annotations
All the inconsistent files from above checks are added to 'excludes' file

2. Summary:
    1. Annotations and stages summary are stored in '.annots' and '.stages' files respectively
    2. Channels summary is stored in '.channels' file

3. Annotations processing:
    1. Annotations are re-mapped to NSRR terms 
    2. Based on above mapping, '.annot' and '.eannot' files are generated

4. Channels processing:
    1. Canonical Signals definitions are created and stored in sigs.canonical file found at [sigs.canonical] (https://gitlab-scm.partners.org/zzz-public/nsrr/-/blob/master/studies/wsc/sigs.canonical)
    2. Canonical EDF's and sample list are generated based on sigs.canonical file
        - Regenerated Signals (EEG,ECG,EMG,LOC,ROC,CAN,TRM,THX,ABD,OXY and POS) with prefix 'cs'
        - Re-sampled above Signals
        - Dropped all other signals


Above process of Harmonization of WSC dataset is captured in detail at [proc.md] (https://gitlab-scm.partners.org/zzz-public/nsrr/-/blob/master/studies/wsc/proc.md)


## File Structure

- **.eannot** - One row per epoch with an indication of scored sleep stage (e.g. *wake*, *N1*, *N2*, *N3*, *REM*). These annotation files were created by the NSRR team using Luna. [Read more about Luna's .eannot annotation format.](http://zzz.bwh.harvard.edu/luna/ref/annotations/#eannot-files)

1. Canonical EDF's and Sample list
2. .eannot and .annot files
3. Annotation summary file(s)
4. Channel summary file
5. excludes files


## Signal harmonization

Using [Luna](http://zzz.bwh.harvard.edu/luna/), a list of all channel names were extracted from the EDFs for the Wisconsin Sleep Cohort. Subsequently, the extracted channel names were assigned to a set of new standardized channel names, outlined on the [montage and sampling rate information page](:pages_path:/montage-and-sampling-rate-information.md). Later, the channel names in EDF files were changed to these standardized channel names for consistency with the montage page. Some recordings made on the Grass Heritage system contained two identically named airflow channels with differing traces. These naming issues were corrected, and the "duplicate" traces are now correctly distinguished as Nasal and Oral Airflow.

## History / changelog

*May 2021*
- Added version 1 of NSRR Harmonized files

## Questions?

Our efforts as part of harmonization is to identify and capture issues in Original Dataset of WSC study. As our Harmoziation processes are still evolving, we cannot ensure that we had captured 100% of persisting issues in the study. Feel free to report the errors as you may find them.

Please reach out to us at support@sleepdata.org or in the [Forum](https://sleepdata.org/forum) if you have questions.