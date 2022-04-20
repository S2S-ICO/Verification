# MJO Diagnostics Tools

## 1. Overviews
### [1] climpred: Verification of weather and climate forecasts
#### ※ "[climpred]" is listed here by courtesy of Aaron Spring. See the "[climpred]" for further details.
> There are many packages out there related to computing metrics on initialized geoscience predictions. However, we didn’t find any one package that unified all our needs.
>
> Output from earth system prediction hindcast (also called re-forecast) experiments is difficult to work with. A typical output file could contain the dimensions initialization, lead time, ensemble member, latitude, longitude, depth. climpred leverages the labeled dimensions of xarray to handle the headache of bookkeeping for you. We offer HindcastEnsemble and PerfectModelEnsemble objects that carry products to verify against (e.g., control runs, reconstructions, uninitialized ensembles) along with your initialized prediction output.
>
> When computing lead-dependent skill scores, climpred handles all of the init+lead-valid_time-matching for you, properly aligning the multiple time dimensions between the hindcast and verification datasets. We offer a suite of vectorized deterministic and probabilistic metrics that can be applied to time series and grids. It’s as easy as concatenating your initialized prediction output into one xarray.Dataset and running the HindcastEnsemble.verify() command:
```sh
HindcastEnsemble.verify(
    metric="rmse", comparison="e2o", dim="init", alignment="maximize"
)
```
</br></br>
### [2] Spaceholder for next item
</br>

## 2. Contents
### [1] climred </br>
> #### Numerical Weather Prediction
> - Calculate skill for NWP model GEFS for 6-hourly global forecasts
> #### Subseasonal
> - Calculate skill of a MJO Index of SubX model GEOS_V2p1 as function of daily lead time
> - Calculate skill of a MJO Index of S2S models as function of daily lead time
> - Calculate skill of a MJO Index of SubX model GEOS_V2p1 as function of weekly lead time
> - Calculate skill of S2S model ECMWF for daily global reforecasts
> #### Monthly and Seasonal
> - Calculate ENSO Skill of NMME model NCEP-CFSv2 as Function of Initial Month vs. Lead Time
> - Calculate Seasonal ENSO Skill of the NMME model NCEP-CFSv2
> #### Decadal
> - Demo of Perfect Model Predictability Functions
> - Hindcast Predictions of Equatorial Pacific SSTs
> - Diagnosing Potential Predictability
> - Significance Testing
> #### Misc
> - Using dask with climpred
> - climpred on CPU vs GPU
> - Setting up your own output
> - intake-esm for cmorized output

</br></br>
### [2] Spaceholder for next item
</br>

## 3. Installation Instructions

### [1] climpred </br>
> You can install the latest release of climpred using pip or conda:
```sh
pip install climpred[complete]
```
```sh
conda install -c conda-forege climpred
```
> See the "[climpred]" for detailed instructions

</br></br>
### [2] Spaceholder for next item
</br>

## 4. Examples
### [1] climpred </br>
> The detailed application of the technique can be checked through the link of each technique.
> #### Numerical Weather Prediction
> - [Calculate skill for NWP model GEFS for 6-hourly global forecasts]
> #### Subseasonal
> - [Calculate skill of a MJO Index of SubX model GEOS_V2p1 as function of daily lead time]
> - [Calculate skill of a MJO Index of S2S models as function of daily lead time]
> - [Calculate skill of a MJO Index of SubX model GEOS_V2p1 as function of weekly lead time]
> - [Calculate skill of S2S model ECMWF for daily global reforecasts]
> #### Monthly and Seasonal
> - [Calculate ENSO Skill of NMME model NCEP-CFSv2 as Function of Initial Month vs. Lead Time]
> - [Calculate Seasonal ENSO Skill of the NMME model NCEP-CFSv2]
> #### Decadal
> - [Demo of Perfect Model Predictability Functions]
> - [Hindcast Predictions of Equatorial Pacific SSTs]
> - [Diagnosing Potential Predictability]
> - [Significance Testing]
> #### Misc
> - [Using dask with climpred]
> - [climpred on CPU vs GPU]
> - [Setting up your own output]
> - [intake-esm for cmorized output]

</br></br>
### [2] Spaceholder for next item

(Detailed guide to run program codes will be described here!)

example)

```sh
MJODiagnostics(Parameter,...)
```
</br>

## 5. Issues
### [1] climpred
#### Patch note
The latest releases of climpred can be found on [climpred's github].

#### Additional usefull tool
[xskillscore] is an open source project and Python package that provides verification metrics of deterministic (and probabilistic from properscoring) forecasts with xarray.

</br></br>
### [2] Spaceholder for next item
</br>

## 6. Contributors & Acknowledgements
### [1] climpred
> #### Core Developers
> - Aaron Spring 
  [github]: https://github.com/aaronspring/
> - Riley X. Brady 
  [github]: https://github.com/bradyrx/
> #### Contributors
> - Andrew Huang 
  [github]: https://github.com/ahuang11/
> - Kathy Pegion 
  [github]: https://github.com/kpegion/
> - Anderson Banihirwe 
  [github]: https://github.com/andersy005/
> - Ray Bell 
  [github]: https://github.com/raybellwaves/

</br></br>
### [2] Spaceholder for next item
</br>

(Contributors and relevant Acknowledgements for program codes will be listed here!)

example)

The MJOWG wishes to acknowledge and thank U.S. CLIVAR and International CLIVAR for supporting this working group and its activities </br>
by MJO Simulation Diagnostics

## 7. How to cite
### [1] climpred
> See the "[climpred]" for detailed instructions </br>

</br></br>
### [2] Spaceholder for next item
</br>

(Citation for program codes will be listed here!)

example)

National Center for Atmospheric Research Staff (Eds). Last modified 08 Oct 2013. "[The Climate Data Guide: MJO]: Madden-Julian Oscillation Diagnostics." 

## 8. Disclaimer
Any claims against the Institute stemming from the use of any GitHub-related project will be governed.


  [climpred]: https://climpred.readthedocs.io/en/stable/examples.html#subseasonal
  [Manual]: https://climatedataguide.ucar.edu/climate-data/mjo-madden-julian-oscillation-diagnostics
  [The Climate Data Guide: MJO]: https://climatedataguide.ucar.edu/climate-data/mjo-madden-julian-oscillation-diagnostics
  [Calculate skill for NWP model GEFS for 6-hourly global forecasts]: https://climpred.readthedocs.io/en/stable/examples/NWP/NWP_GEFS_6h_forecasts.html#
  [Calculate skill of a MJO Index of SubX model GEOS_V2p1 as function of daily lead time]: https://climpred.readthedocs.io/en/stable/examples/subseasonal/daily-subx-example.html
  [Calculate skill of a MJO Index of S2S models as function of daily lead time]: https://climpred.readthedocs.io/en/stable/examples/subseasonal/daily-S2S-IRIDL.html
  [Calculate skill of a MJO Index of SubX model GEOS_V2p1 as function of weekly lead time]: https://climpred.readthedocs.io/en/stable/examples/subseasonal/weekly-subx-example.html
  [Calculate skill of S2S model ECMWF for daily global reforecasts]: https://climpred.readthedocs.io/en/stable/examples/subseasonal/daily-S2S-ECMWF.html
  [Calculate ENSO Skill of NMME model NCEP-CFSv2 as Function of Initial Month vs. Lead Time]: https://climpred.readthedocs.io/en/stable/examples/monseas/monthly-enso-subx-example.html
  [Calculate Seasonal ENSO Skill of the NMME model NCEP-CFSv2]: https://climpred.readthedocs.io/en/stable/examples/monseas/seasonal-enso-subx-example.html
  [Demo of Perfect Model Predictability Functions]: https://climpred.readthedocs.io/en/stable/examples/decadal/perfect-model-predictability-demo.html
  [Hindcast Predictions of Equatorial Pacific SSTs]: https://climpred.readthedocs.io/en/stable/examples/decadal/tropical-pacific-ssts.html
  [Diagnosing Potential Predictability]: https://climpred.readthedocs.io/en/stable/examples/decadal/diagnose-potential-predictability.html
  [Significance Testing]: https://climpred.readthedocs.io/en/stable/examples/decadal/Significance.html
  [Using dask with climpred]: https://climpred.readthedocs.io/en/stable/examples/misc/efficient_dask.html
  [climpred on CPU vs GPU]: https://climpred.readthedocs.io/en/stable/examples/misc/climpred_gpu.html
  [Setting up your own output]: https://climpred.readthedocs.io/en/stable/examples/misc/setup_your_own_data.html
  [intake-esm for cmorized output]: https://climpred.readthedocs.io/en/stable/examples/misc/setup_your_own_data.html#intake-esm-for-cmorized-output
  [S2S-ai-cahllenge]: https://github.com/ecmwf-lab/climetlab-s2s-ai-challenge
  [climpred's github]: https://github.com/pangeo-data/climpred
  [xskillscore]: https://github.com/xarray-contrib/xskillscore
