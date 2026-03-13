# GEO Satellite Orbital Behaviour Analysis

This repository contains an exploratory analysis of **Geostationary (GEO) satellite orbital behaviour** using publicly available Two-Line Element (TLE) data.

The project focuses on identifying patterns in satellite motion such as station-keeping behaviour, orbital drift, and potential anomalies.

## Author

Gabriel Casarotto  
IPSA – Institut Polytechnique des Sciences Avancées

## Project Overview

Geostationary satellites are expected to remain near a fixed longitude above the equator.  
However, orbital perturbations and operational maneuvers can cause variations in their orbital parameters.

This project analyzes historical TLE data to better understand these behaviours.

The analysis includes:

- extraction of orbital parameters from TLE data
- temporal analysis of satellite orbital elements
- identification of station-keeping patterns
- detection of orbital drift or irregular behaviour

## Dataset

The dataset contains historical TLE records for several **GEO satellites**, identified by their **NORAD catalog ID**.

Each entry includes:

- epoch
- inclination
- right ascension of the ascending node (RAAN)
- eccentricity
- argument of perigee
- mean anomaly
- mean motion

These parameters allow the reconstruction and analysis of satellite orbital evolution.

## Analysis Performed

The notebook performs several exploratory analyses:

- parsing and preprocessing of TLE data
- time-series analysis of orbital parameters
- visualization of orbital evolution
- detection of possible maneuvers or abnormal behaviour

Visualizations include:

- temporal evolution of orbital elements
- comparison between satellites
- identification of stable vs drifting orbits

## Repository Structure
- analyse_de_donnees.ipynb # Exploratory analysis notebook
- mon_dataset_geo.csv # TLE dataset used for the analysis
- README.md

## Tools and Libraries

The analysis is performed using Python with the following libraries:

- NumPy
- Pandas
- Matplotlib

Additional libraries may be used to manipulate orbital data such as:

- sgp4
- astropy
- skyfield

## Applications

Understanding GEO satellite behaviour is important for:

- **Space Situational Awareness (SSA)**
- satellite operations monitoring
- detection of orbital maneuvers
- space traffic management

## Notes

This project was originally inspired by an orbital analysis workflow similar to those used in **space surveillance and tracking applications**.

![image alt]([https://github.com/gabriel-casarotto/GEO-Satellite-Orbital-Behaviour-Analysis/blob/main/station%20keeping.png?raw=true](https://raw.githubusercontent.com/gabriel-casarotto/GEO-Satellite-Orbital-Behaviour-Analysis/refs/heads/main/station_keeping.png)

![image alt]([https://github.com/gabriel-casarotto/GEO-Satellite-Orbital-Behaviour-Analysis/blob/main/Orbital%20Status.png?raw=true](https://raw.githubusercontent.com/gabriel-casarotto/GEO-Satellite-Orbital-Behaviour-Analysis/refs/heads/main/drifting.png)

![alt image](https://raw.githubusercontent.com/gabriel-casarotto/GEO-Satellite-Orbital-Behaviour-Analysis/refs/heads/main/orbital_status_geo.png)
