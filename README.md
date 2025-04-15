# lunar-megaregolith-porosity-structure
The repository contains residual Bouguer anomaly data of observation craters and iSALE-2D simulation results.

## Repository Contents
- Data of observation craters
- Input files used to run iSALE-2D simulations
- Data for producing graphs similar to Figures 4, and 5 in the article (_publication in preparation_)

The simulations sed different target porosity structures, including porous layer thickness and pre-impact porosity. To distinguish between these parameters, the folders follow the following naming convention: `h(porous layer thickness)_P(pre-impact porosity)_I(impactor diameter)`. For example, **h3_P15_I1** stands for **h = 6 km**, **P = 15%**, **I = 1 km**. For exponential porosity structure, the files are named `EXP(exponential)_I(impactor diameter)`.

## observation data
**observation_data.csv**:The observed crater data used in Figure 2, including **Lon** (central longitude, deg), **Lat** (central latitude, deg), **Diam** (diameter, km), **RBA** (residual Bouguer anomaly, mGal), **Terrane** (FHT - 0, SPA - 2, mare - 3).

## iSALE input files
- **exponential porosity**: Impact settings of exponential porosity structures. `EXP_material.inp` is the material parameters used for these simulations.
- **two-layer porosity**: Impact settings of two-layer porosity structures. `P(pre-impact porosity)_material.inp` represent the material parameters of different pre-impact porosity for these simulations.

## simulation results
- For each model:
  - `porosity.txt`: the porosity data of the impact crater
  - `xc.txt`: the coordinate data of the model in the x direction
  - `yc.txt`: the coordinate data of the model in the y direction
