# Dataset introduction

The [WSC dataset](:files_path:/datasets) posted on the NSRR has gone through various post-processing steps in order to prepare the data for more widespread sharing. Changes and updates to the source data and variable definitions have been coordinated in the [wsc-data-dictionary repository](https://github.com/nsrr/wsc-data-dictionary).

**Disclaimer:** These data are not perfect. Please [submit issues](https://github.com/nsrr/wsc-data-dictionary/issues) for any new problematic findings.

## Structure

The [WSC dataset](:files_path:/datasets) contains 2,570 records. The dataset is deidentified. Individual participants are distinguished by the [wsc_id](https://sleepdata.org/datasets/wsc/variables/wsc_id) variable. Only participants who agreed to share their data have been included.

Participants have up to five (5) records in the dataset. Each record corresponds to a different research visit. Records are differentiated by the [wsc_vst](https://sleepdata.org/datasets/wsc/variables/wsc_vst) (study visit number) variable. The [vst_year](https://sleepdata.org/datasets/wsc/variables/vst_year) variable indicates the calendar year of each study visit. The study visit is primarily an indicator of chronology and not an indicator of distinct "waves" or "timepoints" of data collection across subjects.

Click [here to browse the WSC dataset variables](https://sleepdata.org/datasets/wsc/variables).

## Death tracking

The WSC team tracks incident events and deaths among enrolled subjects. Death certificate searches are completed on a regular basis. Cause of death comes from death certificates with an internal adjudication process to categorize cause of death into groups for research purposes. Click [here to browse the death adjudication variables](https://sleepdata.org/datasets/wsc/variables?folder=Clinical+Data/Incident+Outcomes).

## History / changelog

*July 2022*
- Version 0.5.0 of dataset released, replacing incident CVD/stroke data with death adjudication data

*April 2021*
- Version 0.2.0 of dataset released, including incident outcomes tracking

*May 2020*
- WSC team submits source data to NSRR

## Questions?

Please reach out to us at support@sleepdata.org or in the [Forum](https://sleepdata.org/forum) if you have questions.
