# iau-star-names
[![collect-data-monthly](https://github.com/cyschneck/iau-star-names/actions/workflows/collect_data_monthly.yml/badge.svg)](https://github.com/cyschneck/iau-star-names/actions/workflows/collect_data_monthly.yml)

All IAU named stars are collected from [IAU-Catalog of Star Names](https://exopla.net/star-names/modern-iau-star-names/)

Last updated: **November 28, 2025**

`iau_data.csv`:
- Proper Names
- WGSN ID
- Desgination
- HIP
- Bayer ID
- Constellation
- Origin
- Ethnic/Cultural Group/Language
- Reference
- Additional Information
- Date of Adoption

`star_names.csv` data is collected via automatic web scraping from [`in-the-sky.org`](https://github.com/cyschneck/iau-star-names/blob/main/data/2_inthesky_star_data.csv) and [`wikipedia.org`](https://github.com/cyschneck/Star-Chart-Spherical-Projection/blob/main/star_chart_spherical_projection/data/3_backup_star_data.csv) (and some [manual additions](https://github.com/cyschneck/iau-star-names/blob/main/data/0_missing_manual.csv)
- Common Name
- Right Ascension (HH.MM.SS)
- Declination (DD.SS)
- Magnitude (V, Visual)
- Proper Motion Speed (mas/yr)
- Proper Motion Angle (DD.SS)
- Proper Motion RA (mas/yr)
- Proper Motion DEC (mas/yr)
- Alternative Names
- URL

> [!NOTE]
> IAU WGSN distinguishes between the star `Nganurganity` and `Unurgunite`, even though they share the same Designation (HR 2646) and HIP (33856) that both represent the star [Sigma Canis Majoris](https://en.wikipedia.org/wiki/Sigma_Canis_Majoris). In the `star_data.csv` this will be listed as `Nganurganity` with `Unurgunite` in the list of alternative names

> [!IMPORTANT]
> Betelgeuse's companion star, Betelgeuse B (offically named `Siwarha`) was declared on [July 24, 2025](https://iopscience.iop.org/article/10.3847/2041-8213/adeaaf) and, as of yet, has no designation or proper motion so it is not currently included in `stars_with_data.csv`

## Development Environment
To run or test against this github repo/fork, a development environment can be created via conda/miniconda

First, [install Miniconda](https://docs.conda.io/projects/miniconda/en/latest/miniconda-install.html)

Then, using the existing `environment.yml`, a new conda environment can be create to run against

```
conda env create --file environment.yml
```
Once the environment has been built, activate the environment:
```
conda activate iau_stars
```

## Bibliography

Named stars specified by ["IAU Catalog of Star Names"](https://exopla.net/star-names/modern-iau-star-names/) with the star position (right ascension and declination) as well as the angle and speed of proper motion from [in-the-sky.org](https://in-the-sky.org/) and Wikipedia where indicated
