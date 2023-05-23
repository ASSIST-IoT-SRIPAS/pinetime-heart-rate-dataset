# PineTime heart rate dataset

Dataset of heart rate measurements collected from the PineTime wristband, with a gold standard reference.

## Contents

The repository contains both the raw and the "merged", clean data. The merged data is much easier to work with and should be used when building machine learning models. The raw data is provided for transparency, reproducibility, and to allow for studies that could use the other data collected from the Equivital device.

- `schedule.md` – schedule of the study, indicating the start and end times of each exercise and break.
- `data_raw/` – raw data collected from the PineTime wristband and the Equivital device. Each subdirectory corresponds to one participant. The files are in the [Feather format](https://arrow.apache.org/docs/python/feather.html).
- `data_merged/` – merged data series that can be used for building ML models. The files are in JSON format and follow a nested structure, where each heart rate measurement is associated with a series of acceleration measurements that preceded it. Each file corresponds to one continuous measurement session – there are sometimes multiple sessions per participant due to intermittent hardware failures.

## Authors

- [Monika Kobus](https://orcid.org/0000-0003-3217-1050) – data collection
- [Anna Dąbrowska](https://orcid.org/0000-0003-4295-3005) – data collection
- [Piotr Sowiński](https://orcid.org/0000-0002-2543-9461) – data collection and processing

## Acknowledgements

This work is part of the [ASSIST-IoT project](https://assist-iot.eu/) that has received funding from the EU’s Horizon 2020 research and innovation programme under grant agreement No 957258.

The [Central Institute for Labour Protection – National Research Institute's](https://www.ciop.pl/en) provided facilities and equipment for data collection.

## License

The dataset is licensed under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).
