# Polysomnography introduction

## Description and overview

The Sleep Research Laboratory is part of the Clinical and Translational Research Core of the University of Wisconsin.  The Research Laboratory is in a dedicated wing of the CTRC unit in University of Wisconsin Hospital and Clinics. The Sleep Research Lab consists of two sleep rooms and a control room. The sleep rooms are used almost exclusively by the Wisconsin Sleep Cohort Study, but are also available for other researchers.

## Equipment

[6/2000-10/2009]: Heritage System, Grass - Telefactor (**Gamma**)

Each sleep room is served by a single-bed Grass-Telefactor Heritage digital sleep system. The systems have 16 channels, 8 selectable and 8 fixed, with 4 DC coupled auxiliary inputs.  Both systems are equipped with 15A54 research amplifiers having a bandwidth of 0.5Hz-6kHz.

[10/2009 – 12/2015]: Comet Lab Based system, Grass Technologies (**Twin**)

Each sleep room is served by a single-bed Grass Technologies Comet Lab - based digital sleep system. The systems have 40 AC channels, 31 referential and 9 bipolar, with 8 DC coupled auxiliary inputs.  Both systems are equipped with AS40 research amplifiers having a bandwidth of 1.0Hz-100Hz.

In addition to the two recording systems, the control room also has a reviewer station for data analysis.  All systems are networked, allowing for off-site review and analysis.

The two sleep rooms and control room are equipped with state-of-the-art video and audio monitoring. Input/output connections between sleep room and control room are made through in-the-wall connector panels for increased assurance of optimum signal-to-noise ratios.

Polysomnography is obtained from EEG scalp electrodes, electrooculogram, EMG of chin and legs, ECG, snore microphone, airflow from Dymedix nasal-oral thermistor, Pro-Tech nasal pressure transducer, breathing effort from Pro-Tech zRIP inductance plethysmography summation systems, and oxygen hemoglobin from the Ohmeda 3900 oximeter using a 3-second averaging rate.

Notes:
- [WSCS Manual of Operations (PDF)](:files_path:/documentation/WSCS_Manual_of_Operations.pdf)
- [Montage and Sampling Rate Information](:pages_path:/montage-and-sampling-rate-information.md)
- [WSCS Scoring Annotation Documentation (XLSX)](:files_path:/documentation/wsc-scoring-annotation-documentation.xlsx)

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

- **.sco.txt** - WSC original respiratory event scoring for Gamma studies.
- **.stg.txt** - WSC original staging format for Gamma studies. The sleep staging codes are as follows:
  - 0: Wake
  - 1: N1
  - 2: N2
  - 3: N3
  - 4: N4
  - 5: REM
  - 6: Movement
  - 7: No stage
- **.log.txt** - WSC original biocalibrations and light indicators for Gamma studies.
- **.allscore.txt** - WSC original staging and respiratory event scoring for Twin studies.

The staging and scoring rules are described in the [WSC Manual of Operations](:files_path:/documentation/WSCS_Manual_of_Operations.pdf). The WSC team [provided a spreadsheet](:files_path:/documentation/wsc-scoring-annotation-documentation.xlsx) with additional details about the annotation files.

## NSRR signal harmonization

Using [Luna](http://zzz.bwh.harvard.edu/luna/), a list of all channel names were extracted from the EDFs for the Wisconsin Sleep Cohort. Subsequently, the extracted channel names were assigned to a set of new standardized channel names, outlined on the [montage and sampling rate information page](:pages_path:/montage-and-sampling-rate-information.md). Later, the channel names in EDF files were changed to these standardized channel names for consistency with the montage page. Some recordings made on the Grass Heritage system contained two identically named airflow channels with differing traces. These naming issues were corrected, and the "duplicate" traces are now correctly distinguished as Nasal and Oral Airflow.

## History / changelog

*June 2021*
- .eannot staging files removed. The NSRR team will revisit harmonized EDFs/annotations in the future. Please use the original WSC annotation files at this time.

*November 2020*
- Add .eannot staging files and original scoring annotation files

*August 2020*
- Deposit 2,570 EDFs on NSRR

*May 2020*
- WSC team submits raw EDF data to NSRR

## Questions?

Please reach out to us at support@sleepdata.org or in the [Forum](https://sleepdata.org/forum) if you have questions.
