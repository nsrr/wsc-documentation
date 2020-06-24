# Montage and sampling rate information

The settings below represent the standards set at the beginning of the project. There may be a small proportion of studies and signals that do not match these standards exactly. Please review the settings at the individual sleep study level as you proceed with any analyses.

## Grass Comet Lab Based system (2009-present)
| Channel                       | EDF Label | Input 1  | Input 2 | Sampling rate (Hz) | Hardware filters (Hz) | Sensor type                                                |
|:-----------------------------:|:---------:|:--------:|:-------:|:------------------:|:---------------------:|:----------------------------------------------------------:|
| Left EOG                      | E1        | E1       | M2      | 200                | Low Pass 35           | -                                        |
| Right EOG                     | E2        | E2       | M1      | 200                | Low Pass 35           | -                                        |
| Left Frontal EEG              | F3_M2     | F3       | M2      | 200                | Low Pass 35           | -                                        |
| Frontal EEG                   | Fz_M2     | Fz       | M2      | 200                | Low Pass 35           | -                                        |
| Central EEG                   | Cz_M2     | Cz       | M2      | 200                | Low Pass 35           | -                                        |
| Left Central EEG              | C3_M2     | C3       | M2      | 200                | Low Pass 35           | -                                        |
| Parietal EEG                  | Pz_M2     | Pz       | M2      | 200                | Low Pass 35           | -                                        |
| Left Occipital EEG            | O1_M2     | O1       | M2      | 200                | Low Pass 35           | -                                        |
| Linked Center & Left Chin EMG | cchin_l   | cchin_l  | -    | 200                | Low Pass 70           |                                                            |
| Linked Left & Right Leg EMG   | lleg_r    | lleg_r   | -     | 200                | Low Pass 70           |                                                            |
| ECG                           | ECG       | ECG      | -       | 200                | Low Pass 35           |                                                            |
| Snore                         | snore     | snore    | -       | 200                | Low Pass 70           | Pro-Tech snore sensor                                      |
| Airflow                       | flow      | flow     | -       | 200                | Low Pass 15           | Dymedix disposible oral nasal airflow sensor               |
| Nasal Pressure                | nas_pres  | nas_pres | -       | 200                | Low Pass 15           | Pro-tech nasal pressure transducer                         |
| Thoracic IP                   | thorax    | thorax   | -       | 200                | Low Pass 15           | Pro-Tech Z-Rip inductance plethysmography summation system |
| Abdominal IP                  | abdomen   | abdomen  | -       | 200                | Low Pass 15           | Pro-Tech Z-Rip inductance plethysmography summation system |
| IP Sum                        | sum       | sum      | -       | 200                | Low Pass 15           | Pro-Tech Z-Rip inductance plethysmography summation system |
| Position                      | position  | position | -       | 200                | -                     | Natus Neurology DC body position sensor                    |
| SpO2                          | spo2      | spo2     | -       | 200                | -                     | Ohmeda 3900 Oximeter with a 3 second averaging rate        |


## Grass Heritage system (2000-2009)
| Channel                     | EDF Label | Input 1   | Input 2 | Sampling rate (Hz) | Hardware filters (Hz) | Sensor type                             |
|:---------------------------:|:---------:|:---------:|:-------:|:------------------:|:---------------------:|:---------------------------------------:|
| Left EOG                    | E1        | E1        | M2      | 100                | Low Pass 30           | -                     |
| Right EOG                   | E2        | E2        | M1      | 100                | Low Pass 30           | -                     |
| Left Central EEG            | C3_M2     | C3        | M2      | 100                | Low Pass 30           | -                     |
| Left Occipital EEG          | O1_M2     | O1        | M2      | 100                | Low Pass 30           | -                     |
| Chin EMG                    | chin      | chin      | Fpz     | 100                | Low Pass 30           | -                     |
| Linked Left & Right Leg EMG | lleg_r    | lleg_r    | Fpz     | 100                | Low Pass 30           | -                     |
| Snore                       | snore     | snore     | -       | 100                | Low Pass 30           | Microphone                              |
| ECG                         | ECG       | ECG       | -       | 100                | Low Pass 30           |                                         |
| Nasal Airflow               | nasalflow | nasalflow | -       | 100                | Low Pass 30           | Thermistor                              |
| Oral Airflow                | oralflow  | oralflow  | -       | 100                | Low Pass 30           | Thermistor                              |
| Nasal Pressure              | nas_pres  | nas_pres  | -       | 100                | Low Pass 30           | Transducer                              |
| Thoracic IP                 | thorax    | thorax    | -       | 100                | -                     | Respiratory inductance plethysmography  |
| Abdominal IP                | abdomen   | abdomen   | -       | 100                | -                     | Respiratory inductance plethysmography  |
| IP Sum                      | sum       | sum       | -       | 100                | -                     | Respiratory inductance plethysmography  |
| Position                    | position  | position  | -       | 100                | -                     | Body Position                           |
| SpO2                        | spo2      | spo2      | -       | 100                | -                     | Oximeter                                |

